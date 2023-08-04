# Comparing `tmp/sbcli-3.4.tar.gz` & `tmp/sbcli-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-plysqbgl\sbcli-3.4.tar", last modified: Fri Aug  4 17:16:34 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-1l2pffxq\sbcli-3.5.tar", last modified: Fri Aug  4 17:32:49 2023, max compression
```

## Comparing `sbcli-3.4.tar` & `sbcli-3.5.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.908977 sbcli-3.4/
--rw-rw-rw-   0        0        0    43356 2023-08-04 17:16:34.907981 sbcli-3.4/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.797132 sbcli-3.4/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.4/management/__init__.py
--rw-rw-rw-   0        0        0    54606 2023-08-04 16:43:57.000000 sbcli-3.4/management/cli.py
--rw-rw-rw-   0        0        0    12293 2023-08-04 17:15:41.000000 sbcli-3.4/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.4/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.4/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.814107 sbcli-3.4/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.4/management/controllers/__init__.py
--rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/cluster_events.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.4/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.4/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.4/management/controllers/events_controller.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.4/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/mgmt_events.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.4/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.4/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/storage_events.py
--rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.4/management/kv_store.py
--rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.4/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.836028 sbcli-3.4/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.4/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.4/management/models/base_model.py
--rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.4/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.4/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.4/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.4/management/models/events.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.4/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.4/management/models/iface.py
--rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.4/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.4/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.4/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.4/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.4/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.4/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.854007 sbcli-3.4/management/scripts/
--rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.4/management/scripts/__init__.py
--rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/db_config_single.sh
--rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/deploy_stack.sh
--rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.4/management/scripts/docker-compose-swarm.yml
--rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.4/management/scripts/haproxy.cfg
--rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/install_deps.sh
--rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/prepare_mgmt.sh
--rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/set_db_config.sh
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.873939 sbcli-3.4/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.4/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.4/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.4/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0      832 2021-11-04 16:27:59.000000 sbcli-3.4/management/services/install_service.sh
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.4/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.4/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.4/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.4/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0      173 2021-11-04 16:10:02.000000 sbcli-3.4/management/services/remove_service.sh
--rw-rw-rw-   0        0        0      245 2023-02-10 18:30:33.000000 sbcli-3.4/management/services/service_template.service
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.4/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.4/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.874925 sbcli-3.4/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.4/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53541 2023-08-04 16:13:04.000000 sbcli-3.4/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.4/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.905986 sbcli-3.4/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43356 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2055 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 17:16:34.908977 sbcli-3.4/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-08-04 17:16:12.000000 sbcli-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.456179 sbcli-3.5/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 17:32:49.456179 sbcli-3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.344477 sbcli-3.5/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.5/management/__init__.py
+-rw-rw-rw-   0        0        0    54606 2023-08-04 16:43:57.000000 sbcli-3.5/management/cli.py
+-rw-rw-rw-   0        0        0    12293 2023-08-04 17:15:41.000000 sbcli-3.5/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.5/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.5/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.363426 sbcli-3.5/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.5/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.5/management/controllers/cluster_events.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.5/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.5/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.5/management/controllers/events_controller.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.5/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.5/management/controllers/mgmt_events.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.5/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.5/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.5/management/controllers/storage_events.py
+-rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.5/management/kv_store.py
+-rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.5/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.385369 sbcli-3.5/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.5/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.5/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.5/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.5/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.5/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.5/management/models/events.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.5/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.5/management/models/iface.py
+-rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.5/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.5/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.5/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.5/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.5/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.5/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.404317 sbcli-3.5/management/scripts/
+-rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.5/management/scripts/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.5/management/scripts/db_config_single.sh
+-rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.5/management/scripts/deploy_stack.sh
+-rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.5/management/scripts/docker-compose-swarm.yml
+-rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.5/management/scripts/haproxy.cfg
+-rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.5/management/scripts/install_deps.sh
+-rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.5/management/scripts/prepare_mgmt.sh
+-rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.5/management/scripts/set_db_config.sh
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.425260 sbcli-3.5/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.5/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.5/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.5/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0      865 2023-08-04 17:32:07.000000 sbcli-3.5/management/services/install_service.sh
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.5/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.5/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.5/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.5/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0      173 2021-11-04 16:10:02.000000 sbcli-3.5/management/services/remove_service.sh
+-rw-rw-rw-   0        0        0      245 2023-02-10 18:30:33.000000 sbcli-3.5/management/services/service_template.service
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.5/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.5/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.428253 sbcli-3.5/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.5/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0     1693 2023-08-04 16:23:47.000000 sbcli-3.5/management/spdk_installer/install_spdk.sh
+-rw-rw-rw-   0        0        0    53541 2023-08-04 16:13:04.000000 sbcli-3.5/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.5/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-04 17:32:49.454187 sbcli-3.5/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2097 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 17:32:49.000000 sbcli-3.5/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:32:49.457176 sbcli-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-08-04 17:32:26.000000 sbcli-3.5/setup.py
```

### Comparing `sbcli-3.4/PKG-INFO` & `sbcli-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.4
+Version: 3.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.4/README.md` & `sbcli-3.5/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/cli.py` & `sbcli-3.5/management/cli.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/cluster_ops.py` & `sbcli-3.5/management/cluster_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/compute_node_ops.py` & `sbcli-3.5/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/constants.py` & `sbcli-3.5/management/constants.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/cluster_events.py` & `sbcli-3.5/management/controllers/cluster_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/cluster_lifecycle.py` & `sbcli-3.5/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/device_lifecycle.py` & `sbcli-3.5/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/events_controller.py` & `sbcli-3.5/management/controllers/events_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/lvol_controller.py` & `sbcli-3.5/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/mgmt_events.py` & `sbcli-3.5/management/controllers/mgmt_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/node_lifecycle.py` & `sbcli-3.5/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/pool_controller.py` & `sbcli-3.5/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/controllers/storage_events.py` & `sbcli-3.5/management/controllers/storage_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/kv_store.py` & `sbcli-3.5/management/kv_store.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/mgmt_node_ops.py` & `sbcli-3.5/management/mgmt_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/base_model.py` & `sbcli-3.5/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/cluster.py` & `sbcli-3.5/management/models/cluster.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/compute_node.py` & `sbcli-3.5/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/device_stat.py` & `sbcli-3.5/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/events.py` & `sbcli-3.5/management/models/events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/global_settings.py` & `sbcli-3.5/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/iface.py` & `sbcli-3.5/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/mgmt_node.py` & `sbcli-3.5/management/models/mgmt_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/nvme_device.py` & `sbcli-3.5/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/pool.py` & `sbcli-3.5/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/models/storage_node.py` & `sbcli-3.5/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/pci_utils.py` & `sbcli-3.5/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/rpc_client.py` & `sbcli-3.5/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/scripts/__init__.py` & `sbcli-3.5/management/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/scripts/docker-compose-swarm.yml` & `sbcli-3.5/management/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/scripts/haproxy.cfg` & `sbcli-3.5/management/scripts/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/scripts/install_deps.sh` & `sbcli-3.5/management/scripts/install_deps.sh`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/__init__.py` & `sbcli-3.5/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/device_monitor.py` & `sbcli-3.5/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/device_stat_collector.py` & `sbcli-3.5/management/services/device_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/install_service.sh` & `sbcli-3.5/management/services/install_service.sh`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 then
     echo "$SERVICE_NAME is installed and running, nothing to do."
     exit 0
 fi
 
 if [ ! -f "/lib/systemd/system/$SERVICE_NAME.service" ]; then
     echo "Creating service unit files..."
