# Comparing `tmp/hypergo-0.1.8.tar.gz` & `tmp/hypergo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.8.tar", last modified: Thu Aug  3 02:44:56 2023, max compression
+gzip compressed data, was "hypergo-0.1.9.tar", last modified: Fri Aug  4 14:34:53 2023, max compression
```

## Comparing `hypergo-0.1.8.tar` & `hypergo-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.534507 hypergo-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.514506 hypergo-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.522507 hypergo-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 02:44:43.000000 hypergo-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-03 02:44:43.000000 hypergo-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 02:44:43.000000 hypergo-0.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-03 02:44:43.000000 hypergo-0.1.8/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:43.000000 hypergo-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 02:44:56.534507 hypergo-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 02:44:43.000000 hypergo-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-03 02:44:43.000000 hypergo-0.1.8/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 02:44:43.000000 hypergo-0.1.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.530507 hypergo-0.1.8/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-03 02:44:43.000000 hypergo-0.1.8/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.530507 hypergo-0.1.8/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 02:44:56.000000 hypergo-0.1.8/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-03 02:44:43.000000 hypergo-0.1.8/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 02:44:43.000000 hypergo-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 02:44:56.534507 hypergo-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-03 02:44:43.000000 hypergo-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:44:56.534507 hypergo-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-03 02:44:43.000000 hypergo-0.1.8/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.768368 hypergo-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.760368 hypergo-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.764368 hypergo-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 14:34:43.000000 hypergo-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-04 14:34:43.000000 hypergo-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 14:34:43.000000 hypergo-0.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-04 14:34:43.000000 hypergo-0.1.9/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:43.000000 hypergo-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 14:34:53.768368 hypergo-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-04 14:34:43.000000 hypergo-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-04 14:34:43.000000 hypergo-0.1.9/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-04 14:34:43.000000 hypergo-0.1.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.764368 hypergo-0.1.9/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-04 14:34:43.000000 hypergo-0.1.9/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.764368 hypergo-0.1.9/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 14:34:53.000000 hypergo-0.1.9/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-04 14:34:43.000000 hypergo-0.1.9/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 14:34:43.000000 hypergo-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 14:34:53.768368 hypergo-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-04 14:34:43.000000 hypergo-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:53.768368 hypergo-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-04 14:34:43.000000 hypergo-0.1.9/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.8/.github/workflows/python-publish.yml` & `hypergo-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/.gitignore` & `hypergo-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/BACKLOG.md` & `hypergo-0.1.9/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/RELEASE_NOTES.md` & `hypergo-0.1.9/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.9/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/config.py` & `hypergo-0.1.9/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/executor.py` & `hypergo-0.1.9/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/graph.py` & `hypergo-0.1.9/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/hypergo_cli.py` & `hypergo-0.1.9/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/hypergo_click.py` & `hypergo-0.1.9/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/hypergo_cmd.py` & `hypergo-0.1.9/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/local_storage.py` & `hypergo-0.1.9/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/message.py` & `hypergo-0.1.9/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/service_bus_connection.py` & `hypergo-0.1.9/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/stdio_connection.py` & `hypergo-0.1.9/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/storage.py` & `hypergo-0.1.9/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/transform.py` & `hypergo-0.1.9/hypergo/transform.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/utility.py` & `hypergo-0.1.9/hypergo/utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo/version.py` & `hypergo-0.1.9/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.9/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/lint.sh` & `hypergo-0.1.9/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/setup.py` & `hypergo-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test.json` & `hypergo-0.1.9/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test.yaml` & `hypergo-0.1.9/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.9/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_dynamic_routing_key.py` & `hypergo-0.1.9/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_local_storage.py` & `hypergo-0.1.9/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_message.py` & `hypergo-0.1.9/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_storage.py` & `hypergo-0.1.9/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_utility.py` & `hypergo-0.1.9/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.8/tests/test_utility_serialization.py` & `hypergo-0.1.9/tests/test_utility_serialization.py`

 * *Files identical despite different names*

