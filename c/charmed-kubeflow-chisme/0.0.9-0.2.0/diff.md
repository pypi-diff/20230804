# Comparing `tmp/charmed-kubeflow-chisme-0.0.9.tar.gz` & `tmp/charmed-kubeflow-chisme-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmed-kubeflow-chisme-0.0.9.tar", last modified: Fri Apr 21 13:09:27 2023, max compression
+gzip compressed data, was "charmed-kubeflow-chisme-0.2.0.tar", last modified: Thu Aug  3 22:17:02 2023, max compression
```

## Comparing `charmed-kubeflow-chisme-0.0.9.tar` & `charmed-kubeflow-chisme-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,66 @@
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)    11357 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/LICENSE
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2230 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/PKG-INFO
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1737 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/README.md
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1178 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/pyproject.toml
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      741 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/setup.cfg
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.522024 charmed-kubeflow-chisme-0.0.9/src/
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.526024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/__init__.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.530024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      174 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     3620 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/_bundle.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.530024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      446 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      751 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      374 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_kubernetes.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      953 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_with_status.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.534024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      214 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1597 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/_juju.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.534024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      364 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2464 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)    23458 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      855 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/__init__.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      237 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     3946 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_many.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2308 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      761 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/mocking.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      189 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1306 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/_update_layer.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      235 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      863 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      422 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      461 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/_charm_status.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      473 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/_lightkube.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.526024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2230 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/PKG-INFO
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1631 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)        1 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/dependency_links.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)       92 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/requires.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)       24 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.081493 charmed-kubeflow-chisme-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/bundle/_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/charm_reconciler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/component_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/component_graph_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/kubernetes_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/leadership_gate_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/model_name_gate_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/pebble_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/components/serialised_data_interface_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/_with_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/juju/_juju.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24561 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/_many.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/pebble/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/pebble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/pebble/_update_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/rock/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/rock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/rock/_check_rock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/status_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/status_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/status_handling/multistatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/testing/serialized_data_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.089493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/types/_charm_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 22:16:52.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/types/_lightkube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:17:02.085493 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-03 22:17:02.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-03 22:17:02.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:17:02.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 22:17:02.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 22:17:02.000000 charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/top_level.txt
```

### Comparing `charmed-kubeflow-chisme-0.0.9/LICENSE` & `charmed-kubeflow-chisme-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/PKG-INFO` & `charmed-kubeflow-chisme-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmed-kubeflow-chisme
-Version: 0.0.9
+Version: 0.2.0
 Summary: A collection of helpers for Charms maintained by the Charmed Kubeflow team
 Home-page: https://github.com/canonical/charmed-kubeflow-chisme
 Author: Charmed Kubeflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -20,17 +20,20 @@
 both the Charmed Operators maintained by the [Charmed Kubeflow](ckf) team as well as anyone else who benefits from them.
 
 # Contents
 
 * [Exceptions](./src/charmed_kubeflow_chisme/exceptions/README.md): A collection of standard Exceptions for use when writing charms.
 * [Kubernetes](./src/charmed_kubeflow_chisme/kubernetes/README.md): Helpers for interacting with Kubernetes
 * [Lightkube](./src/charmed_kubeflow_chisme/lightkube/README.md): Helpers specific to using or extending [Lightkube](lightkube-rtd)
+* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
+* [Reusable Charm Components](./src/charmed_kubeflow_chisme/components/README.md): The `Component` abstraction that encapsulates any piece of logic for a Charm, a reusable reconcile function `CharmReconciler` that executes `Components`, and a collection of `Components` for things like running Pebble containers or deploying Kubernetes resources
+* [Rock](./src/charmed_kubeflow_chisme/README.md): Utilities for testing ROCKs
 * [Status Handling](./src/charmed_kubeflow_chisme/status_handling/README.md): Helpers for working with Charm Status objects
+* [Testing](./src/charmed_kubeflow_chisme/testing/README.md): Utilities for testing Charms
 * [Types](./src/charmed_kubeflow_chisme/types/README.md): Reusable typing definitions, useful for adding type hints
-* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
```

### Comparing `charmed-kubeflow-chisme-0.0.9/README.md` & `charmed-kubeflow-chisme-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 both the Charmed Operators maintained by the [Charmed Kubeflow](ckf) team as well as anyone else who benefits from them.
 
 # Contents
 
 * [Exceptions](./src/charmed_kubeflow_chisme/exceptions/README.md): A collection of standard Exceptions for use when writing charms.
 * [Kubernetes](./src/charmed_kubeflow_chisme/kubernetes/README.md): Helpers for interacting with Kubernetes
 * [Lightkube](./src/charmed_kubeflow_chisme/lightkube/README.md): Helpers specific to using or extending [Lightkube](lightkube-rtd)
+* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
+* [Reusable Charm Components](./src/charmed_kubeflow_chisme/components/README.md): The `Component` abstraction that encapsulates any piece of logic for a Charm, a reusable reconcile function `CharmReconciler` that executes `Components`, and a collection of `Components` for things like running Pebble containers or deploying Kubernetes resources
+* [Rock](./src/charmed_kubeflow_chisme/README.md): Utilities for testing ROCKs
 * [Status Handling](./src/charmed_kubeflow_chisme/status_handling/README.md): Helpers for working with Charm Status objects
+* [Testing](./src/charmed_kubeflow_chisme/testing/README.md): Utilities for testing Charms
 * [Types](./src/charmed_kubeflow_chisme/types/README.md): Reusable typing definitions, useful for adding type hints
-* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
```

### Comparing `charmed-kubeflow-chisme-0.0.9/pyproject.toml` & `charmed-kubeflow-chisme-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 max-complexity = 10
 exclude = [".git", "__pycache__", ".tox", "build", "dist", "*.egg_info", "venv"]
 select = ["E", "W", "F", "C", "N", "R", "D", "H"]
 # Ignore W503, E501 because using black creates errors with this
 # Ignore D107 Missing docstring in __init__
 ignore = ["W503", "E501", "D107"]
 # D100, D101, D102, D103: Ignore missing docstrings in tests
-per-file-ignores = ["tests/*:D100,D101,D102,D103,D104"]
+per-file-ignores = ["tests/*:D100,D101,D102,D103,D104,F811"]
 docstring-convention = "google"
 # Check for properly formatted copyright header in each file
 copyright-check = "True"
 copyright-author = "Canonical Ltd."
 copyright-regexp = "Copyright\\s\\d{4}([-,]\\d{4})*\\s+%(author)s"
```

### Comparing `charmed-kubeflow-chisme-0.0.9/setup.cfg` & `charmed-kubeflow-chisme-0.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = charmed-kubeflow-chisme
-version = 0.0.9
+version = 0.2.0
 author = Charmed Kubeflow
 description = A collection of helpers for Charms maintained by the Charmed Kubeflow team
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/canonical/charmed-kubeflow-chisme
 classifiers = 
 	Programming Language :: Python :: 3
@@ -17,14 +17,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	deepdiff<=6.2.1
 	jinja2
 	lightkube > 0.10.0
 	ops > 1.2.0
+	serialized-data-interface
 	ruamel.yaml
 	tenacity
 
 [options.extras_require]
 test = 
 	pytest
 	black
```

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/_bundle.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/bundle/_bundle.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,10 +17,10 @@
         some_function()
     except SomeErrorOfTheFunction as e:
         raise GenericCharmRuntimeError("Some function failed because x and y") from e
     """
 
     __module__ = None
 
-    def __init__(self, msg: str):
-        super().__init__(str(msg))
+    def __init__(self, msg: str, *args):
+        super().__init__(str(msg), *args)
         self.msg = str(msg)
```

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_with_status.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/exceptions/_with_status.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/_juju.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/juju/_juju.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 import functools
 import logging
 from pathlib import Path
-from typing import Callable, Iterable, List, Optional, Tuple
+from typing import Callable, Iterable, List, Optional, Tuple, Union
 
 from jinja2 import Template
 from lightkube import Client, codecs
 from lightkube.core.exceptions import ApiError
 from lightkube.core.resource import NamespacedResource, Resource, api_info
 from ops.model import ActiveStatus, BlockedStatus
 
 from ..exceptions import ErrorWithStatus
 from ..lightkube.batch import apply_many, delete_many
 from ..status_handling import get_first_worst_error
 from ..types import (
     LightkubeResourcesList,
     LightkubeResourceType,
-    LightkubeResourceTypesList,
+    LightkubeResourceTypesSet,
 )
 from ..types._charm_status import AnyCharmStatus
 from ._check_resources import check_resources
 
 ERROR_MESSAGE_NO_LABELS = "{caller} requires labels to be set"
