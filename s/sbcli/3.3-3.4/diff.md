# Comparing `tmp/sbcli-3.3.tar.gz` & `tmp/sbcli-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-ug2nriv4\sbcli-3.3.tar", last modified: Fri Aug  4 16:39:50 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-plysqbgl\sbcli-3.4.tar", last modified: Fri Aug  4 17:16:34 2023, max compression
```

## Comparing `sbcli-3.3.tar` & `sbcli-3.4.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.222340 sbcli-3.3/
--rw-rw-rw-   0        0        0    43356 2023-08-04 16:39:50.221344 sbcli-3.3/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.111636 sbcli-3.3/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.3/management/__init__.py
--rw-rw-rw-   0        0        0    54640 2023-08-04 16:13:04.000000 sbcli-3.3/management/cli.py
--rw-rw-rw-   0        0        0    12292 2023-08-04 16:13:04.000000 sbcli-3.3/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.3/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.3/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.133577 sbcli-3.3/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.3/management/controllers/__init__.py
--rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/cluster_events.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.3/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.3/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.3/management/controllers/events_controller.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.3/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/mgmt_events.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.3/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.3/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/storage_events.py
--rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.3/management/kv_store.py
--rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.3/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.157513 sbcli-3.3/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.3/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.3/management/models/base_model.py
--rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.3/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.3/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.3/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.3/management/models/events.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.3/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.3/management/models/iface.py
--rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.3/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.3/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.3/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.3/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.3/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.3/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.171504 sbcli-3.3/management/scripts/
--rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.3/management/scripts/__init__.py
--rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/db_config_single.sh
--rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/deploy_stack.sh
--rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.3/management/scripts/docker-compose-swarm.yml
--rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.3/management/scripts/haproxy.cfg
--rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/install_deps.sh
--rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/prepare_mgmt.sh
--rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/set_db_config.sh
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.190426 sbcli-3.3/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.3/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.3/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.3/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.3/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.3/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.3/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.3/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.3/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.3/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.191423 sbcli-3.3/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.3/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53541 2023-08-04 16:13:04.000000 sbcli-3.3/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.3/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.219350 sbcli-3.3/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43356 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1933 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 16:39:50.223337 sbcli-3.3/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-08-04 16:39:27.000000 sbcli-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.908977 sbcli-3.4/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 17:16:34.907981 sbcli-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.797132 sbcli-3.4/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.4/management/__init__.py
+-rw-rw-rw-   0        0        0    54606 2023-08-04 16:43:57.000000 sbcli-3.4/management/cli.py
+-rw-rw-rw-   0        0        0    12293 2023-08-04 17:15:41.000000 sbcli-3.4/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.4/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.4/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.814107 sbcli-3.4/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.4/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/cluster_events.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.4/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.4/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.4/management/controllers/events_controller.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.4/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/mgmt_events.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.4/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.4/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.4/management/controllers/storage_events.py
+-rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.4/management/kv_store.py
+-rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.4/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.836028 sbcli-3.4/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.4/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.4/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.4/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.4/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.4/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.4/management/models/events.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.4/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.4/management/models/iface.py
+-rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.4/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.4/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.4/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.4/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.4/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.4/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.854007 sbcli-3.4/management/scripts/
+-rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.4/management/scripts/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/db_config_single.sh
+-rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/deploy_stack.sh
+-rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.4/management/scripts/docker-compose-swarm.yml
+-rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.4/management/scripts/haproxy.cfg
+-rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/install_deps.sh
+-rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/prepare_mgmt.sh
+-rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.4/management/scripts/set_db_config.sh
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.873939 sbcli-3.4/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.4/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.4/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.4/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0      832 2021-11-04 16:27:59.000000 sbcli-3.4/management/services/install_service.sh
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.4/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.4/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.4/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.4/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0      173 2021-11-04 16:10:02.000000 sbcli-3.4/management/services/remove_service.sh
+-rw-rw-rw-   0        0        0      245 2023-02-10 18:30:33.000000 sbcli-3.4/management/services/service_template.service
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.4/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.4/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.874925 sbcli-3.4/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.4/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0    53541 2023-08-04 16:13:04.000000 sbcli-3.4/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.4/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-04 17:16:34.905986 sbcli-3.4/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2055 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 17:16:34.000000 sbcli-3.4/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:16:34.908977 sbcli-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-08-04 17:16:12.000000 sbcli-3.4/setup.py
```

### Comparing `sbcli-3.3/PKG-INFO` & `sbcli-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.3
+Version: 3.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.3/README.md` & `sbcli-3.4/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/cli.py` & `sbcli-3.4/management/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,16 +232,15 @@
         sub_command.add_argument("NQN", help='cluster NQN subsystem')
         sub_command.add_argument("--CLI_PASS", help='Password for CLI SSH connection', required=False)
 
         # join cluster
         sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
         sub_command.add_argument("cluster_ip", help='the cluster IP address')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("role", help='Choose the node role in the cluster',
-                                 choices=["management", "storage"])
+        sub_command.add_argument("role", help='Choose the node role in the cluster', choices=["management", "storage"])
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
 
         # show cluster info
         sub_command = self.add_sub_command(
             subparser, 'status', 'Show cluster status')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
