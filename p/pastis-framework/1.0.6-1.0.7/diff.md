# Comparing `tmp/pastis-framework-1.0.6.tar.gz` & `tmp/pastis-framework-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastis-framework-1.0.6.tar", last modified: Sun Jul 30 15:22:05 2023, max compression
+gzip compressed data, was "pastis-framework-1.0.7.tar", last modified: Fri Aug  4 21:42:41 2023, max compression
```

## Comparing `pastis-framework-1.0.6.tar` & `pastis-framework-1.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16489 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastis-benchmark
--rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastis-broker
--rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastisd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/bin/pastis-aflpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/aflpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/pastis-honggfuzz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/honggfuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/bin/pastis-triton
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/pastisdse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/libpastis/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/enginedesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/libpastis/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/proto/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/sast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastis_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastisbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/replayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastisbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/stat_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16489 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/bin/pastis-benchmark
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/bin/pastis-broker
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/bin/pastisd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-aflpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-aflpp/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/bin/pastis-aflpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-aflpp/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-aflpp/broker-addon/aflppbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/aflpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-honggfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-honggfuzz/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/bin/pastis-honggfuzz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-honggfuzz/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-honggfuzz/broker-addon/hfbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/honggfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-triton/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-triton/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-triton/bin/pastis-triton
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.376534 pastis-framework-1.0.7/engines/pastis-triton/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-triton/broker-addon/pastisttbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.380534 pastis-framework-1.0.7/engines/pastis-triton/pastisdse/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-triton/pastisdse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/engines/pastis-triton/pastisdse/pastisdse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/libpastis/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/enginedesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/libpastis/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/proto/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/sast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/libpastis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/pastis_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-04 21:42:41.000000 pastis-framework-1.0.7/pastis_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-04 21:42:41.000000 pastis-framework-1.0.7/pastis_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:42:41.000000 pastis-framework-1.0.7/pastis_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 21:42:41.000000 pastis-framework-1.0.7/pastis_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 21:42:41.000000 pastis-framework-1.0.7/pastis_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/pastisbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbenchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbenchmark/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbenchmark/replayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbenchmark/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/pastisbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10600 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/stat_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/pastisbroker/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:42:41.384534 pastis-framework-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-04 21:42:40.000000 pastis-framework-1.0.7/setup.py
```

### Comparing `pastis-framework-1.0.6/LICENSE` & `pastis-framework-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/PKG-INFO` & `pastis-framework-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.6
+Version: 1.0.7
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.6/README.md` & `pastis-framework-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/bin/pastis-benchmark` & `pastis-framework-1.0.7/bin/pastis-benchmark`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/bin/pastis-broker` & `pastis-framework-1.0.7/bin/pastis-broker`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/bin/pastisd` & `pastis-framework-1.0.7/bin/pastisd`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/bin/pastis-aflpp` & `pastis-framework-1.0.7/engines/pastis-aflpp/bin/pastis-aflpp`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/__init__.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/aflpp.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/aflpp.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/driver.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/replay.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/workspace.py` & `pastis-framework-1.0.7/engines/pastis-aflpp/pastisaflpp/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/pastis-honggfuzz` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/bin/pastis-honggfuzz`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/__init__.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/driver.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/honggfuzz.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/replay.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/workspace.py` & `pastis-framework-1.0.7/engines/pastis-honggfuzz/pastishf/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-triton/bin/pastis-triton` & `pastis-framework-1.0.7/engines/pastis-triton/bin/pastis-triton`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py` & `pastis-framework-1.0.7/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/engines/pastis-triton/pastisdse/pastisdse.py` & `pastis-framework-1.0.7/engines/pastis-triton/pastisdse/pastisdse.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/agent.py` & `pastis-framework-1.0.7/libpastis/agent.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/enginedesc.py` & `pastis-framework-1.0.7/libpastis/enginedesc.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/package.py` & `pastis-framework-1.0.7/libpastis/package.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/proto/message_pb2.py` & `pastis-framework-1.0.7/libpastis/proto/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/sast.py` & `pastis-framework-1.0.7/libpastis/sast.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/types.py` & `pastis-framework-1.0.7/libpastis/types.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/libpastis/utils.py` & `pastis-framework-1.0.7/libpastis/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastis_framework.egg-info/PKG-INFO` & `pastis-framework-1.0.7/pastis_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.6
+Version: 1.0.7
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.6/pastis_framework.egg-info/SOURCES.txt` & `pastis-framework-1.0.7/pastis_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbenchmark/models.py` & `pastis-framework-1.0.7/pastisbenchmark/models.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbenchmark/plotter.py` & `pastis-framework-1.0.7/pastisbenchmark/plotter.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbenchmark/replayer.py` & `pastis-framework-1.0.7/pastisbenchmark/replayer.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbenchmark/results.py` & `pastis-framework-1.0.7/pastisbenchmark/results.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbroker/broker.py` & `pastis-framework-1.0.7/pastisbroker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     NO_TRANSMIT = 2       # Does not transmit seed to peers (for comparing perfs of tools against each other)
 
 
 
 
 class PastisBroker(BrokerAgent):
 
+    PROXY_NETID = b"PROXY"
+    PROXY_ID = "PROXY"
+
     def __init__(self, workspace: PathLike,
                  binaries_dir: PathLike,
                  broker_mode: BrokingMode,
                  check_mode: CheckMode = CheckMode.CHECK_ALL,
                  inject_loc: SeedInjectLoc = SeedInjectLoc.STDIN,
                  sast_report: PathLike = None,
                  p_argv: List[str] = None,
@@ -114,15 +117,16 @@
         self._startup_quorum = start_quorum
         self._current_quorum = 0
 
         # Proxy feature
         self._proxy = None
         self._proxy_cli = None
         self._proxy_start_signal = False
-        self._proxy_seed_queue = queue.Queue()
+        self._proxy_to_clis = queue.Queue()
+        self._clis_to_proxy = queue.Queue()
 
         # Coverage + filtering feature
         self._coverage_manager = None
         self.filter_inputs: bool = filter_inputs
         if filter_inputs or stream:
             if (path := self.find_vanilla_binary()) is not None:  # Find an executable suitable for coverage
                 logging.info(f"Coverage binary: {path}")
@@ -200,15 +204,16 @@
         self.register_stop_coverage_callback(self.stop_coverage_received)
         self.register_data_callback(self.data_received)
 
     def get_client(self, cli_id: bytes) -> Optional[PastisClient]:
         cli = self.clients.get(cli_id)
         if not cli:
             logging.warning(f"client '{cli_id}' unknown (send stop)")
-            self.send_stop(cli_id)
+            if cli.netid != self.PROXY_NETID:
+                self.send_stop(cli_id)
         return cli
 
     def kick_client(self, cli_id: bytes) -> None:
         cli = self.clients.pop(cli_id)  # pop it from client list
         logging.info(f"kick client: {cli.strid}")
         self.send_stop(cli_id)
 
@@ -217,45 +222,57 @@
         if not cli:
             return
         is_new = seed not in self._seed_pool
         h = md5(seed).hexdigest()
 
         # Show log message and save seed to file
         self.statmanager.update_seed_stat(cli, typ)  # Add info only if new
-        cli.log(LogLevel.INFO, f"seed {h} [{self._colored_seed_type(typ)}][{self._colored_seed_newness(is_new)}]")
+        cli.log(LogLevel.INFO, f"seed {h} [{cli.strid}][{self._colored_seed_type(typ)}][{self._colored_seed_newness(is_new)}]")
         cli.add_own_seed(seed)  # Add seed in client's seed
         fname = self.write_seed(typ, cli.strid, seed) # Write seed to file
 
         if is_new:
-            if self._coverage_manager:
-                sp = fname.split("_")
-                covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], h, fname, typ, cli.netid, cli.strid, "GRANTED", "", -1, [])
-                self._coverage_manager.push_input(covi)
+            if self.is_proxied and not cli.strid == self.PROXY_ID:  # Directly forward to proxy if not proxy
+                self._clis_to_proxy.put((cli.netid, typ, seed))
+
+            if self._coverage_manager:  # True if filter_is_activated
+                self.push_input_filtering(cli.netid, cli.strid, fname, seed, typ)
 
             if not self.filter_inputs:  # If seed are not filtered send it right away
                 self.seed_granted(cli.netid, typ, seed)
         else:
             logging.debug(f"receive duplicate seed {h} by {cli.strid}")
 
+    def push_input_filtering(self, netid: bytes, id: str, fname: str, seed: bytes, typ: SeedType) -> None:
+        sp = fname.split("_")
+        covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], md5(seed).hexdigest(),
+                           fname, typ, netid, id, "GRANTED", "", -1, [])
+        self._coverage_manager.push_input(covi)
+
     def seed_granted(self, cli_id: bytes, typ: SeedType, seed: bytes):
         # Save it in the local pool
         self._seed_pool[seed] = typ
+        if cli_id == b"PROXY":
+            self._init_seed_pool[seed] = typ
 
         # Iterate on all clients and send it to whomever never received it
         if self.broker_mode == BrokingMode.FULL:
             self.send_seed_to_all_others(cli_id, typ, seed)
 
-        if self.is_proxied:  # Forward it to the proxy
-            self._proxy.send_seed(typ, seed)
-
     def send_seed_to_all_others(self, origin_id: bytes, typ: SeedType, seed: bytes) -> None:
         for c in self.iter_other_clients(origin_id):
-            if c.is_new_seed(seed):
-                self.send_seed(c.netid, typ, seed)  # send the seed to the client
-                c.add_peer_seed(seed)  # Add it in its list of seed
+            self.send_seed_to(c, typ, seed)
+
+    def send_seed_to(self, cli: PastisClient, typ: SeedType, seed: bytes) -> None:
+        if cli.is_new_seed(seed):
+            if cli.netid == self.PROXY_NETID:
+                self._proxy.send_seed(typ, seed)
+            else:
+                self.send_seed(cli.netid, typ, seed)  # send the seed to the client
+            cli.add_peer_seed(seed)  # Add it in its list of seed
 
     def add_seed_file(self, file: PathLike, initial: bool = False) -> None:
         p = Path(file)
         logging.info(f"Add seed {p.name} in pool")
         # Save seed in the workspace
         self.workspace.save_seed_file(SeedType.INPUT, p, initial)
 
@@ -398,15 +415,16 @@
             logging.info(
                 f"Launch client {cli.strid} as its targeting an address that has just been validated")
             self.start_client_and_send_corpus(cli)
 
     def stop_broker(self):
         for client in self.clients.values():
             logging.info(f"Send stop to {client.strid}")
-            self.send_stop(client.netid)
+            if client.netid != self.PROXY_NETID:
+                self.send_stop(client.netid)
         self._stop = True
 
         # Stop coverage manager if any
         if self._coverage_manager:
             self._coverage_manager.stop()
 
         # Call the statmanager to wrap-up values
@@ -505,15 +523,15 @@
                     logging.error(f"No alert target for binary package {package.name}")
             else:
                 logging.error(f"In mode {self.ck_mode} but the binary package is not a QBinExport")
                 return
 
         # Update internal client info and send him the message
         engine_args_str = engine_args.to_str() if engine_args else ""
-        logging.info(f"send start client {client.id}: {package.name} [{engine.NAME}, {covmode.name}, {fuzzmod.name}, {exmode.name}]")
+        logging.info(f"send start client {client.strid}: {package.name} [{engine.NAME}, {covmode.name}, {fuzzmod.name}, {exmode.name}]")
         client.set_running(package.name, engine, covmode, exmode, self.ck_mode, engine_args_str)
         client.configure_logger(self.workspace.log_directory, random.choice(COLORS))  # Assign custom color client
 
         self.send_start(client.netid,
                         package.name,
                         package.executable_path if package.is_standalone() else package.make_package(),
                         self.argv,
@@ -644,22 +662,34 @@
 
                 if self._running: # Perform following checks only if running
                     # if inputs are filtered. Get granted inputs and forward them to appropriate clients
                     if self.filter_inputs:
                         for item in self._coverage_manager.iter_granted_inputs():
                             self.seed_granted(item.fuzzer_id, item.seed_status, item.content)
 
-                    # Check if there are seed coming from the proxy-master to forward to clients
-                    if not self._proxy_seed_queue.empty():
-                        try:
-                            while True:
-                                origin, typ, seed = self._proxy_seed_queue.get_nowait()
-                                self.send_seed_to_all_others(origin, typ, seed)
-                        except queue.Empty:
-                            pass
+                    if self.is_proxied:
+                        # Check if there are seed to forward to primary (proxy main)
+                        cli = self.clients[self.PROXY_NETID]
+                        if not self._clis_to_proxy.empty():
+                            try:
+                                while True:
+                                    _, typ, seed = self._clis_to_proxy.get_nowait()
+                                    self.send_seed_to(cli, typ, seed)
+                            except queue.Empty:
+                                pass
+
+                        # Check if there are seed coming from the proxy to forward to clients
+                        # Used: only if filtering is disabled (otherwise goes through coverageManager)
+                        if not self._proxy_to_clis.empty():
+                            try:
+                                while True:
+                                    origin, typ, seed = self._proxy_to_clis.get_nowait()
+                                    self.seed_received(origin, typ, seed)
+                            except queue.Empty:
+                                pass
 
                 if self._stop:
                     logging.info("broker terminate")
                     break
         except KeyboardInterrupt:
             logging.info("stop required (Ctrl+C)")
         self.workspace.status = WorkspaceStatus.FINISHED
@@ -764,14 +794,18 @@
     @property
     def is_proxied(self) -> bool:
         """
         Get if the broker as a proxy to another broker.
         """
         return self._proxy is not None
 
+    @property
+    def is_filter_activated(self) -> bool:
+        return bool(self.filter_inputs)
+
     def set_proxy(self, ip: str, port: int, py_module: str) -> bool:
         self._proxy = ClientAgent()
 
         # Load the engine info to impersonate
         desc = load_engine_descriptor(py_module)
         if desc is None:
             logging.error("Cannot load FuzzingEngineDescriptor")
@@ -783,33 +817,33 @@
         self._proxy.register_seed_callback(self._proxy_seed_received)
         self._proxy.register_stop_callback(self._proxy_stop_received)
 
         logging.info(f"connect to broker {ip}:{port}")
         self._proxy.connect(ip, port)
         self._proxy.start()
 
+        # Create "fake" client object
+        cli = PastisClient(self.new_uid(), self.PROXY_NETID, [], Arch.X86_64, 0, 0, "proxy", Platform.LINUX)
+        cli.set_running("", desc, CoverageMode.AUTO, ExecMode.AUTO, self.ck_mode, "")
+        cli.configure_logger(self.workspace.log_directory, random.choice(COLORS))
+        self.clients[self.PROXY_NETID] = cli
+
     def _proxy_start_received(self, fname: str, binary: bytes, engine: FuzzingEngineInfo, exmode: ExecMode,
                               fuzzmode: FuzzMode, chkmode: CheckMode, covmode: CoverageMode, seed_inj: SeedInjectLoc,
                               engine_args: str, argv: List[str], sast_report: str = None):
         # FIXME: Use parameters received
         logging.info("[PROXY] start received !")
         self._running = True
         self._proxy_start_signal = True
         # if self._running:
         #     self.start_pending_clients()
 
     def _proxy_seed_received(self, typ: SeedType, seed: bytes):
         # Forward the seed to underlying clients
         logging.info(f"[PROXY] receive {md5(seed).hexdigest()} [{typ.name}] (forward it)")
 
-        # Save the seed locally
-        self.write_seed(typ, "PROXY", seed)
-        self._seed_pool[seed] = typ  # add it to the pool
-        self._init_seed_pool[seed] = typ  # also consider it as initial corpus
-
-        # Forward it to all clients
-        self._proxy_seed_queue.put((b"PROXY", typ, seed))
-        # self.send_seed_to_all_others(b"PROXY", typ, seed)
+        # Forward it to main thread to be handled as normal seed
+        self._proxy_to_clis.put((b"PROXY", typ, seed))
 
     def _proxy_stop_received(self):
         logging.info(f"[PROXY] stop received!")
         self._stop = True
```

