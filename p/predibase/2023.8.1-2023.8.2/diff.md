# Comparing `tmp/predibase-2023.8.1.tar.gz` & `tmp/predibase-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-2023.8.1.tar", last modified: Thu Aug  3 01:12:09 2023, max compression
+gzip compressed data, was "predibase-2023.8.2.tar", last modified: Thu Aug  3 23:28:27 2023, max compression
```

## Comparing `predibase-2023.8.1.tar` & `predibase-2023.8.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 01:11:12.000000 predibase-2023.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 01:12:09.871128 predibase-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-03 01:11:12.000000 predibase-2023.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.855128 predibase-2023.8.1/predibase/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.863128 predibase-2023.8.1/predibase/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/connection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/deployment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/engine_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/llm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/permission_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.863128 predibase-2023.8.1/predibase/pql/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/query_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/triton_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.859128 predibase-2023.8.1/predibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 01:12:09.000000 predibase-2023.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 01:11:12.000000 predibase-2023.8.1/requirements_predictor.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:12:09.871128 predibase-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-03 01:11:12.000000 predibase-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 23:27:19.000000 predibase-2023.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 23:28:27.446507 predibase-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-03 23:27:19.000000 predibase-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.442507 predibase-2023.8.2/predibase/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/resource_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/triton_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 23:28:27.000000 predibase-2023.8.2/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:27.446507 predibase-2023.8.2/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.000000 predibase-2023.8.2/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 23:28:27.000000 predibase-2023.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 23:27:19.000000 predibase-2023.8.2/requirements_predictor.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:28:27.446507 predibase-2023.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-03 23:27:19.000000 predibase-2023.8.2/setup.py
```

### Comparing `predibase-2023.8.1/predibase/cli.py` & `predibase-2023.8.2/predibase/cli.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/create.py` & `predibase-2023.8.2/predibase/cli_commands/create.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/delete.py` & `predibase-2023.8.2/predibase/cli_commands/delete.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/deploy.py` & `predibase-2023.8.2/predibase/cli_commands/deploy.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/list.py` & `predibase-2023.8.2/predibase/cli_commands/list.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/prompt.py` & `predibase-2023.8.2/predibase/cli_commands/prompt.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/settings.py` & `predibase-2023.8.2/predibase/cli_commands/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/cli_commands/utils.py` & `predibase-2023.8.2/predibase/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/client.py` & `predibase-2023.8.2/predibase/client.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/connection.py` & `predibase-2023.8.2/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/connection_mixin.py` & `predibase-2023.8.2/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/dataset_mixin.py` & `predibase-2023.8.2/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/deployment_mixin.py` & `predibase-2023.8.2/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/engine_mixin.py` & `predibase-2023.8.2/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/llm_mixin.py` & `predibase-2023.8.2/predibase/llm_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/model_mixin.py` & `predibase-2023.8.2/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/permission_mixin.py` & `predibase-2023.8.2/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/pql/__init__.py` & `predibase-2023.8.2/predibase/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/pql/adapter.py` & `predibase-2023.8.2/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/pql/api.py` & `predibase-2023.8.2/predibase/pql/api.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/pql/utils.py` & `predibase-2023.8.2/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/predictor.py` & `predibase-2023.8.2/predibase/predictor.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/query_mixin.py` & `predibase-2023.8.2/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/config.py` & `predibase-2023.8.2/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/connection.py` & `predibase-2023.8.2/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/connection_object.py` & `predibase-2023.8.2/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/connection_properties.py` & `predibase-2023.8.2/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/dataset.py` & `predibase-2023.8.2/predibase/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/dataset_info.py` & `predibase-2023.8.2/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/deployment.py` & `predibase-2023.8.2/predibase/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/engine.py` & `predibase-2023.8.2/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/llm.py` & `predibase-2023.8.2/predibase/resource/llm.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/model.py` & `predibase-2023.8.2/predibase/resource/model.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/query.py` & `predibase-2023.8.2/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource/user.py` & `predibase-2023.8.2/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/resource_util.py` & `predibase-2023.8.2/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/triton_util.py` & `predibase-2023.8.2/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase/util.py` & `predibase-2023.8.2/predibase/util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase.egg-info/SOURCES.txt` & `predibase-2023.8.2/predibase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase_notebook/__init__.py` & `predibase-2023.8.2/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/predibase_notebook/env.py` & `predibase-2023.8.2/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.8.1/setup.py` & `predibase-2023.8.2/setup.py`

 * *Files identical despite different names*

