# Comparing `tmp/sbcli-3.1.tar.gz` & `tmp/sbcli-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-636hp240\sbcli-3.1.tar", last modified: Thu Aug  3 20:58:41 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-jvmhi78i\sbcli-3.2.tar", last modified: Thu Aug  3 22:56:39 2023, max compression
```

## Comparing `sbcli-3.1.tar` & `sbcli-3.2.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.157622 sbcli-3.1/
--rw-rw-rw-   0        0        0    43356 2023-08-03 20:58:41.156626 sbcli-3.1/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:40.953168 sbcli-3.1/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.1/management/__init__.py
--rw-rw-rw-   0        0        0    54198 2023-08-03 20:32:22.000000 sbcli-3.1/management/cli.py
--rw-rw-rw-   0        0        0    12261 2023-08-03 20:32:22.000000 sbcli-3.1/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.1/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.1/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.010017 sbcli-3.1/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.1/management/controllers/__init__.py
--rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/cluster_events.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.1/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.1/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.1/management/controllers/events_controller.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.1/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/mgmt_events.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.1/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.1/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.1/management/controllers/storage_events.py
--rw-rw-rw-   0        0        0     5834 2023-08-03 20:21:48.000000 sbcli-3.1/management/kv_store.py
--rw-rw-rw-   0        0        0     3649 2023-08-03 20:21:48.000000 sbcli-3.1/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.058886 sbcli-3.1/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.1/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.1/management/models/base_model.py
--rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.1/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.1/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/events.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.1/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.1/management/models/iface.py
--rw-rw-rw-   0        0        0      673 2023-08-03 20:21:48.000000 sbcli-3.1/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.1/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.1/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.1/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.1/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.1/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.069857 sbcli-3.1/management/scripts/
--rw-rw-rw-   0        0        0     1050 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/__init__.py
--rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/db_config_single.sh
--rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/deploy_stack.sh
--rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/install_deps.sh
--rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/prepare_mgmt.sh
--rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.1/management/scripts/set_db_config.sh
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.123712 sbcli-3.1/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.1/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.1/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.1/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.1/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.1/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.1/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.1/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.1/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.1/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.126705 sbcli-3.1/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.1/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-3.1/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.1/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-03 20:58:41.154631 sbcli-3.1/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43356 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 20:58:40.000000 sbcli-3.1/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 20:58:41.157622 sbcli-3.1/setup.cfg
--rw-rw-rw-   0        0        0      819 2023-08-03 20:54:24.000000 sbcli-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.231159 sbcli-3.2/
+-rw-rw-rw-   0        0        0    43356 2023-08-03 22:56:39.230161 sbcli-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.123446 sbcli-3.2/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-3.2/management/__init__.py
+-rw-rw-rw-   0        0        0    54183 2023-08-03 21:15:28.000000 sbcli-3.2/management/cli.py
+-rw-rw-rw-   0        0        0    11947 2023-08-03 22:53:27.000000 sbcli-3.2/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-3.2/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      795 2023-08-03 20:21:48.000000 sbcli-3.2/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.142397 sbcli-3.2/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-3.2/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/cluster_events.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-3.2/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-3.2/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0     1019 2023-08-01 03:44:27.000000 sbcli-3.2/management/controllers/events_controller.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-3.2/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0     3578 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/mgmt_events.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-3.2/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-3.2/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0    36931 2023-08-01 03:53:15.000000 sbcli-3.2/management/controllers/storage_events.py
+-rw-rw-rw-   0        0        0     5851 2023-08-03 21:53:05.000000 sbcli-3.2/management/kv_store.py
+-rw-rw-rw-   0        0        0     3624 2023-08-03 22:29:29.000000 sbcli-3.2/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.167328 sbcli-3.2/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-3.2/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-3.2/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1871 2023-08-03 20:21:48.000000 sbcli-3.2/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-3.2/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-3.2/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1140 2023-08-03 20:21:48.000000 sbcli-3.2/management/models/events.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-3.2/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-3.2/management/models/iface.py
+-rw-rw-rw-   0        0        0      672 2023-08-03 22:29:29.000000 sbcli-3.2/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-3.2/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-3.2/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-3.2/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-3.2/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-3.2/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.181290 sbcli-3.2/management/scripts/
+-rw-rw-rw-   0        0        0     1052 2023-08-03 21:52:24.000000 sbcli-3.2/management/scripts/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/db_config_single.sh
+-rw-rw-rw-   0        0        0      310 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/deploy_stack.sh
+-rw-rw-rw-   0        0        0     2908 2023-08-03 21:52:24.000000 sbcli-3.2/management/scripts/docker-compose-swarm.yml
+-rw-rw-rw-   0        0        0     1216 2023-07-07 17:10:45.000000 sbcli-3.2/management/scripts/haproxy.cfg
+-rw-rw-rw-   0        0        0     1125 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/install_deps.sh
+-rw-rw-rw-   0        0        0        0 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/prepare_mgmt.sh
+-rw-rw-rw-   0        0        0       62 2023-08-03 20:21:48.000000 sbcli-3.2/management/scripts/set_db_config.sh
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.195257 sbcli-3.2/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-3.2/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-3.2/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3517 2023-08-01 03:53:15.000000 sbcli-3.2/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-3.2/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-3.2/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-3.2/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-3.2/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-3.2/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-3.2/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.196252 sbcli-3.2/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-3.2/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-3.2/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     2061 2023-08-03 20:24:10.000000 sbcli-3.2/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-3.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-03 22:56:39.229164 sbcli-3.2/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43356 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1933 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 22:56:39.000000 sbcli-3.2/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 22:56:39.231159 sbcli-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-08-03 21:59:56.000000 sbcli-3.2/setup.py
```

### Comparing `sbcli-3.1/PKG-INFO` & `sbcli-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.1
+Version: 3.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.1/README.md` & `sbcli-3.2/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/cli.py` & `sbcli-3.2/management/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -954,15 +954,15 @@
             else:
                 return size_string
         except:
             print(f"Error parsing size: {size_string}")
             exit(-1)
 
 