-    cp $SERVICE_UNIT_FILE "/lib/systemd/system/$SERVICE_NAME.service"
+    echo $SERVICE_UNIT_FILE
+    sudo cp $SERVICE_UNIT_FILE "/lib/systemd/system/$SERVICE_NAME.service"
     sudo systemctl daemon-reload
     sudo systemctl enable $SERVICE_NAME
     sudo systemctl start $SERVICE_NAME
 else
     echo "$SERVICE_NAME stopped, trying to start it..."
     sudo systemctl enable $SERVICE_NAME
     sudo systemctl start $SERVICE_NAME
```

### Comparing `sbcli-3.4/management/services/lvol_stat_collector.py` & `sbcli-3.5/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/mgmt_node_monitor.py` & `sbcli-3.5/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/node_monitor.py` & `sbcli-3.5/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/port_stat_collector.py` & `sbcli-3.5/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/services/stat_collector.py` & `sbcli-3.5/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/spdk_installer/__init__.py` & `sbcli-3.5/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/storage_node_ops.py` & `sbcli-3.5/management/storage_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/management/utils.py` & `sbcli-3.5/management/utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.4/sbcli.egg-info/PKG-INFO` & `sbcli-3.5/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.4
+Version: 3.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.4/sbcli.egg-info/SOURCES.txt` & `sbcli-3.5/sbcli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,14 @@
 management/services/mgmt_node_monitor.py
 management/services/node_monitor.py
 management/services/port_stat_collector.py
 management/services/remove_service.sh
 management/services/service_template.service
 management/services/stat_collector.py
 management/spdk_installer/__init__.py
+management/spdk_installer/install_spdk.sh
 sbcli.egg-info/PKG-INFO
 sbcli.egg-info/SOURCES.txt
 sbcli.egg-info/dependency_links.txt
 sbcli.egg-info/entry_points.txt
 sbcli.egg-info/requires.txt
 sbcli.egg-info/top_level.txt
```

### Comparing `sbcli-3.4/setup.py` & `sbcli-3.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='3.4',
+    version='3.5',
     packages=find_packages(),
     url='https://github.com/',
     author='Hamdy Khader',
     author_email='hamdy.khader@gmail.com',
     description='CLI for managing SimplyBlock cluster',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -23,9 +23,9 @@
     ],
     entry_points={
         'console_scripts': [
             'sbcli=management.cli:main',
         ]
     },
     include_package_data=True,
-    package_data={'': ['scripts/*.*', 'services/*.*']},
+    package_data={'': ['scripts/*.*', 'services/*.*', 'spdk_installer/*.*']},
 )
```