-ERROR_MESSAGE_NO_CHILD_RESOURCE_TYPES = "{caller} requires labels to be set"
+ERROR_MESSAGE_NO_RESOURCE_TYPES = "{caller} requires labels to be defined"
 
 
 def auto_clear_manifests_cache(func):
     """Decorates a class's method to delete any cached self._manifest after invocation.
 
     Useful for decorating properties which, when set, invalidate the existing cached manifest.
     """
@@ -44,26 +44,28 @@
 
 class KubernetesResourceHandler:
     """Defines an API for handling Kubernetes resources in charm code."""
 
     def __init__(
         self,
         field_manager: str,
-        template_files: Optional[Iterable[str]] = None,
+        template_files: Optional[Iterable[Union[str, Path]]] = None,
         context: Optional[dict] = None,
         logger: Optional[logging.Logger] = None,
         labels: Optional[dict] = None,
-        child_resource_types: LightkubeResourceTypesList = None,
+        resource_types: LightkubeResourceTypesSet = None,
+        lightkube_client: Client = None,
     ):
         """Returns a KubernetesResourceHandler instance.
 
         Args:
             field_manager (str): The name of the field manager to use when using server-side-apply
                            in kubernetes.  A good option for this is to use the application name
-                           (eg: `self.model.app.name`).
+                           (eg: `self.model.app.name`).  If providing a `lightkube_client` arg,
+                           this value will override that lightkube_client's field_manager.
             template_files (iterable): (Optional) An iterable of template file paths to
                                                render.  This is required to `render_manifests`, but
                                                can be left unset at instantiation and defined later
             context (dict): (Optional) A dict of context used to render the manifests.
                                                This is required to `render_manifests`, but can be
                                                left unset at instantiation and defined later.
             logger (logging.Logger): (Optional) A logger to use for logging (so that log messages
@@ -77,36 +79,37 @@
                            .get_deployed_resources().
                            Recommended input for this is:
                              labels = {
                               'app.kubernetes.io/name': f"{self.model.app.name}-{self.model.name}",
                               'kubernetes-resource-handler-scope': 'some-user-chosen-scope'
                              }
                            See `get_default_labels` for a helper to generate this label dict.
-            child_resource_types (list): (Optional) List of Lightkube Resource objects that define
-                                         the types of child resources managed by this KRH.
-                                         Must be set to use to use .delete(), .reconcile(), or
-                                         .get_deployed_resources().
+            resource_types (set): (Optional) Set of Lightkube Resource objects that define the
+                                   types of child resources managed by this KRH. Must be set to use
+                                   .delete(), .reconcile(), or .get_deployed_resources().
+            lightkube_client (lightkube.Client): (Optional) Lightkube Client to use for all k8s
+                                                 operations.  If omitted, will create its own.
         """
         self._template_files = None
         self.template_files = template_files
         self._context = None
         self.context = context
         self._field_manager = field_manager
-        self.child_resource_types = child_resource_types
+        self.resource_types = resource_types or set()
         self._labels = None
         self.labels = labels
 
         self._manifests = None
 
         if logger is None:
             self.log = logging.getLogger(__name__)  # TODO: Give default logger a better name
         else:
             self.log = logger
 
-        self._lightkube_client = None
+        self._lightkube_client = lightkube_client
 
     def compute_unit_status(self) -> AnyCharmStatus:
         """Returns a suggested unit status given the state of the managed Kubernetes resources.
 
         The returned status is computed by mapping the state of each resource to a suggested unit
         status and then returning the worst status observed.  The statuses roughly map according
         to:
@@ -138,79 +141,81 @@
 
         self.log.debug(
             "Returning status describing Kubernetes resources state (note: this status "
             f"is not applied - that is the responsibility of the charm): {suggested_unit_status}"
         )
         return suggested_unit_status
 
-    def delete(self):
+    def delete(self, ignore_missing=True):
         """Deletes all resources managed by this KubernetesResourceHandler.
 