-if __name__ == '__main__':
+def main():
     logger_handler = logging.StreamHandler()
     logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
     logger = logging.getLogger()
     logger.addHandler(logger_handler)
 
     cli = CLIWrapper()
     cli.run()
```

### Comparing `sbcli-3.1/management/cluster_ops.py` & `sbcli-3.2/management/cluster_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     except Exception as e:
         print(e)
 
     if not cli_pass:
         cli_pass = utils.generate_string(10)
 
     logger.info("Deploying swarm stack ...")
-    ret = scripts.deploy_stack(constants.TOP_DIR, cli_pass, DEV_IP)
+    ret = scripts.deploy_stack(cli_pass, DEV_IP)
     # print(f"Return code: {ret}")
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     time.sleep(5)
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
@@ -84,15 +84,15 @@
 
 def join_cluster(cluster_ip, cluster_id):
 
     try:
         resp = requests.get(f"http://{cluster_ip}/cluster/{cluster_id}")
         resp_json = resp.json()
         cluster_data = resp_json['results'][0]
-        logger.info(f"Cluster found! NQN:{cluster_data['NQN']}")
+        logger.info(f"Cluster found! NQN:{cluster_data['nqn']}")
         logger.debug(cluster_data)
     except Exception as e:
         logger.error("Error getting cluster data!")
         logger.error(e)
         return ""
     # db_controller = DBController()
     # cls = db_controller.get_clusters(id=cl_id)
@@ -121,42 +121,30 @@
     if not nodes:
         logger.error("No mgmt nodes was found in the cluster!")
         exit(1)
 
     docker_ip = nodes[0].docker_ip_port
     try:
         c = docker.DockerClient(base_url=f"tcp://{docker_ip}", version="auto")
-
-        join_token = c.swarm.attrs['JoinTokens']['Worker']
-
-        # c = docker.DockerClient.from_env()
+        join_token = c.swarm.attrs['JoinTokens']['Manager']
         c = docker.DockerClient(base_url=f"tcp://{DEV_IP}:2375", version="auto")
