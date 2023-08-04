# Comparing `tmp/pympipool-0.6.1.tar.gz` & `tmp/pympipool-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.6.1.tar", last modified: Mon Jul 31 01:02:59 2023, max compression
+gzip compressed data, was "pympipool-0.6.2.tar", last modified: Fri Aug  4 19:50:47 2023, max compression
```

## Comparing `pympipool-0.6.1.tar` & `pympipool-0.6.2.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-31 01:02:53.000000 pympipool-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 01:02:53.000000 pympipool-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-31 01:02:59.159087 pympipool-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-31 01:02:53.000000 pympipool-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/backend/mpiexec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/fluxbroker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/taskbroker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/taskexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/backend/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/taskexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 01:02:59.159087 pympipool-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-31 01:02:58.000000 pympipool-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_parse_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-31 01:02:53.000000 pympipool-0.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.484195 pympipool-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-04 19:50:43.000000 pympipool-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 19:50:43.000000 pympipool-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-04 19:50:47.484195 pympipool-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-08-04 19:50:43.000000 pympipool-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.484195 pympipool-0.6.2/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-04 19:50:47.484195 pympipool-0.6.2/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/backend/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/backend/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/interfaces/fluxbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/interfaces/taskbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/interfaces/taskexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/legacy/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/backend/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/legacy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/interfaces/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool/legacy/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/legacy/shared/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.480195 pympipool-0.6.2/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/taskexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-04 19:50:43.000000 pympipool-0.6.2/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.476195 pympipool-0.6.2/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-04 19:50:47.000000 pympipool-0.6.2/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-04 19:50:47.000000 pympipool-0.6.2/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:50:47.000000 pympipool-0.6.2/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 19:50:47.000000 pympipool-0.6.2/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 19:50:47.000000 pympipool-0.6.2/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 19:50:47.484195 pympipool-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-04 19:50:47.000000 pympipool-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:50:47.484195 pympipool-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_parse_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-04 19:50:43.000000 pympipool-0.6.2/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-04 19:50:43.000000 pympipool-0.6.2/versioneer.py
```

### Comparing `pympipool-0.6.1/LICENSE` & `pympipool-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/PKG-INFO` & `pympipool-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.6.1
+Version: 0.6.2
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.6.1/README.md` & `pympipool-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool/__init__.py` & `pympipool-0.6.2/pympipool/__init__.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool/backend/mpiexec.py` & `pympipool-0.6.2/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool/interfaces/base.py` & `pympipool-0.6.2/pympipool/shared/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 
 class ExecutorBase(FutureExecutor):
     def __init__(self):
         self._future_queue = queue.Queue()
         self._process = None
 