### Comparing `pastis-framework-1.0.6/pastisbroker/client.py` & `pastis-framework-1.0.7/pastisbroker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,18 @@
             hldr = logging.FileHandler(log_dir/f"{self.strid}.log")
             hldr.setLevel(logging.DEBUG)
             hldr.setFormatter(logging.Formatter("%(asctime)s [%(levelname)s]: %(message)s"))
             self.logger.addHandler(hldr)
 
     @property
     def strid(self):
-        return f"CLI-{self.id}-{self._engine.SHORT_NAME if self._engine else 'N/A'}"
+        if self.netid == b"PROXY":
+            return "PROXY"
+        else:
+            return f"CLI-{self.id}-{self._engine.SHORT_NAME if self._engine else 'N-A'}"
 
     def is_new_seed(self, seed: bytes) -> bool:
         """
         Return true if the seed has never been sent to a client
 
         :param seed: seed bytes
         :return: True if never sent to client
```

### Comparing `pastis-framework-1.0.6/pastisbroker/coverage.py` & `pastis-framework-1.0.7/pastisbroker/coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,60 +148,62 @@
                 item, cov_file = self.cov_queue.get(timeout=0.5)
                 # logging.info("Coverage worker fetch item")
                 new_items = []
                 try:
                     coverage: CoverageSingleRun = QBDITrace.from_file(cov_file).coverage
                     if self._coverage.improve_coverage(coverage):
                         self.cli_stats[item.fuzzer_id][1] += 1  # input accepted
-                        self.seeds_accepted += 1
 
                         # Get newly covered items (and put them in the stream queue
-
                         new_items = coverage.difference(self._coverage)
 
                         item.new_coverage = list(new_items)
 
-                        # logging.info(f"seed {item.hash}  ({item.fuzzer_name}) [replay:{}][status:{}] ({len(new_items)} new edges)")
-
                         # Update the global coverage
                         self._coverage.merge(coverage)
 
-                        if item.fuzzer_name != "INITIAL":  # if not initial corpus and granted
-                            self.granted_queue.put(item)
+                        self.grant_input(item)
 
                     else:
                         item.broker_status = "DROPPED" if self.filter_enabled else "GRANTED"
                         # logging.info(f"seed {item.hash} ({item.seed_status.name}) of {item.fuzzer_name} rejected (do not improve coverage)")
 
                     # Remove the coverage file
                     os.unlink(cov_file)
 
                 except json.JSONDecodeError:
                     item.replay_status = "FAIL_PARSE_COV"
                     os.unlink(cov_file)
-                    self.seeds_accepted += 1
-                    if item.fuzzer_name != "INITIAL":  # if not initial corpus add it
-                        self.granted_queue.put(item)
+                    self.grant_input(item)
 
                 except FileNotFoundError:
                     # Grant input
-                    self.seeds_accepted += 1
-                    if item.fuzzer_name != "INITIAL":  # if not initial corpus add it
-                        self.granted_queue.put(item)
+                    self.grant_input(item)
 
                 logging.info(f"seed {item.hash} ({item.fuzzer_name}) [replay:{self.mk_rpl_status(item.replay_status)}][{self.mk_broker_status(item.broker_status, bool(new_items))}][{int(item.replay_time):}s] ({len(new_items)} new edges) (pool:{self.input_queue.qsize()})")
                 # Regardless if it was a success or not log it
                 self.add_item_coverage_stream(item)
             except queue.Empty:
                 pass
             except KeyboardInterrupt:
                 self._running = False
                 logging.info("coverage worker stop")
                 break
 
+    def grant_input(self, item: ClientInput) -> None:
+        """
+        Add the input to the granted_queue if
+        filtering is activated and the input is not
+        part of the initial.
+        """
+        self.seeds_accepted += 1
+        if self.filter_enabled:  # if not enabled do not need to put it in granted input (just logging)
+            if item.fuzzer_name != "INITIAL":  # if not initial corpus add it
+                self.granted_queue.put(item)
+
     @staticmethod
     def mk_rpl_status(status: str) -> str:
         if status == "SUCCESS":
             return mk_color(status, Bcolors.OKGREEN)
         else:
             return mk_color(status, Bcolors.FAIL)
```

### Comparing `pastis-framework-1.0.6/pastisbroker/stat_manager.py` & `pastis-framework-1.0.7/pastisbroker/stat_manager.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbroker/utils.py` & `pastis-framework-1.0.7/pastisbroker/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/pastisbroker/workspace.py` & `pastis-framework-1.0.7/pastisbroker/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.6/setup.py` & `pastis-framework-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md") as f:
     lines = f.readlines()
     README = "\n".join(lines[4:7]+lines[51:])
 
 
 setup(
     name="pastis-framework",
-    version="1.0.6",
+    version="1.0.7",
     description="PASTIS framework for collaborative fuzzing",
     long_description=README,
     long_description_content_type='text/markdown',
     packages=[
         "libpastis",
         "libpastis.proto",
         "pastisbroker",
```