-
-        ''''
-         c.swarm.attrs['JoinTokens']
-{'Worker': 'SWMTKN-1-3azhgb2ervctd3csc73kk25qrh4dc12v0qgboriga8boj4w9b0-8u6f8v3qpg5brv6t5rxdt2ics', 'Manager': 'SWMTKN-1-3azhgb2ervctd3csc73kk25qrh4dc12v0qgboriga8boj4w9b0-djugybjis6ambbfq78yz0juja'}
-
-        '''
-        c.swarm.join(docker_ip, join_token)
+        c.swarm.join([docker_ip.split(":")[0]+"2377"], join_token)
         logger.info("Joining docker swarm > Done")
     except Exception as e:
-        print(e)
-
-    logger.info("Configuring DB...")
-    time.sleep(5)
-    out = scripts.set_db_config_single()
-    logger.info("Configuring DB > Done")
+        raise e
 
+    # logger.info("Configuring DB...")
+    # time.sleep(5)
+    # out = scripts.set_db_config_single()
+    # logger.info("Configuring DB > Done")
 
     mgmt_node_ops.add_mgmt_node(f"{DEV_IP}:2375", cluster_id)
-
     logger.info("Node joined the cluster")
 
 
-
 def add_cluster(blk_size, page_size_in_blocks, model_ids, ha_type, tls,
                 auth_hosts_only, dhchap, nqn, iscsi, cli_pass):
     db_controller = DBController()
     logger.info("Adding new cluster")
     c = Cluster()
     c.uuid = str(uuid.uuid4())
     c.blk_size = blk_size
```

### Comparing `sbcli-3.1/management/compute_node_ops.py` & `sbcli-3.2/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/constants.py` & `sbcli-3.2/management/constants.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/cluster_events.py` & `sbcli-3.2/management/controllers/cluster_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/cluster_lifecycle.py` & `sbcli-3.2/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/device_lifecycle.py` & `sbcli-3.2/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/events_controller.py` & `sbcli-3.2/management/controllers/events_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/lvol_controller.py` & `sbcli-3.2/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/mgmt_events.py` & `sbcli-3.2/management/controllers/mgmt_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/node_lifecycle.py` & `sbcli-3.2/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/pool_controller.py` & `sbcli-3.2/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/controllers/storage_events.py` & `sbcli-3.2/management/controllers/storage_events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/kv_store.py` & `sbcli-3.2/management/kv_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             return ret[0]
 
     def get_mgmt_node_by_id(self, id):
         ret = MgmtNode().read_from_db(self.kv_store, id)
         if ret:
             return ret[0]
 
-    def get_mgmt_nodes(self):
+    def get_mgmt_nodes(self, cluster_id=None):
         return MgmtNode().read_from_db(self.kv_store)
 
     def get_mgmt_node_by_hostname(self, hostname):
         nodes = self.get_mgmt_nodes()
         for node in nodes:
             if node.hostname == hostname:
                 return node
```

### Comparing `sbcli-3.1/management/mgmt_node_ops.py` & `sbcli-3.2/management/mgmt_node_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 import datetime
 import json
 import logging
+import uuid
 
 import docker
 
 from management import utils
 from management.kv_store import DBController
 from management.models.mgmt_node import MgmtNode
 
@@ -20,23 +21,23 @@
         except docker.errors.DockerException as e:
             print(e)
     raise e
 
 
 def add_mgmt_node(ip_port, cluster_id=None):
     db_controller = DBController()
-    baseboard_sn = utils.get_baseboard_sn()
-    node = db_controller.get_mgmt_node_by_id(baseboard_sn)
+    hostname = utils.get_hostname()
+    node = db_controller.get_mgmt_node_by_hostname(hostname)
     if node:
         logger.warning("Node already exists in the cluster")
+        return False
 
     node = MgmtNode()
-    node.baseboard_sn = baseboard_sn
-    node.system_uuid = utils.get_system_id()
-    node.hostname = utils.get_hostname()
+    node.system_uuid = str(uuid.uuid4())
+    node.hostname = hostname
     node.docker_ip_port = ip_port
     node.cluster_id = cluster_id
     node.status = 'active'
     node.write_to_db(db_controller.kv_store)
     logger.info("Done")
     return True