```

### Comparing `sbcli-3.3/management/cluster_ops.py` & `sbcli-3.4/management/cluster_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     try:
         c = docker.DockerClient(base_url=f"tcp://{docker_ip}", version="auto")
         if role == 'management':
             join_token = c.swarm.attrs['JoinTokens']['Manager']
         else:
             join_token = c.swarm.attrs['JoinTokens']['Worker']
         c = docker.DockerClient(base_url=f"tcp://{DEV_IP}:2375", version="auto")
-        c.swarm.join([docker_ip.split(":")[0]+"2377"], join_token)
+        c.swarm.join([docker_ip.split(":")[0]+":2377"], join_token)
         logger.info("Joining docker swarm > Done")
     except Exception as e:
         raise e
 
     # logger.info("Configuring DB...")
     # time.sleep(5)
     # out = scripts.set_db_config_single()
```

### Comparing `sbcli-3.3/management/compute_node_ops.py` & `sbcli-3.4/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/constants.py` & `sbcli-3.4/management/constants.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/cluster_events.py` & `sbcli-3.4/management/controllers/cluster_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/cluster_lifecycle.py` & `sbcli-3.4/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/device_lifecycle.py` & `sbcli-3.4/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/events_controller.py` & `sbcli-3.4/management/controllers/events_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/lvol_controller.py` & `sbcli-3.4/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/mgmt_events.py` & `sbcli-3.4/management/controllers/mgmt_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/node_lifecycle.py` & `sbcli-3.4/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/pool_controller.py` & `sbcli-3.4/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/controllers/storage_events.py` & `sbcli-3.4/management/controllers/storage_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/kv_store.py` & `sbcli-3.4/management/kv_store.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/mgmt_node_ops.py` & `sbcli-3.4/management/mgmt_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/base_model.py` & `sbcli-3.4/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/cluster.py` & `sbcli-3.4/management/models/cluster.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/compute_node.py` & `sbcli-3.4/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/device_stat.py` & `sbcli-3.4/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/events.py` & `sbcli-3.4/management/models/events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/global_settings.py` & `sbcli-3.4/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/iface.py` & `sbcli-3.4/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/mgmt_node.py` & `sbcli-3.4/management/models/mgmt_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/nvme_device.py` & `sbcli-3.4/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/pool.py` & `sbcli-3.4/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/models/storage_node.py` & `sbcli-3.4/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/pci_utils.py` & `sbcli-3.4/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/rpc_client.py` & `sbcli-3.4/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/scripts/__init__.py` & `sbcli-3.4/management/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/scripts/docker-compose-swarm.yml` & `sbcli-3.4/management/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/scripts/haproxy.cfg` & `sbcli-3.4/management/scripts/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/scripts/install_deps.sh` & `sbcli-3.4/management/scripts/install_deps.sh`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/__init__.py` & `sbcli-3.4/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/device_monitor.py` & `sbcli-3.4/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/device_stat_collector.py` & `sbcli-3.4/management/services/device_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/lvol_stat_collector.py` & `sbcli-3.4/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/mgmt_node_monitor.py` & `sbcli-3.4/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/node_monitor.py` & `sbcli-3.4/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/port_stat_collector.py` & `sbcli-3.4/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/services/stat_collector.py` & `sbcli-3.4/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/spdk_installer/__init__.py` & `sbcli-3.4/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/storage_node_ops.py` & `sbcli-3.4/management/storage_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/management/utils.py` & `sbcli-3.4/management/utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.3/sbcli.egg-info/PKG-INFO` & `sbcli-3.4/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.3
+Version: 3.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.3/sbcli.egg-info/SOURCES.txt` & `sbcli-3.4/sbcli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,21 @@
 management/scripts/haproxy.cfg
 management/scripts/install_deps.sh
 management/scripts/prepare_mgmt.sh
 management/scripts/set_db_config.sh
 management/services/__init__.py
 management/services/device_monitor.py
 management/services/device_stat_collector.py
+management/services/install_service.sh
 management/services/lvol_stat_collector.py
 management/services/mgmt_node_monitor.py
 management/services/node_monitor.py
 management/services/port_stat_collector.py
+management/services/remove_service.sh
+management/services/service_template.service
 management/services/stat_collector.py
 management/spdk_installer/__init__.py
 sbcli.egg-info/PKG-INFO
 sbcli.egg-info/SOURCES.txt
 sbcli.egg-info/dependency_links.txt
 sbcli.egg-info/entry_points.txt
 sbcli.egg-info/requires.txt
```

### Comparing `sbcli-3.3/setup.py` & `sbcli-3.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='3.3',
+    version='3.4',
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
-    package_data={'': ['scripts/*.*']},
+    package_data={'': ['scripts/*.*', 'services/*.*']},
 )
```

