# Comparing `tmp/sbcli-3.2.tar.gz` & `tmp/sbcli-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-jvmhi78i\sbcli-3.2.tar", last modified: Thu Aug  3 22:56:39 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-ug2nriv4\sbcli-3.3.tar", last modified: Fri Aug  4 16:39:50 2023, max compression
```

## Comparing `sbcli-3.2.tar` & `sbcli-3.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.231159 sbcli-3.2/
--rw-rw-rw-   0        0        0    43356 2023-08-03 22:56:39.230161 sbcli-3.2/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.123446 sbcli-3.2/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.2/management/__init__.py
--rw-rw-rw-   0        0        0    54183 2023-08-03 21:15:28.000000 sbcli-3.2/management/cli.py
--rw-rw-rw-   0        0        0    11947 2023-08-03 22:53:27.000000 sbcli-3.2/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.2/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.2/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.142397 sbcli-3.2/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.2/management/controllers/__init__.py
--rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/cluster_events.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.2/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.2/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.2/management/controllers/events_controller.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.2/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/mgmt_events.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.2/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.2/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/storage_events.py
--rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.2/management/kv_store.py
--rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.2/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.167328 sbcli-3.2/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.2/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.2/management/models/base_model.py
--rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.2/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.2/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.2/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.2/management/models/events.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.2/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.2/management/models/iface.py
--rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.2/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.2/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.2/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.2/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.2/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.2/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.181290 sbcli-3.2/management/scripts/
--rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.2/management/scripts/__init__.py
--rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/db_config_single.sh
--rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/deploy_stack.sh
--rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.2/management/scripts/docker-compose-swarm.yml
--rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.2/management/scripts/haproxy.cfg
--rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/install_deps.sh
--rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/prepare_mgmt.sh
--rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/set_db_config.sh
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.195257 sbcli-3.2/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.2/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.2/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.2/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.2/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.2/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.2/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.2/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.2/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.2/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.196252 sbcli-3.2/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.2/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-3.2/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.2/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.229164 sbcli-3.2/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43356 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1933 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 22:56:39.231159 sbcli-3.2/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-08-03 21:59:56.000000 sbcli-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.222340 sbcli-3.3/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 16:39:50.221344 sbcli-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.111636 sbcli-3.3/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.3/management/__init__.py
+-rw-rw-rw-   0        0        0    54640 2023-08-04 16:13:04.000000 sbcli-3.3/management/cli.py
+-rw-rw-rw-   0        0        0    12292 2023-08-04 16:13:04.000000 sbcli-3.3/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.3/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.3/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.133577 sbcli-3.3/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.3/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/cluster_events.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.3/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.3/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.3/management/controllers/events_controller.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.3/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/mgmt_events.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.3/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.3/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.3/management/controllers/storage_events.py
+-rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.3/management/kv_store.py
+-rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.3/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.157513 sbcli-3.3/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.3/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.3/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.3/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.3/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.3/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.3/management/models/events.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.3/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.3/management/models/iface.py
+-rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.3/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.3/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.3/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.3/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.3/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.3/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.171504 sbcli-3.3/management/scripts/
+-rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.3/management/scripts/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/db_config_single.sh
+-rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/deploy_stack.sh
+-rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.3/management/scripts/docker-compose-swarm.yml
+-rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.3/management/scripts/haproxy.cfg
+-rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/install_deps.sh
+-rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/prepare_mgmt.sh
+-rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.3/management/scripts/set_db_config.sh
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.190426 sbcli-3.3/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.3/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.3/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.3/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.3/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.3/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.3/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.3/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.3/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.3/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.191423 sbcli-3.3/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.3/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0    53541 2023-08-04 16:13:04.000000 sbcli-3.3/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.3/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-04 16:39:50.219350 sbcli-3.3/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43356 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1933 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 16:39:50.000000 sbcli-3.3/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 16:39:50.223337 sbcli-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-08-04 16:39:27.000000 sbcli-3.3/setup.py
```

### Comparing `sbcli-3.2/PKG-INFO` & `sbcli-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.2
+Version: 3.3
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.2/README.md` & `sbcli-3.3/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/cli.py` & `sbcli-3.3/management/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,18 @@
         sub_command.add_argument("NQN", help='cluster NQN subsystem')
         sub_command.add_argument("--CLI_PASS", help='Password for CLI SSH connection', required=False)
 
         # join cluster
         sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
         sub_command.add_argument("cluster_ip", help='the cluster IP address')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