-        Requires that self.labels and self.child_resource_types be set.
+        Requires that self.labels and self.resource_types be set.
+
+        Args:
+            ignore_missing: *(optional)* Avoid raising 404 errors on deletion (defaults to True)
         """
-        _validate_labels_and_child_resource_types(
-            self.labels, self.child_resource_types, caller_name="delete"
-        )
+        _validate_labels_and_resource_types(self.labels, self.resource_types, caller_name="delete")
 
         resources_to_delete = self.get_deployed_resources()
-        delete_many(self.lightkube_client, resources_to_delete)
+        delete_many(self.lightkube_client, resources_to_delete, ignore_missing, self.log)
 
     def get_deployed_resources(self) -> LightkubeResourcesList:
         """Returns a list of all resources deployed by this KubernetesResourceHandler.
 
-        Requires that self.labels and self.child_resource_types be set.
+        Requires that self.labels and self.resource_types be set.
 
         This method will:
-        * for each resource type listed in self.child_resource_types
+        * for each resource type included in self.resource_types
           * get all resources of that type in the Kubernetes cluster that match the label selector
             defined in self.labels
 
         Returns: A list of Lightkube Resource objects
         """
-        _validate_labels_and_child_resource_types(
-            self.labels, self.child_resource_types, caller_name="get_deployed_resources"
+        _validate_labels_and_resource_types(
+            self.labels, self.resource_types, caller_name="get_deployed_resources"
         )
         resources = []
-        for resource_type in self.child_resource_types:
+        for resource_type in self.resource_types:
             if issubclass(resource_type, NamespacedResource):
                 # Get resources from all namespaces
                 namespace = "*"
             else:
                 # Global resources have no namespace
                 namespace = None
             resources.extend(
                 self.lightkube_client.list(resource_type, namespace=namespace, labels=self._labels)
             )
 
         return resources
 
-    def reconcile(self, force=False):
+    def reconcile(self, force=False, ignore_missing=True):
         """Reconciles the managed resources, removing, updating, or creating objects as required.
 
         This method will:
         * compute a list of Lightkube Resources that are the "desired resources" (the state we
           want, given the current context
-        * for each resource type in self.child_resource_types, get all resources currently deployed
-          that match the label selector in self.labels
+        * for each resource type in self.resource_types, get all resources currently deployed that
+          match the label selector in self.labels
         * compare the current and desired resources, deleting any resources that exist but are not
           in the desired resource list
         * .apply() to update existing objects to the desired state and create new ones
 
         Args:
             force: *(optional)* Passed to self.apply().  This will force apply over any resources
                    marked as managed by another field manager.
+            ignore_missing: *(optional)* Avoid raising 404 errors on deletion (defaults to True)
         """
         existing_resources = self.get_deployed_resources()
         desired_resources = self.render_manifests()
 
         # Delete any resources that exist but are no longer in scope
         resources_to_delete = _in_left_not_right(
             existing_resources, desired_resources, hasher=_hash_lightkube_resource
         )
-        delete_many(self._lightkube_client, resources_to_delete)
+        delete_many(self._lightkube_client, resources_to_delete, ignore_missing, self.log)
 
         # Update remaining resources and create any new ones
         self.apply(force=force)
 
     def render_manifests(
         self,
         template_files: Optional[Iterable[str]] = None,
@@ -287,68 +292,79 @@
             self.log.debug(f"Rendering manifest for {template_file}")
             template = Template(Path(template_file).read_text())
             rendered_template = template.render(**self.context)
             manifest_parts.append(rendered_template)
             self.log.debug(f"Rendered manifest:\n{manifest_parts[-1]}")
         return manifest_parts
 
-    def apply(self, force: bool = False):
+    def apply(self, force: bool = True):
         """Applies the managed Kubernetes resources, adding or modifying these objects.
 
         This can be invoked to create and/or update resources in the kubernetes cluster using
         Kubernetes server-side-apply.  The resources acted upon will be those returned by
         self.render_manifest().
 
         If self.labels is set, the labels will be added to all resources before applying them.
 
-        If self.child_resource_types is set, the a ValueError will be raised if trying to create
-        a resource not in the list.
+        If self.resource_types is set, the a ValueError will be raised if trying to create a
+        resource not in the set.
 
         This function will only add or modify existing objects, it will not delete any resources.
         This includes cases where the manifests have changed over time.  For example:
             * If `render_manifests()` yields the list of resources [PodA], calling `.apply()`
               results in PodA being created
             * If later the charm state has changed and `render_manifests()` yields [PodB], calling
              `.apply()` results in PodB created and PodA being left unchanged (essentially
              orphaned)
         To simultaneously create, update, and delete resources, see self.reconcile().
 
         Args:
-            force: *(optional)* Force is going to "force" Apply requests. It means user will
+            force: *(optional)* Force is going to "force" apply requests. It means user will
                    re-acquire conflicting fields owned by other people.
         """
         resources = self.render_manifests(force_recompute=False)
         self.log.debug(f"Applying {len(resources)} resources")
 
         if self.labels is not None:
             resources = _add_labels_to_resources(resources, self.labels)
 
-        if self.child_resource_types is not None:
+        if self.resource_types:
             try:
-                _validate_resources(resources, allowed_resource_types=self.child_resource_types)
+                _validate_resources(resources, allowed_resource_types=self.resource_types)
             except ValueError as e:
                 raise ValueError(
-                    "Failed to validate resources before applying them.  This likely"
-                    " means we tried to create a resource of type not listed in"
-                    " `KRH.child_resource_types`."
+                    "Failed to validate resources before applying them. This likely means we tried"
+                    " to create a resource of type not included in `KRH.resource_types`."
                 ) from e
 
         try:
-            apply_many(client=self.lightkube_client, objs=resources, force=force)
+            apply_many(
+                client=self.lightkube_client,
+                objs=resources,
+                field_manager=self._field_manager,
+                force=force,
+                logger=self.log,
+            )
         except ApiError as e:
-            # Handle forbidden error as this likely means we do not have --trust
             if e.status.code == 403:
+                # Handle forbidden error as this likely means we do not have --trust
                 self.log.error(
-                    "Received Forbidden (403) error from lightkube when creating resources.  "
-                    "This may be due to the charm lacking permissions to create cluster-scoped "
-                    "roles and resources.  Charm must be deployed with `--trust`"
+                    f"Received Forbidden (403) error from lightkube when creating resources: {e}"
+                    " This may be due to the charm lacking permissions to create cluster-scoped"
+                    " roles and resources. Charm must be deployed with `--trust`"
                 )
-                self.log.error(f"Error received: {str(e)}")
                 raise ErrorWithStatus(
-                    "Cannot apply required resources.  Charm may be missing `--trust`",
+                    "Cannot apply required resources. Charm may be missing `--trust`",
+                    BlockedStatus,
+                )
+            elif self._check_and_report_k8s_conflict(e):
+                # Conflict detected when applying K8s resources
+                raise ErrorWithStatus(
+                    "Cannot apply required resources: conflicts detected. Use with `force=True` to"
+                    " force applying changes to the cluster",
                     BlockedStatus,
                 )
             else:
                 raise e
         self.log.info("Reconcile completed successfully")
 
     @property
@@ -413,14 +429,21 @@
             errors = [error for error in errors if error is not None]
             for i, error in enumerate(errors, start=1):
                 self.log.info(f"Resource issue {i}/{len(errors)}: {error.msg}")
 
         # Return status based on the worst thing we encountered
         return get_first_worst_error(errors).status
 
+    def _check_and_report_k8s_conflict(self, error) -> bool:
+        """Return True if error status code is 409 (conflict), False otherwise."""
+        if error.status.code == 409:
+            self.logger.warning(f"Encountered a conflict: {error}")
+            return True
+        return False
+
 
 def _add_label_field_to_resource(resource: LightkubeResourceType) -> LightkubeResourceType:
     """Adds a metadata.labels field to a Lightkube resource.
 
     Works around a bug where sometimes when the labels field is None it is not overwritable.
     Converts the object to a dict, adds the labels field, and then converts it back to the
     """
@@ -447,21 +470,19 @@
     """Returns a default label style for the KubernetesResourceHandler label selector."""
     return {
         "app.kubernetes.io/instance": f"{application_name}-{model_name}",
         "kubernetes-resource-handler-scope": scope,
     }
 
 
-def _get_resource_classes_in_manifests(resource_list: LightkubeResourcesList):
-    """Returns a list of the resource classes in a list of resources."""
-    resource_classes = []
-    for resource in resource_list:
-        if type(resource) not in resource_classes:
-            resource_classes.append(type(resource))
-    return resource_classes
+def _get_resource_classes_in_manifests(
+    resource_list: LightkubeResourcesList,
+) -> LightkubeResourceTypesSet:
+    """Returns a set of the resource classes in a list of resources."""
+    return {type(rsc) for rsc in resource_list}
 
 
 def _hash_lightkube_resource(resource: Resource) -> Tuple[str, str, str, str, str]:
     """Hashes a Lightkube Resource by returning a tuple of (group, version, kind, name, namespace).
 
     For global resources or resources without a namespace specified, namespace will be None.
     """
@@ -496,30 +517,30 @@
 
     keys_in_left_not_right = set(left_as_dict.keys()) - set(right_as_dict.keys())
     items_in_left_not_right = [left_as_dict[k] for k in keys_in_left_not_right]
 
     return items_in_left_not_right
 
 
-def _validate_labels_and_child_resource_types(labels, child_resource_types, caller_name):
-    """Validates labels and child_resource_types, raising a ValueError if either is empty."""
+def _validate_labels_and_resource_types(labels, resource_types, caller_name):
+    """Validates labels and resource_types, raising a ValueError if either is empty."""
     if not labels:
         raise ValueError(ERROR_MESSAGE_NO_LABELS.format(caller=caller_name))
-    if not child_resource_types:
-        raise ValueError(ERROR_MESSAGE_NO_CHILD_RESOURCE_TYPES.format(caller=caller_name))
+    if not resource_types:
+        raise ValueError(ERROR_MESSAGE_NO_RESOURCE_TYPES.format(caller=caller_name))
 
 
-def _validate_resources(resources, allowed_resource_types: LightkubeResourceTypesList):
-    """Validates that the resources are of a type in the allowed_resource_types list.
+def _validate_resources(resources, allowed_resource_types: LightkubeResourceTypesSet):
+    """Validates that the resources are of a type in the allowed_resource_types set.
 
-    Side effect: raises a ValueError if any resource is not in the allowed_resource_types list.
+    Side effect: raises a ValueError if any resource is not in the allowed_resource_types set.
 
     Args:
         resources: a list of Lightkube resources to validate
-        allowed_resource_types: a list of Lightkube resource classes to validate against
+        allowed_resource_types: a set of Lightkube resource classes to validate against
     """
     resource_types = _get_resource_classes_in_manifests(resources)
     for resource_type in resource_types:
         if resource_type not in allowed_resource_types:
             raise ValueError(
                 f"Resource type {resource_type} not in allowed resource types"
                 f" '{allowed_resource_types}'"
```

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_many.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/_many.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
+import logging
 from typing import Iterable, TypeVar, Union
 
 import lightkube
 from lightkube.core import resource
+from lightkube.core.exceptions import ApiError
 from lightkube.core.resource import GlobalResource, NamespacedResource
 
 # Replace with lightkube.sort_objects once gtsystem/lightkube#33 is merged
 from ._sort_objects import _sort_objects as sort_objects
 
+LOGGER = logging.getLogger(__name__)
+
 GlobalResourceTypeVar = TypeVar("GlobalResource", bound=resource.GlobalResource)
 GlobalSubResourceTypeVar = TypeVar("GlobalSubResource", bound=resource.GlobalSubResource)
 NamespacedResourceTypeVar = TypeVar("NamespacedSubResource", bound=resource.NamespacedResource)
 
 
 def apply_many(
     client: lightkube.Client,
     objs: Iterable[Union[GlobalResourceTypeVar, NamespacedResourceTypeVar]],
     field_manager: str = None,
     force: bool = False,
+    logger: logging.Logger = None,
 ) -> Iterable[Union[GlobalResourceTypeVar, NamespacedResourceTypeVar]]:
     """Create or configure an iterable of Lightkube objects using client.apply().
 
     To avoid referencing objects before they are created, resources are sorted and applied in the
     following order:
     * CRDs
     * Namespaces
@@ -33,65 +38,87 @@
         * RoleBindings and ClusterRoleBindings
     * Everything else (Pod, Deployment, ...)
 
     Sorting is performed using Lightkube's `lightkube.codecs.sort_objects`
 
     Args:
         client: Lightkube client to use for applying resources
-        objs:  iterable of objects to create. This need to be instances of a resource kind and have
-               resource.metadata.namespaced defined if they are namespaced resources
+        objs: Iterable of objects to create. This need to be instances of a resource kind and have
+              resource.metadata.namespaced defined if they are namespaced resources
         field_manager: Name associated with the actor or entity that is making these changes.
         force: *(optional)* Force is going to "force" Apply requests. It means user will
                re-acquire conflicting fields owned by other people.
+        logger: *(optional)* Logger to use for applying resources
 
     Returns:
         A list of Resource objects returned from client.apply().  This list is returned in the
         order the resources were actually applied, not the order in which they're passed as inputs
         in `objs`.
     """
+    logger = logger or LOGGER
     objs = sort_objects(objs)
     returns = [None] * len(objs)
 
     for i, obj in enumerate(objs):
         if isinstance(obj, NamespacedResource):
             namespace = obj.metadata.namespace
         elif isinstance(obj, GlobalResource):
             namespace = None
         else:
             raise TypeError(
                 f"apply_many only supports objects of types NamespacedResource or GlobalResource,"
                 f" got {type(obj)}"
             )
+        logger.debug(f"Creating {obj.__class__} {obj.metadata.name}...")
         returns[i] = client.apply(
             obj=obj, namespace=namespace, field_manager=field_manager, force=force
         )
     return returns
 
 
 def delete_many(
     client: lightkube.Client,
     objs: Iterable[Union[GlobalResourceTypeVar, NamespacedResourceTypeVar]],
+    ignore_missing: bool = True,
+    logger: logging.Logger = None,
 ) -> None:
     """Delete an iterable of objects using client.delete().
 
     To avoid deleting objects that are being used by others in the list (eg: deleting a CRD before
     deleting the CRs), resources are deleted in the reverse order as defined in apply_many
 
     Args:
         client: Lightkube Client to use for deletions
-        objs:  iterable of objects to delete. This need to be instances of a resource kind and have
-               resource.metadata.namespaced defined if they are namespaced resources
+        objs: Iterable of objects to delete. This need to be instances of a resource kind and have
+              resource.metadata.namespaced defined if they are namespaced resources
+        ignore_missing: *(optional)* Avoid raising 404 errors on deletion (defaults to True)
+        logger: *(optional)* Logger to use for deleting resources
     """
+    logger = logger or LOGGER
     objs = sort_objects(objs, reverse=True)
+    exceptions = []
 
     for obj in objs:
         if isinstance(obj, NamespacedResource):
             namespace = obj.metadata.namespace
         elif isinstance(obj, GlobalResource):
             namespace = None
         else:
             raise TypeError(
                 "delete_many only supports objects of types NamespacedResource or GlobalResource,"
                 f" got {type(obj)}"
             )
+        try:
+            logger.debug(f"Deleting {obj.__class__} {obj.metadata.name}...")
+            client.delete(res=obj.__class__, name=obj.metadata.name, namespace=namespace)
+        except ApiError as error:
+            if error.status.code == 404 and ignore_missing:
+                logger.debug(
+                    f"{obj.__class__} {obj.metadata.name} not found! Ignoring because"
+                    f" ignore_missing={ignore_missing}."
+                )
+            else:
+                logger.debug(f"Failed to delete {obj.__class__} {obj.metadata.name}: {error}")
+                exceptions.append(error)
 
-        client.delete(res=obj.__class__, name=obj.metadata.name, namespace=namespace)
+    if exceptions:
+        raise RuntimeError("Deleting K8s resources completed with errors", exceptions)
```

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/mocking.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/lightkube/mocking.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/_update_layer.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/pebble/_update_layer.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/PKG-INFO` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmed-kubeflow-chisme
-Version: 0.0.9
+Version: 0.2.0
 Summary: A collection of helpers for Charms maintained by the Charmed Kubeflow team
 Home-page: https://github.com/canonical/charmed-kubeflow-chisme
 Author: Charmed Kubeflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -20,17 +20,20 @@
 both the Charmed Operators maintained by the [Charmed Kubeflow](ckf) team as well as anyone else who benefits from them.
 
 # Contents
 
 * [Exceptions](./src/charmed_kubeflow_chisme/exceptions/README.md): A collection of standard Exceptions for use when writing charms.
 * [Kubernetes](./src/charmed_kubeflow_chisme/kubernetes/README.md): Helpers for interacting with Kubernetes
 * [Lightkube](./src/charmed_kubeflow_chisme/lightkube/README.md): Helpers specific to using or extending [Lightkube](lightkube-rtd)
+* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
+* [Reusable Charm Components](./src/charmed_kubeflow_chisme/components/README.md): The `Component` abstraction that encapsulates any piece of logic for a Charm, a reusable reconcile function `CharmReconciler` that executes `Components`, and a collection of `Components` for things like running Pebble containers or deploying Kubernetes resources
+* [Rock](./src/charmed_kubeflow_chisme/README.md): Utilities for testing ROCKs
 * [Status Handling](./src/charmed_kubeflow_chisme/status_handling/README.md): Helpers for working with Charm Status objects
+* [Testing](./src/charmed_kubeflow_chisme/testing/README.md): Utilities for testing Charms
 * [Types](./src/charmed_kubeflow_chisme/types/README.md): Reusable typing definitions, useful for adding type hints
-* [Pebble](./src/charmed_kubeflow_chisme/pebble/README.md): Helpers for managing pebble when writing charms
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
```

### Comparing `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt` & `charmed-kubeflow-chisme-0.2.0/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 src/charmed_kubeflow_chisme.egg-info/PKG-INFO
 src/charmed_kubeflow_chisme.egg-info/SOURCES.txt
 src/charmed_kubeflow_chisme.egg-info/dependency_links.txt
 src/charmed_kubeflow_chisme.egg-info/requires.txt
 src/charmed_kubeflow_chisme.egg-info/top_level.txt
 src/charmed_kubeflow_chisme/bundle/__init__.py
 src/charmed_kubeflow_chisme/bundle/_bundle.py
+src/charmed_kubeflow_chisme/components/__init__.py
+src/charmed_kubeflow_chisme/components/charm_reconciler.py
+src/charmed_kubeflow_chisme/components/component.py
+src/charmed_kubeflow_chisme/components/component_graph.py
+src/charmed_kubeflow_chisme/components/component_graph_item.py
+src/charmed_kubeflow_chisme/components/kubernetes_component.py
+src/charmed_kubeflow_chisme/components/leadership_gate_component.py
+src/charmed_kubeflow_chisme/components/model_name_gate_component.py
+src/charmed_kubeflow_chisme/components/pebble_component.py
+src/charmed_kubeflow_chisme/components/serialised_data_interface_components.py
 src/charmed_kubeflow_chisme/exceptions/__init__.py
 src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py
 src/charmed_kubeflow_chisme/exceptions/_kubernetes.py
 src/charmed_kubeflow_chisme/exceptions/_with_status.py
 src/charmed_kubeflow_chisme/juju/__init__.py
 src/charmed_kubeflow_chisme/juju/_juju.py
 src/charmed_kubeflow_chisme/kubernetes/__init__.py
@@ -23,12 +33,17 @@
 src/charmed_kubeflow_chisme/lightkube/__init__.py
 src/charmed_kubeflow_chisme/lightkube/mocking.py
 src/charmed_kubeflow_chisme/lightkube/batch/__init__.py
 src/charmed_kubeflow_chisme/lightkube/batch/_many.py
 src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
 src/charmed_kubeflow_chisme/pebble/__init__.py
 src/charmed_kubeflow_chisme/pebble/_update_layer.py
+src/charmed_kubeflow_chisme/rock/__init__.py
+src/charmed_kubeflow_chisme/rock/_check_rock.py
 src/charmed_kubeflow_chisme/status_handling/__init__.py
 src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
+src/charmed_kubeflow_chisme/status_handling/multistatus.py
+src/charmed_kubeflow_chisme/testing/__init__.py
+src/charmed_kubeflow_chisme/testing/serialized_data_interface.py
 src/charmed_kubeflow_chisme/types/__init__.py
 src/charmed_kubeflow_chisme/types/_charm_status.py
 src/charmed_kubeflow_chisme/types/_lightkube.py
```