```

### Comparing `sbcli-3.1/management/models/base_model.py` & `sbcli-3.2/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/cluster.py` & `sbcli-3.2/management/models/cluster.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/compute_node.py` & `sbcli-3.2/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/device_stat.py` & `sbcli-3.2/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/events.py` & `sbcli-3.2/management/models/events.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/global_settings.py` & `sbcli-3.2/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/iface.py` & `sbcli-3.2/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/mgmt_node.py` & `sbcli-3.2/management/models/mgmt_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
     def __init__(self, data=None):
         super(MgmtNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
-        return self.baseboard_sn
+        return self.system_uuid
```

### Comparing `sbcli-3.1/management/models/nvme_device.py` & `sbcli-3.2/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/pool.py` & `sbcli-3.2/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/models/storage_node.py` & `sbcli-3.2/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/pci_utils.py` & `sbcli-3.2/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/rpc_client.py` & `sbcli-3.2/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/scripts/__init__.py` & `sbcli-3.2/management/scripts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     return process.returncode
 
 
 def install_deps():
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'install_deps.sh')])
 
 
-def deploy_stack(TD, CLI_PASS, DEV_IP):
-    return __run_script(['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), TD, CLI_PASS, DEV_IP])
+def deploy_stack(CLI_PASS, DEV_IP):
+    return __run_script(['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), DIR_PATH, CLI_PASS, DEV_IP])
 
 
 def set_db_config(DEV_IP):
     return __run_script(['bash', os.path.join(DIR_PATH, 'set_db_config.sh'), DEV_IP])
 
 
 def set_db_config_single():
```

### Comparing `sbcli-3.1/management/scripts/install_deps.sh` & `sbcli-3.2/management/scripts/install_deps.sh`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/__init__.py` & `sbcli-3.2/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/device_monitor.py` & `sbcli-3.2/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/device_stat_collector.py` & `sbcli-3.2/management/services/device_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/lvol_stat_collector.py` & `sbcli-3.2/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/mgmt_node_monitor.py` & `sbcli-3.2/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/node_monitor.py` & `sbcli-3.2/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/port_stat_collector.py` & `sbcli-3.2/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/services/stat_collector.py` & `sbcli-3.2/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/spdk_installer/__init__.py` & `sbcli-3.2/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/storage_node_ops.py` & `sbcli-3.2/management/storage_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/management/utils.py` & `sbcli-3.2/management/utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-3.1/sbcli.egg-info/PKG-INFO` & `sbcli-3.2/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 3.1
+Version: 3.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-3.1/sbcli.egg-info/SOURCES.txt` & `sbcli-3.2/sbcli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 management/models/mgmt_node.py
 management/models/nvme_device.py
 management/models/pool.py
 management/models/storage_node.py
 management/scripts/__init__.py
 management/scripts/db_config_single.sh
 management/scripts/deploy_stack.sh
+management/scripts/docker-compose-swarm.yml
+management/scripts/haproxy.cfg
 management/scripts/install_deps.sh
 management/scripts/prepare_mgmt.sh
 management/scripts/set_db_config.sh
 management/services/__init__.py
 management/services/device_monitor.py
 management/services/device_stat_collector.py
 management/services/lvol_stat_collector.py
```

### Comparing `sbcli-3.1/setup.py` & `sbcli-3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='3.1',
+    version='3.2',
     packages=find_packages(),
     url='https://github.com/',
     author='Hamdy Khader',
     author_email='hamdy.khader@gmail.com',
     description='CLI for managing SimplyBlock cluster',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -19,13 +19,13 @@
         "typing",
         "prettytable",
         "docker",
         "psutil",
     ],
     entry_points={
         'console_scripts': [
-            'sbcli=management.cli:__main__',
+            'sbcli=management.cli:main',
         ]
     },
     include_package_data=True,
-    package_data={'': ['scripts/*.sh']},
+    package_data={'': ['scripts/*.*']},
 )
```