+        sub_command.add_argument("role", help='Choose the node role in the cluster',
+                                 choices=["management", "storage"])
+        sub_command.add_argument("ifname", help='Management interface name')
+        sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
 
         # show cluster info
         sub_command = self.add_sub_command(
             subparser, 'status', 'Show cluster status')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
         sub_command = self.add_sub_command(
@@ -894,15 +898,18 @@
         return cluster_ops.create_cluster(
             blk_size, page_size_in_blocks , ha_type, tls,
             auth_hosts_only, NQN , CLI_PASS)
 
     def cluster_join(self, args):
         cluster_id = args.cluster_id
         cluster_ip = args.cluster_ip
-        return cluster_ops.join_cluster(cluster_ip, cluster_id)
+        role = args.role
+        ifname = args.ifname
+        data_nics = args.data_nics
+        return cluster_ops.join_cluster(cluster_ip, cluster_id, role, ifname, data_nics)
 
     def query_yes_no(self, question, default="yes"):
         """Ask a yes/no question via raw_input() and return their answer.
 
         "question" is a string that is presented to the user.
         "default" is the presumed answer if the user just hits <Enter>.
                 It must be "yes" (the default), "no" or None (meaning
```

### Comparing `sbcli-3.2/management/cluster_ops.py` & `sbcli-3.3/management/cluster_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 import logging
 import time
 import uuid
 
 import requests
 
-from management import utils, scripts, constants,  mgmt_node_ops
+from management import utils, scripts, constants, mgmt_node_ops, storage_node_ops
 from management.controllers import events_controller as ec
 from management.kv_store import DBController
 from management.mgmt_node_ops import _get_docker_client
 from management.models.cluster import Cluster
 from management.models.device_stat import DeviceStat
 
 logger = logging.getLogger()
@@ -78,15 +78,15 @@
 
     mgmt_node_ops.add_mgmt_node(f"{DEV_IP}:2375", c.uuid)
 
     logger.info("New Cluster has been created")
     logger.info(c.uuid)
 
 
-def join_cluster(cluster_ip, cluster_id):
+def join_cluster(cluster_ip, cluster_id, role, ifname, data_nics):  # role: ["management", "storage"]
 
     try:
         resp = requests.get(f"http://{cluster_ip}/cluster/{cluster_id}")
         resp_json = resp.json()
         cluster_data = resp_json['results'][0]
         logger.info(f"Cluster found! NQN:{cluster_data['nqn']}")
         logger.debug(cluster_data)
@@ -121,30 +121,39 @@
     if not nodes:
         logger.error("No mgmt nodes was found in the cluster!")
         exit(1)
 
     docker_ip = nodes[0].docker_ip_port
     try:
         c = docker.DockerClient(base_url=f"tcp://{docker_ip}", version="auto")
-        join_token = c.swarm.attrs['JoinTokens']['Manager']
+        if role == 'management':
+            join_token = c.swarm.attrs['JoinTokens']['Manager']
+        else:
+            join_token = c.swarm.attrs['JoinTokens']['Worker']
         c = docker.DockerClient(base_url=f"tcp://{DEV_IP}:2375", version="auto")
         c.swarm.join([docker_ip.split(":")[0]+"2377"], join_token)
         logger.info("Joining docker swarm > Done")
     except Exception as e:
         raise e
 
     # logger.info("Configuring DB...")
     # time.sleep(5)
     # out = scripts.set_db_config_single()
     # logger.info("Configuring DB > Done")
 
-    mgmt_node_ops.add_mgmt_node(f"{DEV_IP}:2375", cluster_id)
+    if role == 'management':
+        mgmt_node_ops.add_mgmt_node(f"{DEV_IP}:2375", cluster_id)
+    else:
+        # add storage node
+        storage_node_ops.add_storage_node(cluster_id, ifname, data_nics)
+
     logger.info("Node joined the cluster")
 
 
+
 def add_cluster(blk_size, page_size_in_blocks, model_ids, ha_type, tls,
                 auth_hosts_only, dhchap, nqn, iscsi, cli_pass):
     db_controller = DBController()
     logger.info("Adding new cluster")
     c = Cluster()
     c.uuid = str(uuid.uuid4())
     c.blk_size = blk_size
```

### Comparing `sbcli-3.2/management/compute_node_ops.py` & `sbcli-3.3/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/constants.py` & `sbcli-3.3/management/constants.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/cluster_events.py` & `sbcli-3.3/management/controllers/cluster_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/cluster_lifecycle.py` & `sbcli-3.3/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/device_lifecycle.py` & `sbcli-3.3/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/events_controller.py` & `sbcli-3.3/management/controllers/events_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/lvol_controller.py` & `sbcli-3.3/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/mgmt_events.py` & `sbcli-3.3/management/controllers/mgmt_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/node_lifecycle.py` & `sbcli-3.3/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/pool_controller.py` & `sbcli-3.3/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/controllers/storage_events.py` & `sbcli-3.3/management/controllers/storage_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/kv_store.py` & `sbcli-3.3/management/kv_store.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/mgmt_node_ops.py` & `sbcli-3.3/management/mgmt_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/base_model.py` & `sbcli-3.3/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/cluster.py` & `sbcli-3.3/management/models/cluster.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/compute_node.py` & `sbcli-3.3/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/device_stat.py` & `sbcli-3.3/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/events.py` & `sbcli-3.3/management/models/events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/global_settings.py` & `sbcli-3.3/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/iface.py` & `sbcli-3.3/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/mgmt_node.py` & `sbcli-3.3/management/models/mgmt_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/nvme_device.py` & `sbcli-3.3/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/pool.py` & `sbcli-3.3/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/models/storage_node.py` & `sbcli-3.3/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/pci_utils.py` & `sbcli-3.3/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/rpc_client.py` & `sbcli-3.3/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/scripts/__init__.py` & `sbcli-3.3/management/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/scripts/docker-compose-swarm.yml` & `sbcli-3.3/management/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/scripts/haproxy.cfg` & `sbcli-3.3/management/scripts/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/scripts/install_deps.sh` & `sbcli-3.3/management/scripts/install_deps.sh`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/__init__.py` & `sbcli-3.3/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/device_monitor.py` & `sbcli-3.3/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/device_stat_collector.py` & `sbcli-3.3/management/services/device_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/lvol_stat_collector.py` & `sbcli-3.3/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/mgmt_node_monitor.py` & `sbcli-3.3/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/node_monitor.py` & `sbcli-3.3/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/port_stat_collector.py` & `sbcli-3.3/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/services/stat_collector.py` & `sbcli-3.3/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/spdk_installer/__init__.py` & `sbcli-3.3/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/management/storage_node_ops.py` & `sbcli-3.3/management/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,40 +250,39 @@
     clusters = db_controller.get_clusters(cluster_id)
     if not clusters:
         logging.error("Cluster not found: %s", cluster_id)
         return False
     cluster = clusters[0]
 
     logging.info("Add Storage node")
-    subsystem_nqn = cluster.nqn
-    BASE_NQN = subsystem_nqn.split(":")[0]
 
     baseboard_sn = utils.get_baseboard_sn()
     snode = db_controller.get_storage_node_by_id(baseboard_sn)
     if snode:
         logger.error("Node already exists")
         #exit(1)
     else:
         snode = StorageNode()
 
     mgmt_ip = _get_if_ip_address(iface_name)
-
     system_id = utils.get_system_id()
     hostname = utils.get_hostname()
+
+    BASE_NQN = cluster.nqn.split(":")[0]
+    subsystem_nqn = f"{BASE_NQN}:{hostname}"
+
     if data_nics:
         data_nics = _get_data_nics("", data_nics)
     else:
         data_nics = _get_data_nics(iface_name, [])
 
-
     # install spdk
     logger.info("Installing SPDK")
     spdk_installer.install_spdk()
 
-
     logger.info("Creating ultra21 service")
     ultra21 = services.ultra21
     ultra21.init_service()
     time.sleep(3)
     logger.info(f"ultra21 service is running: {ultra21.is_service_running()}")
     snode.services = ["ultra21"]
 
@@ -310,15 +309,15 @@
     # creating storage node object
 
     snode.status = StorageNode.STATUS_IN_CREATION
     snode.baseboard_sn = baseboard_sn
     snode.uuid = baseboard_sn
     snode.system_uuid = system_id
     snode.hostname = hostname
-    snode.host_nqn = f"{BASE_NQN}:{hostname}"
+    snode.host_nqn = subsystem_nqn
     snode.subsystem = subsystem_nqn
     snode.data_nics = data_nics
     snode.mgmt_ip = mgmt_ip
     snode.rpc_port = constants.RPC_HTTP_PROXY_PORT
     snode.rpc_username = rpc_user
     snode.rpc_password = rpc_pass
     snode.write_to_db(kv_store)
```

### Comparing `sbcli-3.2/management/utils.py` & `sbcli-3.3/management/utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/sbcli.egg-info/PKG-INFO` & `sbcli-3.3/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.2
+Version: 3.3
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.2/sbcli.egg-info/SOURCES.txt` & `sbcli-3.3/sbcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbcli-3.2/setup.py` & `sbcli-3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='3.2',
+    version='3.3',
     packages=find_packages(),
     url='https://github.com/',
     author='Hamdy Khader',
     author_email='hamdy.khader@gmail.com',
     description='CLI for managing SimplyBlock cluster',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