+    @property
+    def future_queue(self):
+        return self._future_queue
+
     def submit(self, fn, *args, **kwargs):
         """Submits a callable to be executed with the given arguments.
 
         Schedules the callable to be executed as fn(*args, **kwargs) and returns
         a Future instance representing the execution of the callable.
 
         Returns:
```

### Comparing `pympipool-0.6.1/pympipool/interfaces/taskbroker.py` & `pympipool-0.6.2/pympipool/shared/broker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,93 @@
-from pympipool.interfaces.base import ExecutorBase
-from pympipool.shared.thread import RaisingThread
-from pympipool.shared.broker import executor_broker
-
-
-class HPCExecutor(ExecutorBase):
-    def __init__(
-        self,
-        max_workers,
-        cores_per_worker=1,
-        gpus_per_worker=0,
-        oversubscribe=False,
-        enable_flux_backend=False,
-        enable_slurm_backend=False,
-        init_function=None,
-        cwd=None,
-        sleep_interval=0.1,
-        queue_adapter=None,
-        queue_adapter_kwargs=None,
-    ):
-        super().__init__()
-        self._process = RaisingThread(
-            target=executor_broker,
-            kwargs={
-                "future_queue": self._future_queue,
-                "max_workers": max_workers,
-                "cores_per_worker": cores_per_worker,
-                "gpus_per_worker": gpus_per_worker,
-                "oversubscribe": oversubscribe,
-                "enable_flux_backend": enable_flux_backend,
-                "enable_slurm_backend": enable_slurm_backend,
-                "init_function": init_function,
-                "cwd": cwd,
-                "sleep_interval": sleep_interval,
-                "queue_adapter": queue_adapter,
-                "queue_adapter_kwargs": queue_adapter_kwargs,
-            },
+from concurrent.futures import as_completed, Future
+import queue
+from time import sleep
+
+from pympipool.interfaces.taskexecutor import Executor
+
+
+def executor_broker(
+    future_queue,
+    max_workers,
+    cores_per_worker=1,
+    gpus_per_worker=0,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    init_function=None,
+    cwd=None,
+    sleep_interval=0.1,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
+):
+    meta_future_lst = _get_executor_list(
+        max_workers=max_workers,
+        cores_per_worker=cores_per_worker,
+        gpus_per_worker=gpus_per_worker,
+        oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        init_function=init_function,
+        cwd=cwd,
+        queue_adapter=queue_adapter,
+        queue_adapter_kwargs=queue_adapter_kwargs,
+    )
+    while True:
+        try:
+            task_dict = future_queue.get_nowait()
+        except queue.Empty:
+            sleep(sleep_interval)
+        else:
+            if execute_task_dict(task_dict=task_dict, meta_future_lst=meta_future_lst):
+                future_queue.task_done()
+            else:
+                future_queue.task_done()
+                break
+
+
+def execute_task_dict(task_dict, meta_future_lst):
+    if "fn" in task_dict.keys():
+        meta_future = next(as_completed(meta_future_lst.keys()))
+        executor = meta_future_lst.pop(meta_future)
+        executor.future_queue.put(task_dict)
+        meta_future_lst[task_dict["future"]] = executor
+        return True
+    elif "shutdown" in task_dict.keys() and task_dict["shutdown"]:
+        for executor in meta_future_lst.values():
+            executor.shutdown(wait=task_dict["wait"])
+        return False
+    else:
+        raise ValueError("Unrecognized Task in task_dict: ", task_dict)
+
+
+def _get_executor_list(
+    max_workers,
+    cores_per_worker=1,
+    gpus_per_worker=0,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    init_function=None,
+    cwd=None,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
+):
+    return {
+        get_future_done(): Executor(
+            cores=cores_per_worker,
+            gpus_per_task=int(gpus_per_worker / cores_per_worker),
+            oversubscribe=oversubscribe,
+            enable_flux_backend=enable_flux_backend,
+            enable_slurm_backend=enable_slurm_backend,
+            init_function=init_function,
+            cwd=cwd,
+            queue_adapter=queue_adapter,
+            queue_adapter_kwargs=queue_adapter_kwargs,
         )
-        self._process.start()
+        for _ in range(max_workers)
+    }
+
+
+def get_future_done():
+    f = Future()
+    f.set_result(True)
+    return f
```

### Comparing `pympipool-0.6.1/pympipool/interfaces/taskexecutor.py` & `pympipool-0.6.2/pympipool/interfaces/taskexecutor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pympipool.interfaces.base import ExecutorBase
+from pympipool.shared.base import ExecutorBase
 from pympipool.shared.thread import RaisingThread
 from pympipool.shared.taskexecutor import (
     execute_parallel_tasks,
     cloudpickle_register,
 )
 
 
@@ -21,33 +21,32 @@
         enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
         init_function (None): optional function to preset arguments for functions which are submitted later
         cwd (str/None): current working directory where the parallel python task is executed
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
-    Simple example:
+    Examples:
         ```
-        import numpy as np
-        from pympipool import Executor
-
-        def calc(i, j, k):
-            from mpi4py import MPI
-            size = MPI.COMM_WORLD.Get_size()
-            rank = MPI.COMM_WORLD.Get_rank()
-            return np.array([i, j, k]), size, rank
-
-        def init_k():
-            return {"k": 3}
-
-        with Executor(cores=2, init_function=init_k) as p:
-            fs = p.submit(calc, 2, j=4)
-            print(fs.result())
-
-        >>> [(array([2, 4, 3]), 2, 0), (array([2, 4, 3]), 2, 1)]
+        >>> import numpy as np
+        >>> from pympipool import Executor
+        >>>
+        >>> def calc(i, j, k):
+        >>>     from mpi4py import MPI
+        >>>     size = MPI.COMM_WORLD.Get_size()
+        >>>     rank = MPI.COMM_WORLD.Get_rank()
+        >>>     return np.array([i, j, k]), size, rank
+        >>>
+        >>> def init_k():
+        >>>     return {"k": 3}
+        >>>
+        >>> with Executor(cores=2, init_function=init_k) as p:
+        >>>     fs = p.submit(calc, 2, j=4)
+        >>>     print(fs.result())
+        [(array([2, 4, 3]), 2, 0), (array([2, 4, 3]), 2, 1)]
         ```
     """
 
     def __init__(
         self,
         cores,
         gpus_per_task=0,
```

### Comparing `pympipool-0.6.1/pympipool/legacy/backend/mpipool.py` & `pympipool-0.6.2/pympipool/legacy/backend/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool/legacy/interfaces/executor.py` & `pympipool-0.6.2/pympipool/legacy/interfaces/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pympipool.interfaces.base import ExecutorBase
+from pympipool.shared.base import ExecutorBase
 from pympipool.shared.thread import RaisingThread
 from pympipool.legacy.shared.interface import execute_serial_tasks
 from pympipool.shared.taskexecutor import cloudpickle_register
 
 
 class PoolExecutor(ExecutorBase):
     """
@@ -20,27 +20,27 @@
         enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
         cwd (str/None): current working directory where the parallel python task is executed
         sleep_interval (float):
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
-    Simple example:
+    Examples:
         ```
-        from pympipool import PoolExecutor
-
-        def calc(i, j):
-            return i + j
-
-        with PoolExecutor(max_workers=2) as p:
-            fs1 = p.submit(calc, 1, 2)
-            fs2 = p.submit(calc, 3, 4)
-            fs3 = p.submit(calc, 5, 6)
-            fs4 = p.submit(calc, 7, 8)
-            print(fs1.result(), fs2.result(), fs3.result(), fs4.result()
+        >>> from pympipool import PoolExecutor
+        >>>
+        >>> def calc(i, j):
+        >>>     return i + j
+        >>>
+        >>> with PoolExecutor(max_workers=2) as p:
+        >>>     fs1 = p.submit(calc, 1, 2)
+        >>>     fs2 = p.submit(calc, 3, 4)
+        >>>     fs3 = p.submit(calc, 5, 6)
+        >>>     fs4 = p.submit(calc, 7, 8)
+        >>>     print(fs1.result(), fs2.result(), fs3.result(), fs4.result()
         ```
     """
 
     def __init__(
         self,
         max_workers=1,
         gpus_per_task=0,
```

### Comparing `pympipool-0.6.1/pympipool/legacy/interfaces/pool.py` & `pympipool-0.6.2/pympipool/legacy/interfaces/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,24 @@
         oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only)
         enable_flux_backend (bool): use the flux-framework as backend
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
         cwd (str/None): current working directory where the parallel python task is executed
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
-    Simple example:
+    Examples:
         ```
-        import numpy as np
-        from pympipool import Pool
-
-        def calc(i):
-            return np.array(i ** 2)
-
-        with Pool(cores=2) as p:
-            print(p.map(func=calc, iterable=[1, 2, 3, 4]))
+        >>> import numpy as np
+        >>> from pympipool import Pool
+        >>>
+        >>> def calc(i):
+        >>>     return np.array(i ** 2)
+        >>>
+        >>> with Pool(cores=2) as p:
+        >>>     print(p.map(func=calc, iterable=[1, 2, 3, 4]))
         ```
     """
 
     def __init__(
         self,
         max_workers=1,
         gpus_per_task=0,
```

### Comparing `pympipool-0.6.1/pympipool/legacy/shared/backend.py` & `pympipool-0.6.2/pympipool/legacy/shared/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tqdm import tqdm
 
-from pympipool.shared.backend import call_funct, _update_default_dict_from_arguments
+from pympipool.shared.backend import call_funct, update_default_dict_from_arguments
 
 
 def map_funct(executor, funct, lst, chunksize=1, cores_per_task=1, map_flag=True):
     if cores_per_task == 1:
         if map_flag:
             results = executor.map(funct, lst, chunksize=chunksize)
         else:
@@ -38,15 +38,15 @@
 
     Args:
         argument_lst (list): list of arguments as strings
 
     Returns:
         dict: dictionary with the parsed arguments and their corresponding values
     """
-    return _update_default_dict_from_arguments(
+    return update_default_dict_from_arguments(
         argument_lst=argument_lst,
         argument_dict={
             "total_cores": "--cores-total",
             "zmqport": "--zmqport",
             "cores_per_task": "--cores-per-task",
             "host": "--host",
         },
```

### Comparing `pympipool-0.6.1/pympipool/legacy/shared/interface.py` & `pympipool-0.6.2/pympipool/legacy/shared/interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool/shared/backend.py` & `pympipool-0.6.2/pympipool/shared/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,25 @@
 
     Args:
         argument_lst (list): list of arguments as strings
 
     Returns:
         dict: dictionary with the parsed arguments and their corresponding values
     """
-    return _update_default_dict_from_arguments(
+    return update_default_dict_from_arguments(
         argument_lst=argument_lst,
         argument_dict={
             "zmqport": "--zmqport",
             "host": "--host",
         },
         default_dict={"host": "localhost"},
     )
 
 
-def _update_default_dict_from_arguments(argument_lst, argument_dict, default_dict):
+def update_default_dict_from_arguments(argument_lst, argument_dict, default_dict):
     default_dict.update(
         {
             k: argument_lst[argument_lst.index(v) + 1]
             for k, v in argument_dict.items()
             if v in argument_lst
         }
     )
```

### Comparing `pympipool-0.6.1/pympipool/shared/broker.py` & `pympipool-0.6.2/tests/test_connection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,100 @@
-from concurrent.futures import as_completed, Future
-import queue
-from time import sleep
-
-from pympipool.interfaces.taskexecutor import Executor
-
-
-class MetaExecutorFuture(object):
-    def __init__(self, future, executor):
-        self.future = future
-        self.executor = executor
-
-    @property
-    def _condition(self):
-        return self.future._condition
-
-    @property
-    def _state(self):
-        return self.future._state
-
-    @property
-    def _waiters(self):
-        return self.future._waiters
-
-    def done(self):
-        return self.future.done()
-
-    def submit(self, task_dict):
-        self.future = task_dict["future"]
-        self.executor._future_queue.put(task_dict)
-
-
-def executor_broker(
-    future_queue,
-    max_workers,
-    cores_per_worker=1,
-    gpus_per_worker=0,
-    oversubscribe=False,
-    enable_flux_backend=False,
-    enable_slurm_backend=False,
-    init_function=None,
-    cwd=None,
-    sleep_interval=0.1,
-    queue_adapter=None,
-    queue_adapter_kwargs=None,
-):
-    meta_future_lst = _get_executor_list(
-        max_workers=max_workers,
-        cores_per_worker=cores_per_worker,
-        gpus_per_worker=gpus_per_worker,
-        oversubscribe=oversubscribe,
-        enable_flux_backend=enable_flux_backend,
-        enable_slurm_backend=enable_slurm_backend,
-        init_function=init_function,
-        cwd=cwd,
-        queue_adapter=queue_adapter,
-        queue_adapter_kwargs=queue_adapter_kwargs,
-    )
-    while True:
-        try:
-            task_dict = future_queue.get_nowait()
-        except queue.Empty:
-            sleep(sleep_interval)
-        else:
-            if _execute_task_dict(task_dict=task_dict, meta_future_lst=meta_future_lst):
-                future_queue.task_done()
-            else:
-                future_queue.task_done()
-                break
-
-
-def _execute_task_dict(task_dict, meta_future_lst):
-    if "fn" in task_dict.keys():
-        meta_future = next(as_completed(meta_future_lst))
-        meta_future.submit(task_dict=task_dict)
-        return True
-    elif "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-        for meta in meta_future_lst:
-            meta.executor.shutdown(wait=task_dict["wait"])
-        return False
-    else:
-        raise ValueError("Unrecognized Task in task_dict: ", task_dict)
-
-
-def _get_executor_list(
-    max_workers,
-    cores_per_worker=1,
-    gpus_per_worker=0,
-    oversubscribe=False,
-    enable_flux_backend=False,
-    enable_slurm_backend=False,
-    init_function=None,
-    cwd=None,
-    queue_adapter=None,
-    queue_adapter_kwargs=None,
-):
-    return [
-        MetaExecutorFuture(
-            future=_get_future_done(),
-            executor=Executor(
-                cores=cores_per_worker,
-                gpus_per_task=int(gpus_per_worker / cores_per_worker),
-                oversubscribe=oversubscribe,
-                enable_flux_backend=enable_flux_backend,
-                enable_slurm_backend=enable_slurm_backend,
-                init_function=init_function,
-                cwd=cwd,
-                queue_adapter=queue_adapter,
-                queue_adapter_kwargs=queue_adapter_kwargs,
-            ),
-        )
-        for _ in range(max_workers)
-    ]
-
-
-def _get_future_done():
-    f = Future()
-    f.set_result(True)
-    return f
+import os
+import unittest
+from pympipool.shared.connections import (
+    BaseInterface,
+    MpiExecInterface,
+    SlurmSubprocessInterface,
+    PysqaInterface,
+    FluxCmdInterface,
+    get_connection_interface
+)
+
+
+class Interface(BaseInterface):
+    def __init__(self, cwd, cores=1, gpus_per_core=0, oversubscribe=False):
+        super().__init__(
+            cwd=cwd,
+            cores=cores,
+            gpus_per_core=gpus_per_core,
+            oversubscribe=oversubscribe,
+        )
+
+
+class TestExecutor(unittest.TestCase):
+    def setUp(self):
+        self.interface = Interface(
+            cwd=None,
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False
+        )
+
+    def test_bootup(self):
+        with self.assertRaises(NotImplementedError):
+            self.interface.bootup(command_lst=[])
+
+    def test_shutdown(self):
+        with self.assertRaises(NotImplementedError):
+            self.interface.shutdown(wait=True)
+
+    def test_poll(self):
+        with self.assertRaises(NotImplementedError):
+            self.interface.poll()
+
+
+class TestInterfaceConnection(unittest.TestCase):
+    def test_mpiexec(self):
+        interface = get_connection_interface(
+            cwd=None,
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False,
+            enable_flux_backend=False,
+            enable_slurm_backend=False,
+            queue_adapter=None,
+            queue_type=None,
+            queue_adapter_kwargs=None,
+        )
+        self.assertIsInstance(interface, MpiExecInterface)
+
+    def test_slurm(self):
+        interface = get_connection_interface(
+            cwd=None,
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False,
+            enable_flux_backend=False,
+            enable_slurm_backend=True,
+            queue_adapter=None,
+            queue_type=None,
+            queue_adapter_kwargs=None,
+        )
+        self.assertIsInstance(interface, SlurmSubprocessInterface)
+
+    def test_pysqa(self):
+        interface = get_connection_interface(
+            cwd=None,
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False,
+            enable_flux_backend=False,
+            enable_slurm_backend=False,
+            queue_adapter=True,
+            queue_type=None,
+            queue_adapter_kwargs=None,
+        )
+        self.assertIsInstance(interface, PysqaInterface)
+
+    def test_flux_cmd(self):
+        interface = get_connection_interface(
+            cwd=None,
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False,
+            enable_flux_backend=True,
+            enable_slurm_backend=False,
+            queue_adapter=None,
+            queue_type=None,
+            queue_adapter_kwargs=None,
+        )
+        self.assertIsInstance(interface, FluxCmdInterface)
```

### Comparing `pympipool-0.6.1/pympipool/shared/communication.py` & `pympipool-0.6.2/pympipool/shared/communication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cloudpickle
-import socket
+from socket import gethostname
 import zmq
 
 from pympipool.shared.connections import get_connection_interface
 
 
 class SocketInterface(object):
     """
@@ -107,15 +107,15 @@
     queue_adapter=None,
     queue_type=None,
     queue_adapter_kwargs=None,
 ):
     if enable_flux_backend or enable_slurm_backend or queue_adapter is not None:
         command_lst += [
             "--host",
-            socket.gethostname(),
+            gethostname(),
         ]
     connections = get_connection_interface(
         cwd=cwd,
         cores=cores,
         gpus_per_core=gpus_per_core,
         oversubscribe=oversubscribe,
         enable_flux_backend=enable_flux_backend,
```

### Comparing `pympipool-0.6.1/pympipool/shared/connections.py` & `pympipool-0.6.2/pympipool/shared/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from abc import ABC
 import os
 import subprocess
 
 
 class BaseInterface(ABC):
-    def __init__(self, cwd, cores=1, gpus_per_core=0, oversubscribe=False):
+    def __init__(
+        self, cwd, cores=1, threads_per_core=1, gpus_per_core=0, oversubscribe=False
+    ):
         self._cwd = cwd
         self._cores = cores
+        self._threads_per_core = threads_per_core
         self._gpus_per_core = gpus_per_core
         self._oversubscribe = oversubscribe
 
     def bootup(self, command_lst):
         raise NotImplementedError
 
     def shutdown(self, wait=True):
         raise NotImplementedError
 
     def poll(self):
         raise NotImplementedError
 
 
 class SubprocessInterface(BaseInterface):
-    def __init__(self, cwd=None, cores=1, gpus_per_core=0, oversubscribe=False):
+    def __init__(
+        self,
+        cwd=None,
+        cores=1,
+        threads_per_core=1,
+        gpus_per_core=0,
+        oversubscribe=False,
+    ):
         super().__init__(
             cwd=cwd,
             cores=cores,
+            threads_per_core=threads_per_core,
             gpus_per_core=gpus_per_core,
             oversubscribe=oversubscribe,
         )
         self._process = None
 
     def bootup(self, command_lst):
         self._process = subprocess.Popen(
@@ -68,14 +79,15 @@
 
 
 class SlurmSubprocessInterface(SubprocessInterface):
     def generate_command(self, command_lst):
         command_prepend_lst = generate_slurm_command(
             cores=self._cores,
             cwd=self._cwd,
+            threads_per_core=self._threads_per_core,
             gpus_per_core=self._gpus_per_core,
             oversubscribe=self._oversubscribe,
         )
         return super().generate_command(
             command_lst=command_prepend_lst + command_lst,
         )
 
@@ -138,29 +150,38 @@
             "-n",
             str(self._cores),
         ]
         if self._cwd is not None:
             command_prepend_lst += [
                 "--cwd=" + self._cwd,
             ]
+        if self._threads_per_core > 1:
+            command_prepend_lst += ["--cores-per-task=" + str(self._threads_per_core)]
         if self._gpus_per_core > 0:
             command_prepend_lst += ["--gpus-per-task=" + str(self._gpus_per_core)]
         return super().generate_command(
             command_lst=command_prepend_lst + command_lst,
         )
 
 
 class FluxPythonInterface(BaseInterface):
     def __init__(
-        self, cwd=None, cores=1, gpus_per_core=0, oversubscribe=False, executor=None
+        self,
+        cwd=None,
+        cores=1,
+        threads_per_core=1,
+        gpus_per_core=0,
+        oversubscribe=False,
+        executor=None,
     ):
         super().__init__(
             cwd=cwd,
             cores=cores,
             gpus_per_core=gpus_per_core,
+            threads_per_core=threads_per_core,
             oversubscribe=oversubscribe,
         )
         self._executor = executor
         self._future = None
 
     def bootup(self, command_lst):
         import flux.job
@@ -170,15 +191,15 @@
                 "Oversubscribing is currently not supported for the Flux adapter."
             )
         if self._executor is None:
             self._executor = flux.job.FluxExecutor()
         jobspec = flux.job.JobspecV1.from_command(
             command=command_lst,
             num_tasks=self._cores,
-            cores_per_task=1,
+            cores_per_task=self._threads_per_core,
             gpus_per_task=self._gpus_per_core,
             num_nodes=None,
             exclusive=False,
         )
         jobspec.environment = dict(os.environ)
         if self._cwd is not None:
             jobspec.cwd = self._cwd
@@ -192,16 +213,20 @@
         # so we wait until the execution is completed.
         self._future.result()
 
     def poll(self):
         return self._future is not None and not self._future.done()
 
 
-def generate_slurm_command(cores, cwd, gpus_per_core=0, oversubscribe=False):
+def generate_slurm_command(
+    cores, cwd, threads_per_core=1, gpus_per_core=0, oversubscribe=False
+):
     command_prepend_lst = ["srun", "-n", str(cores), "-D", cwd]
+    if threads_per_core > 1:
+        command_prepend_lst += ["--cpus-per-task" + str(threads_per_core)]
     if gpus_per_core > 0:
         command_prepend_lst += ["--gpus-per-task=" + str(gpus_per_core)]
     if oversubscribe:
         command_prepend_lst += ["--oversubscribe"]
     return command_prepend_lst
```

### Comparing `pympipool-0.6.1/pympipool/shared/taskexecutor.py` & `pympipool-0.6.2/pympipool/shared/taskexecutor.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     1 refers to 1 level higher than the map function
 
     Args:
         ind (int): index of the level at which pickle by value starts while for the rest pickle by reference is used
     """
     try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
         cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
+    except IndexError:
+        cloudpickle_register(ind=ind - 1)
     except ValueError:
         pass
 
 
 def execute_parallel_tasks(
     future_queue,
     cores,
@@ -82,18 +84,18 @@
         gpus_per_core=gpus_per_task,
         oversubscribe=oversubscribe,
         enable_flux_backend=enable_flux_backend,
         enable_slurm_backend=enable_slurm_backend,
         queue_adapter=queue_adapter,
         queue_adapter_kwargs=queue_adapter_kwargs,
     )
-    _execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
+    execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
 
 
-def _execute_parallel_tasks_loop(interface, future_queue):
+def execute_parallel_tasks_loop(interface, future_queue):
     while True:
         task_dict = future_queue.get()
         if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
             interface.shutdown(wait=task_dict["wait"])
             future_queue.task_done()
             break
         elif "fn" in task_dict.keys() and "future" in task_dict.keys():
```

### Comparing `pympipool-0.6.1/pympipool/shared/thread.py` & `pympipool-0.6.2/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/pympipool.egg-info/PKG-INFO` & `pympipool-0.6.2/pympipool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.6.1
+Version: 0.6.2
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.6.1/pympipool.egg-info/SOURCES.txt` & `pympipool-0.6.2/pympipool.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 pympipool.egg-info/PKG-INFO
 pympipool.egg-info/SOURCES.txt
 pympipool.egg-info/dependency_links.txt
 pympipool.egg-info/requires.txt
 pympipool.egg-info/top_level.txt
 pympipool/backend/__init__.py
 pympipool/backend/mpiexec.py
+pympipool/backend/serial.py
 pympipool/interfaces/__init__.py
-pympipool/interfaces/base.py
 pympipool/interfaces/fluxbroker.py
 pympipool/interfaces/taskbroker.py
 pympipool/interfaces/taskexecutor.py
 pympipool/legacy/__init__.py
 pympipool/legacy/backend/__init__.py
 pympipool/legacy/backend/mpipool.py
 pympipool/legacy/interfaces/__init__.py
 pympipool/legacy/interfaces/executor.py
 pympipool/legacy/interfaces/pool.py
 pympipool/legacy/shared/__init__.py
 pympipool/legacy/shared/backend.py
 pympipool/legacy/shared/interface.py
 pympipool/shared/__init__.py
 pympipool/shared/backend.py
+pympipool/shared/base.py
 pympipool/shared/broker.py
 pympipool/shared/communication.py
 pympipool/shared/connections.py
 pympipool/shared/taskexecutor.py
 pympipool/shared/thread.py
 tests/test_communicator_split.py
 tests/test_connection.py
@@ -42,12 +43,13 @@
 tests/test_interface.py
 tests/test_meta.py
 tests/test_multitask.py
 tests/test_parse.py
 tests/test_parse_legacy.py
 tests/test_pool.py
 tests/test_queue.py
+tests/test_serial.py
 tests/test_task.py
 tests/test_thread.py
 tests/test_worker.py
 tests/test_worker_memory.py
 tests/test_zmq.py
```

### Comparing `pympipool-0.6.1/setup.py` & `pympipool-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_communicator_split.py` & `pympipool-0.6.2/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_executor.py` & `pympipool-0.6.2/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_flux.py` & `pympipool-0.6.2/tests/test_flux.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,23 +35,38 @@
 
 
 @unittest.skipIf(skip_flux_test, "Flux is not installed, so the flux tests are skipped.")
 class TestFlux(unittest.TestCase):
     def setUp(self):
         self.executor = FluxExecutor()
 
-    def test_flux_executor(self):
+    def test_flux_executor_serial(self):
         with PyFluxExecutor(max_workers=2, executor=self.executor) as exe:
             fs_1 = exe.submit(calc, 1)
             fs_2 = exe.submit(calc, 2)
             self.assertEqual(fs_1.result(), 1)
             self.assertEqual(fs_2.result(), 2)
             self.assertTrue(fs_1.done())
             self.assertTrue(fs_2.done())
 
+    def test_flux_executor_threads(self):
+        with PyFluxExecutor(max_workers=1, threads_per_core=2, executor=self.executor) as exe:
+            fs_1 = exe.submit(calc, 1)
+            fs_2 = exe.submit(calc, 2)
+            self.assertEqual(fs_1.result(), 1)
+            self.assertEqual(fs_2.result(), 2)
+            self.assertTrue(fs_1.done())
+            self.assertTrue(fs_2.done())
+
+    def test_flux_executor_parallel(self):
+        with PyFluxExecutor(max_workers=1, cores_per_worker=2, executor=self.executor) as exe:
+            fs_1 = exe.submit(mpi_funct, 1)
+            self.assertEqual(fs_1.result(), [(1, 2, 0), (1, 2, 1)])
+            self.assertTrue(fs_1.done())
+
     def test_single_task(self):
         with SingleTaskExecutor(cores=2, executor=self.executor) as p:
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(list(output), [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]])
 
     def test_execute_task(self):
         f = Future()
@@ -63,14 +78,29 @@
             future_queue=q,
             cores=1,
             executor=self.executor
         )
         self.assertEqual(f.result(), 2)
         q.join()
 
+    def test_execute_task_threads(self):
+        f = Future()
+        q = Queue()
+        q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
+        q.put({"shutdown": True, "wait": True})
+        cloudpickle_register(ind=1)
+        execute_parallel_tasks(
+            future_queue=q,
+            cores=1,
+            threads_per_core=1,
+            executor=self.executor
+        )
+        self.assertEqual(f.result(), 2)
+        q.join()
+
     def test_internal_memory(self):
         with SingleTaskExecutor(cores=1, init_function=set_global, executor=self.executor) as p:
             f = p.submit(get_global)
             self.assertFalse(f.done())
             self.assertEqual(f.result(), np.array([5]))
             self.assertTrue(f.done())
 
@@ -79,7 +109,17 @@
         f = Future()
         q.put({"fn": calc, "args": (1,), "kwargs": {}, "future": f})
         q.put({"shutdown": True, "wait": True})
         executor_broker(future_queue=q, max_workers=1, executor=self.executor)
         self.assertTrue(f.done())
         self.assertEqual(f.result(), 1)
         q.join()
+
+    def test_executor_broker_threads(self):
+        q = Queue()
+        f = Future()
+        q.put({"fn": calc, "args": (1,), "kwargs": {}, "future": f})
+        q.put({"shutdown": True, "wait": True})
+        executor_broker(future_queue=q, max_workers=1, threads_per_core=2, executor=self.executor)
+        self.assertTrue(f.done())
+        self.assertEqual(f.result(), 1)
+        q.join()
```

### Comparing `pympipool-0.6.1/tests/test_future.py` & `pympipool-0.6.2/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_interface.py` & `pympipool-0.6.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_meta.py` & `pympipool-0.6.2/tests/test_meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,97 @@
 from concurrent.futures import as_completed, Future, Executor
 from queue import Queue
 import unittest
 from pympipool.shared.broker import (
     executor_broker,
-    _execute_task_dict,
-    _get_future_done,
+    execute_task_dict,
+    get_future_done,
     _get_executor_list,
 )
 
 from pympipool.interfaces.taskbroker import HPCExecutor
 
 
 def calc(i):
     return i
 
 
+def mpi_funct(i):
+    from mpi4py import MPI
+    size = MPI.COMM_WORLD.Get_size()
+    rank = MPI.COMM_WORLD.Get_rank()
+    return i, size, rank
+
+
 class TestFutureCreation(unittest.TestCase):
     def test_get_future_done(self):
-        f = _get_future_done()
+        f = get_future_done()
         self.assertTrue(isinstance(f, Future))
         self.assertTrue(f.done())
 
 
 class TestMetaExecutorFuture(unittest.TestCase):
     def test_meta_executor_future(self):
-        meta_future = _get_executor_list(max_workers=1)[0]
-        self.assertTrue(isinstance(meta_future.future, Future))
-        self.assertTrue(isinstance(meta_future.executor, Executor))
-        self.assertTrue(meta_future.done())
-        self.assertEqual(meta_future, next(as_completed([meta_future])))
-        meta_future.submit(task_dict={"shutdown": True, "wait": True, "future": _get_future_done()})
+        meta_future = _get_executor_list(max_workers=1)
+        future_obj = list(meta_future.keys())[0]
+        executor_obj = list(meta_future.values())[0]
+        self.assertTrue(isinstance(future_obj, Future))
+        self.assertTrue(isinstance(executor_obj, Executor))
+        self.assertTrue(future_obj.done())
+        self.assertEqual(future_obj, next(as_completed(meta_future.keys())))
+        executor_obj.shutdown(wait=True)
 
     def test_execute_task_dict(self):
         meta_future_lst = _get_executor_list(max_workers=1)
         f = Future()
-        self.assertTrue(_execute_task_dict(
+        self.assertTrue(execute_task_dict(
             task_dict={"fn": calc, "args": (1,), "kwargs": {}, "future": f},
             meta_future_lst=meta_future_lst
         ))
         self.assertEqual(f.result(), 1)
         self.assertTrue(f.done())
-        self.assertFalse(_execute_task_dict(
+        self.assertFalse(execute_task_dict(
             task_dict={"shutdown": True, "wait": True},
             meta_future_lst=meta_future_lst
         ))
 
+    def test_execute_task_dict_error(self):
+        meta_future_lst = _get_executor_list(max_workers=1)
+        with self.assertRaises(ValueError):
+            execute_task_dict(task_dict={}, meta_future_lst=meta_future_lst)
+        list(meta_future_lst.values())[0].shutdown(wait=True)
+
     def test_executor_broker(self):
         q = Queue()
         f = Future()
         q.put({"fn": calc, "args": (1,), "kwargs": {}, "future": f})
         q.put({"shutdown": True, "wait": True})
         executor_broker(future_queue=q, max_workers=1)
         self.assertTrue(f.done())
         self.assertEqual(f.result(), 1)
         q.join()
 
 
 class TestMetaExecutor(unittest.TestCase):
-    def test_meta_executor(self):
+    def test_meta_executor_serial(self):
         with HPCExecutor(max_workers=2) as exe:
             fs_1 = exe.submit(calc, 1)
             fs_2 = exe.submit(calc, 2)
             self.assertEqual(fs_1.result(), 1)
             self.assertEqual(fs_2.result(), 2)
             self.assertTrue(fs_1.done())
             self.assertTrue(fs_2.done())
+
+    def test_meta_executor_single(self):
+        with HPCExecutor(max_workers=1) as exe:
+            fs_1 = exe.submit(calc, 1)
+            fs_2 = exe.submit(calc, 2)
+            self.assertEqual(fs_1.result(), 1)
+            self.assertEqual(fs_2.result(), 2)
+            self.assertTrue(fs_1.done())
+            self.assertTrue(fs_2.done())
+
+    def test_meta_executor_parallel(self):
+        with HPCExecutor(max_workers=1, cores_per_worker=2) as exe:
+            fs_1 = exe.submit(mpi_funct, 1)
+            self.assertEqual(fs_1.result(), [(1, 2, 0), (1, 2, 1)])
+            self.assertTrue(fs_1.done())
```

### Comparing `pympipool-0.6.1/tests/test_multitask.py` & `pympipool-0.6.2/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_parse.py` & `pympipool-0.6.2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_parse_legacy.py` & `pympipool-0.6.2/tests/test_parse_legacy.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_pool.py` & `pympipool-0.6.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_queue.py` & `pympipool-0.6.2/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_task.py` & `pympipool-0.6.2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_worker.py` & `pympipool-0.6.2/tests/test_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,23 @@
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
             self.assertTrue(output.done())
             self.assertEqual(len(p), 0)
         self.assertEqual(output.result(), np.array(4))
 
+    def test_executor_multi_submission(self):
+        with Executor(cores=1) as p:
+            fs_1 = p.submit(calc, i=2)
+            fs_2 = p.submit(calc, i=2)
+            self.assertEqual(fs_1.result(), np.array(4))
+            self.assertEqual(fs_2.result(), np.array(4))
+            self.assertTrue(fs_1.done())
+            self.assertTrue(fs_2.done())
+
     def test_shutdown(self):
         p = Executor(cores=1)
         fs1 = p.submit(sleep_one, i=2)
         fs2 = p.submit(sleep_one, i=4)
         sleep(1)
         p.shutdown(wait=True, cancel_futures=True)
         self.assertTrue(fs1.done())
```

### Comparing `pympipool-0.6.1/tests/test_worker_memory.py` & `pympipool-0.6.2/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/tests/test_zmq.py` & `pympipool-0.6.2/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.1/versioneer.py` & `pympipool-0.6.2/versioneer.py`

 * *Files identical despite different names*

