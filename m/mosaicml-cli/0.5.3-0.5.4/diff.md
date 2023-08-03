# Comparing `tmp/mosaicml-cli-0.5.3.tar.gz` & `tmp/mosaicml-cli-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.5.3.tar", last modified: Wed Aug  2 21:37:36 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.5.4.tar", last modified: Thu Aug  3 23:18:34 2023, max compression
```

## Comparing `mosaicml-cli-0.5.3.tar` & `mosaicml-cli-0.5.4.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.884269 mosaicml-cli-0.5.3/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-02 21:37:36.884139 mosaicml-cli-0.5.3/PKG-INFO
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7089 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/README.md
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857267 mosaicml-cli-0.5.3/mcli/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2239 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/__init__.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857731 mosaicml-cli-0.5.3/mcli/api/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/__init__.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.857956 mosaicml-cli-0.5.3/mcli/api/cluster/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      210 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/cluster/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5805 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.858155 mosaicml-cli-0.5.3/mcli/api/engine/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/engine/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    26027 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/engine/engine.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    13444 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/exceptions.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.858428 mosaicml-cli-0.5.3/mcli/api/finetune/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      141 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/finetune/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6802 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/finetune/api_instruction_finetune.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.859364 mosaicml-cli-0.5.3/mcli/api/inference_deployments/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1521 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3297 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5045 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3992 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     8516 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2294 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2746 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6499 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.859728 mosaicml-cli-0.5.3/mcli/api/mint/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/shell.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2676 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/mint/tty.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.860151 mosaicml-cli-0.5.3/mcli/api/model/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1114 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/model/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    10386 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/model/cluster_details.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5770 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/model/inference_deployment.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    14890 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/model/run.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.861323 mosaicml-cli-0.5.3/mcli/api/runs/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1269 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3785 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_create_interactive_run.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3034 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_create_run.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4365 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     8796 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    11001 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5367 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_start_run.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5559 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5916 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_update_run.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4091 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    10049 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.861534 mosaicml-cli-0.5.3/mcli/api/schema/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/schema/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      636 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862018 mosaicml-cli-0.5.3/mcli/api/secrets/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      309 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2386 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2943 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3665 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2354 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/typing_future.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862231 mosaicml-cli-0.5.3/mcli/api/users/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      139 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/users/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2715 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/users/api_get_users.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      920 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/api/utils.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.862450 mosaicml-cli-0.5.3/mcli/cli/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/__init__.py
--rwxr-xr-x   0 tyler.lee   (502) staff       (20)     6069 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/cli.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871104 mosaicml-cli-0.5.3/mcli/cli/common/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/common/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2560 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7464 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871362 mosaicml-cli-0.5.3/mcli/cli/m_connect/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6462 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.871695 mosaicml-cli-0.5.3/mcli/cli/m_create/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2385 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/m_create.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    16900 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872036 mosaicml-cli-0.5.3/mcli/cli/m_delete/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6448 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/delete.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5838 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872230 mosaicml-cli-0.5.3/mcli/cli/m_deploy/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4253 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.872794 mosaicml-cli-0.5.3/mcli/cli/m_describe/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7869 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_clusters.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3929 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    13495 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2719 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.873735 mosaicml-cli-0.5.3/mcli/cli/m_get/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      467 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7069 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/clusters.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6459 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/display.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     8135 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4804 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/m_get.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     8967 2023-08-01 21:45:05.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/runs.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2189 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/secrets.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1580 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_get/users.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.873968 mosaicml-cli-0.5.3/mcli/cli/m_init/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_init/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3908 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874177 mosaicml-cli-0.5.3/mcli/cli/m_interactive/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     9036 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874711 mosaicml-cli-0.5.3/mcli/cli/m_kube/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5523 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1398 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2050 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6946 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.874939 mosaicml-cli-0.5.3/mcli/cli/m_log/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_log/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    11756 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875420 mosaicml-cli-0.5.3/mcli/cli/m_ping/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1411 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875626 mosaicml-cli-0.5.3/mcli/cli/m_predict/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1905 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.875832 mosaicml-cli-0.5.3/mcli/cli/m_root/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_root/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      536 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.876041 mosaicml-cli-0.5.3/mcli/cli/m_run/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_run/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    11501 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.876790 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2964 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1793 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1656 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/organization.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      745 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877027 mosaicml-cli-0.5.3/mcli/cli/m_stop/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4062 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877240 mosaicml-cli-0.5.3/mcli/cli/m_update/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_update/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6560 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_update/m_update.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877571 mosaicml-cli-0.5.3/mcli/cli/m_util/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1161 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/m_util.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     9495 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/cli/m_util/util.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.877792 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3544 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/cli/m_watchdog/m_watchdog.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    13108 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/config.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.878642 mosaicml-cli-0.5.3/mcli/models/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/gpu_type.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    12287 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/inference_deployment_config.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      479 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/models/mcli_cluster.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      456 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/mcli_envvar.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6728 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/models/mcli_secret.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    17258 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/models/run_config.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.878784 mosaicml-cli-0.5.3/mcli/objects/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/__init__.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.879657 mosaicml-cli-0.5.3/mcli/objects/secrets/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1090 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880644 mosaicml-cli-0.5.3/mcli/objects/secrets/create/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1646 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/base.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2244 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2408 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6377 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3858 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5342 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      783 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1017 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/env_var.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      556 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/gcp.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/mounted.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      967 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/oci.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      961 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/s3.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1718 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880871 mosaicml-cli-0.5.3/mcli/proto/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/proto/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1477 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.880994 mosaicml-cli-0.5.3/mcli/sdk/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2006 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/sdk/__init__.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883053 mosaicml-cli-0.5.3/mcli/utils/
--rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/__init__.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6318 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/utils/utils_cli.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4409 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.3/mcli/utils/utils_completers.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_config.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)      740 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_date.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2225 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_epilog.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     7140 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.3/mcli/utils/utils_finetune.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    10774 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_interactive.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4527 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_logging.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     2160 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1087 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.3/mcli/utils/utils_model.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6605 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_pypi.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3115 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_rich.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5358 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.3/mcli/utils/utils_run_status.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     4350 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_spinner.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)    10751 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_string_functions.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1677 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_types.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/mcli/utils/utils_yaml.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3876 2023-08-02 21:36:35.000000 mosaicml-cli-0.5.3/mcli/version.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883688 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/
--rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 tyler.lee   (502) staff       (20)     5225 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tyler.lee   (502) staff       (20)        1 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tyler.lee   (502) staff       (20)       75 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 tyler.lee   (502) staff       (20)     1660 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 tyler.lee   (502) staff       (20)        5 2023-08-02 21:37:36.000000 mosaicml-cli-0.5.3/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 tyler.lee   (502) staff       (20)    31087 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/pyproject.toml
--rw-r--r--   0 tyler.lee   (502) staff       (20)       38 2023-08-02 21:37:36.884306 mosaicml-cli-0.5.3/setup.cfg
--rw-r--r--   0 tyler.lee   (502) staff       (20)     3062 2023-08-02 21:36:35.000000 mosaicml-cli-0.5.3/setup.py
-drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-02 21:37:36.883977 mosaicml-cli-0.5.3/tests/
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6449 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_config.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)       62 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_simple.py
--rw-r--r--   0 tyler.lee   (502) staff       (20)     6116 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.3/tests/test_upgrade.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.368805 mosaicml-cli-0.5.4/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-03 23:18:34.368647 mosaicml-cli-0.5.4/PKG-INFO
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7089 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/README.md
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.324294 mosaicml-cli-0.5.4/mcli/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2239 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.325358 mosaicml-cli-0.5.4/mcli/api/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.325802 mosaicml-cli-0.5.4/mcli/api/cluster/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      210 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5805 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.326352 mosaicml-cli-0.5.4/mcli/api/engine/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/engine/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    26027 2023-08-03 23:09:27.000000 mosaicml-cli-0.5.4/mcli/api/engine/engine.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13444 2023-08-03 23:09:27.000000 mosaicml-cli-0.5.4/mcli/api/exceptions.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.326962 mosaicml-cli-0.5.4/mcli/api/finetune/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      141 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/finetune/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6802 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/finetune/api_instruction_finetune.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.331415 mosaicml-cli-0.5.4/mcli/api/inference_deployments/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1521 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3297 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5045 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4227 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8516 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2294 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2746 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6499 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.332135 mosaicml-cli-0.5.4/mcli/api/mint/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/mint/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/mint/shell.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2676 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/mint/tty.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.333403 mosaicml-cli-0.5.4/mcli/api/model/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1114 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/model/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10386 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5770 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    16761 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/model/run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.336187 mosaicml-cli-0.5.4/mcli/api/runs/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1269 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/runs/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3755 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3004 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4335 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8796 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10941 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5337 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5529 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5886 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4061 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10049 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.336725 mosaicml-cli-0.5.4/mcli/api/schema/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/schema/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      636 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.337655 mosaicml-cli-0.5.4/mcli/api/secrets/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      309 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2386 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2943 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3665 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2354 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/typing_future.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.338245 mosaicml-cli-0.5.4/mcli/api/users/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      139 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/users/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2715 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/users/api_get_users.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      920 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/api/utils.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.338710 mosaicml-cli-0.5.4/mcli/cli/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/__init__.py
+-rwxr-xr-x   0 tyler.lee   (502) staff       (20)     6069 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/cli/cli.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.339463 mosaicml-cli-0.5.4/mcli/cli/common/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/common/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2560 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7464 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.339875 mosaicml-cli-0.5.4/mcli/cli/m_connect/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6462 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.340387 mosaicml-cli-0.5.4/mcli/cli/m_create/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2385 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    16900 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.340992 mosaicml-cli-0.5.4/mcli/cli/m_delete/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6448 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5838 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.341506 mosaicml-cli-0.5.4/mcli/cli/m_deploy/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4253 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.4/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.342544 mosaicml-cli-0.5.4/mcli/cli/m_describe/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7869 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_clusters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3929 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13495 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2719 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.344504 mosaicml-cli-0.5.4/mcli/cli/m_get/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      467 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7069 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6459 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/display.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8135 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4804 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     8967 2023-08-01 21:45:05.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2189 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1580 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.344952 mosaicml-cli-0.5.4/mcli/cli/m_init/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3908 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.345519 mosaicml-cli-0.5.4/mcli/cli/m_interactive/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     9059 2023-08-03 23:17:08.000000 mosaicml-cli-0.5.4/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.346861 mosaicml-cli-0.5.4/mcli/cli/m_kube/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5523 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1398 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2050 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6946 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.347452 mosaicml-cli-0.5.4/mcli/cli/m_log/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    12557 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.348043 mosaicml-cli-0.5.4/mcli/cli/m_ping/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1411 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.4/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.348675 mosaicml-cli-0.5.4/mcli/cli/m_predict/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1905 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.4/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.349387 mosaicml-cli-0.5.4/mcli/cli/m_root/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      536 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.349898 mosaicml-cli-0.5.4/mcli/cli/m_run/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    11501 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.351660 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2964 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1793 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1656 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      840 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      745 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.352203 mosaicml-cli-0.5.4/mcli/cli/m_stop/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4062 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.4/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.352657 mosaicml-cli-0.5.4/mcli/cli/m_update/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6560 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.353365 mosaicml-cli-0.5.4/mcli/cli/m_util/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1161 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     9495 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/cli/m_util/util.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.353928 mosaicml-cli-0.5.4/mcli/cli/m_watchdog/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3544 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    13108 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.355653 mosaicml-cli-0.5.4/mcli/models/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/models/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/models/gpu_type.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    12351 2023-08-03 23:16:23.000000 mosaicml-cli-0.5.4/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      479 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      456 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6728 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/models/mcli_secret.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    17258 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/models/run_config.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.355922 mosaicml-cli-0.5.4/mcli/objects/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.358075 mosaicml-cli-0.5.4/mcli/objects/secrets/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1090 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.360312 mosaicml-cli-0.5.4/mcli/objects/secrets/create/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1646 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2244 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2408 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6377 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3858 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5342 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      783 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1017 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      556 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1267 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      967 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      961 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1718 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.360772 mosaicml-cli-0.5.4/mcli/proto/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/proto/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1477 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.361159 mosaicml-cli-0.5.4/mcli/sdk/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2006 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/sdk/__init__.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.366182 mosaicml-cli-0.5.4/mcli/utils/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        0 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/__init__.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6318 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/utils/utils_cli.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4409 2023-07-25 22:03:34.000000 mosaicml-cli-0.5.4/mcli/utils/utils_completers.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7047 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      740 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_date.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2225 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     7140 2023-08-02 21:36:03.000000 mosaicml-cli-0.5.4/mcli/utils/utils_finetune.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10774 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4527 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_logging.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     2160 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1087 2023-08-02 21:17:13.000000 mosaicml-cli-0.5.4/mcli/utils/utils_model.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6605 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3115 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_rich.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5358 2023-07-18 02:44:37.000000 mosaicml-cli-0.5.4/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     4350 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1103 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    10751 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1677 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_types.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1001 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3876 2023-08-03 23:17:08.000000 mosaicml-cli-0.5.4/mcli/version.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.367728 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)      696 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     5225 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        1 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       75 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     1660 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)        5 2023-08-03 23:18:34.000000 mosaicml-cli-0.5.4/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tyler.lee   (502) staff       (20)    31087 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/pyproject.toml
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       38 2023-08-03 23:18:34.368851 mosaicml-cli-0.5.4/setup.cfg
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     3062 2023-08-02 21:36:35.000000 mosaicml-cli-0.5.4/setup.py
+drwxr-xr-x   0 tyler.lee   (502) staff       (20)        0 2023-08-03 23:18:34.368350 mosaicml-cli-0.5.4/tests/
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6449 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/tests/test_config.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)       62 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/tests/test_simple.py
+-rw-r--r--   0 tyler.lee   (502) staff       (20)     6116 2023-07-14 21:37:02.000000 mosaicml-cli-0.5.4/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.5.3/PKG-INFO` & `mosaicml-cli-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.3
+Version: 0.5.4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.3/README.md` & `mosaicml-cli-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/__init__.py` & `mosaicml-cli-0.5.4/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.5.4/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/engine/engine.py` & `mosaicml-cli-0.5.4/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/exceptions.py` & `mosaicml-cli-0.5.4/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/finetune/api_instruction_finetune.py` & `mosaicml-cli-0.5.4/mcli/api/finetune/api_instruction_finetune.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     hf_checkpoint_path: str = f'{checkpoint_save_folder}/{run_name}/hf_checkpoints'
 
     # For now, we are utilizing the Composer trainer script in llm-foundry.
     # We should consider de-coupling our finetuning service from external, public repos
     integrations: list = [{
         'integration_type': 'git_repo',
         'git_repo': 'mosaicml/llm-foundry',
-        'git_commit': 'bd8127252c660e45ed01413645d29427f86c085a',
+        'git_commit': '05c6055ed38c495df746bcc97ac371fa61acb2ef',
         'pip_install': '-e .[gpu]',
         'ssh_clone': False,  # Should be true if using a private repo
     }]
 
     # Auto-infer instance and number of gpus, defaults to 1 node
     final_gpu_type: Optional[str] = gpu_type
     final_gpus: Optional[int] = gpus
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,37 +22,40 @@
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
     failed: Optional[bool] = False,
+    follow: bool = False,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     failed: Optional[bool] = False,
+    follow: bool = False,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: bool = False,
     failed: Optional[bool] = False,
+    follow: bool = False,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Get the current logs for an active or completed inference deployment
 
     Get the current logs for an active or completed inference deployment in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made.
 
@@ -68,25 +71,27 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_inference_deployment_logs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the log text, use ``return_value.result()`` with an optional
             ``timeout`` argument.
         failed (``bool``): Return the logs of the latest failed deployment if ``True``.
             ``False`` by default.
+        follow (``bool``): Returns the logs of the inference deployment as they are produced if ``True``.
+          Defaults to ``False``.
 
     Returns:
         If future is False:
             The full log text for a inference deployment at the time of the request as a :obj:`str`
         Otherwise:
             A :class:`~concurrent.futures.Future` for the log text
     """
     # Convert to strings
     deployment_name = deployment.name if isinstance(deployment, InferenceDeployment) else deployment
 
-    filters: Dict[str, Any] = {'name': deployment_name, 'failed': failed}
+    filters: Dict[str, Any] = {'name': deployment_name, 'failed': failed, 'follow': follow}
     if restart:
         filters['restartCount'] = restart
 
     variables = {VARIABLE_DATA_NAME: filters}
 
     cfg = MCLIConfig.load_config()
     cfg.update_entity(variables[VARIABLE_DATA_NAME], set_user=False)
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.5.4/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/mint/shell.py` & `mosaicml-cli-0.5.4/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/mint/tty.py` & `mosaicml-cli-0.5.4/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/model/__init__.py` & `mosaicml-cli-0.5.4/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.5.4/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.5.4/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/model/run.py` & `mosaicml-cli-0.5.4/mcli/api/model/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,21 +109,33 @@
 
     Args:
         run_uid (`str`): Unique identifier for the run
         name (`str`): User-defined name of the run
         status (:class:`~mcli.utils.utils_run_status.RunStatus`): Status of the run at a moment in time
         created_at (`datetime`): Date and time when the run was created
         updated_at (`datetime`): Date and time when the run was last updated
-        config (:class:`~mcli.models.run_config.RunConfig`): The
-            :class:`run configuration <mcli.models.run_config.RunConfig>` that was used to launch to the run
-
-        started_at (`Optional[datetime]`): Date and time when the run entered
-            the `STARTED` :class:`~mcli.utils.utils_run_status.RunStatus`
-        completed_at (`Optional[datetime]`): Date and time when the run entered
-            the `COMPLETED` :class:`~mcli.utils.utils_run_status.RunStatus`
+        created_by (`str`): Email of the user who created the run
+        priority (`str`): Priority of the run
+        preemptible (`bool`): Whether the run can be stopped and re-queued by higher priority jobs
+        retry_on_system_failure (`bool`): Whether the run should be retried on system failure
+        cluster (`str`): Cluster the run is running on
+        gpus (`int`): Number of GPUs the run is using
+        gpu_type (`str`): Type of GPU the run is using
+        cpus (`int`): Number of CPUs the run is using
+        node_count (`int`): Number of nodes the run is using
+        latest_resumption (:class:`~mcli.api.model.run.Resumption`): Latest resumption of the run
+        max_retries (`Optional[int]`): Maximum number of times the run can be retried
+        reason (`Optional[str]`): Reason the run was stopped
+        nodes (`List[:class:`~mcli.api.model.run.Node`]`): Nodes the run is using
+        submitted_config (`Optional[:class:`~mcli.models.run_config.RunConfig`]`): Submitted run configuration
+        metadata (`Optional[Dict[str, Any]]`): Metadata associated with the run
+        last_resumption_id (`Optional[str]`): ID of the last resumption of the run
+        resumptions (`List[:class:`~mcli.api.model.run.Resumption`]`): Resumptions of the run
+        lifecycle (`List[:class:`~mcli.api.model.run.RunLifecycle`]`): Lifecycle of the run
+        image (`Optional[str]`): Image the run is using
     """
 
     run_uid: str
     name: str
     status: RunStatus
     created_at: datetime
     updated_at: datetime
@@ -135,40 +147,78 @@
     gpus: int
     gpu_type: str
     cpus: int
     node_count: int
 
     latest_resumption: Resumption
     max_retries: Optional[int] = None
-    started_at: Optional[datetime] = None
-    completed_at: Optional[datetime] = None
     reason: Optional[str] = None
     nodes: List[Node] = field(default_factory=list)
     submitted_config: Optional[RunConfig] = None
     metadata: Optional[Dict[str, Any]] = None
     last_resumption_id: Optional[str] = None
     resumptions: List[Resumption] = field(default_factory=list)
     lifecycle: List[RunLifecycle] = field(default_factory=list)
     image: Optional[str] = None
 
     _required_properties: Tuple[str] = tuple([
         'id',
         'name',
         'status',
         'createdAt',
-        'completedAt',
         'updatedAt',
         'reason',
         'createdByEmail',
         'priority',
         'preemptible',
         'retryOnSystemFailure',
         'resumptions',
     ])
 
+    @property
+    def started_at(self) -> Optional[datetime]:
+        """The time the run was first started
+
+        If there are multiple resumptions, this will be the earliest start time
+        Started At will be None if the first resumption has not been started
+
+        Returns:
+            The time the run was first started
+        """
+        for resumption in self.resumptions:
+            if resumption.started_at:
+                return resumption.started_at
+
+        return None
+
+    @property
+    def completed_at(self) -> Optional[datetime]:
+        """The time the run was completed
+
+        If there are multiple resumptions, this will be the last end time
+        Completed At will be None if the last resumption has not been completed
+
+        Returns:
+            The time the run was last completed
+        """
+
+        for resumption in self.resumptions[:-1]:
+            if resumption.ended_at:
+                return resumption.ended_at
+
+            # Stopped resumptions are special: you can technically stop a resumption
+            # before it starts, resulting in a resumption with no start or end time.
+            # For these cases, use the previous resumption's end time (if it exists)
+
+            # Otherwise, if ended_at is None, the resumption is still running
+            if resumption.status != RunStatus.STOPPED:
+                return None
+
+        return None
+
     def _get_time_in_status(self, status: RunStatus) -> float:
         """Returns the time spent in a given status
 
         Args:
             status (:class:`~mcli.utils.utils_run_status.RunStatus`): The status to get the time for
 
         Returns:
@@ -376,31 +426,21 @@
         missing = set(cls._required_properties) - set(response)
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
                 message=f'Missing required key(s) in response to deserialize Run object: {", ".join(missing)}',
             )
 
-        started_at = None
-        if response['startedAt'] is not None:
-            started_at = convert_datetime(response['startedAt'])
-
-        completed_at = None
-        if response['completedAt'] is not None:
-            completed_at = convert_datetime(response['completedAt'])
-
         resumptions = [Resumption.from_mapi_response(r) for r in response['resumptions']]
         latest_resumption = resumptions[-1]
 
         args = {
             'run_uid': response['id'],
             'name': response['name'],
             'created_at': convert_datetime(response['createdAt']),
-            'started_at': started_at,
-            'completed_at': completed_at,
             'updated_at': convert_datetime(response['updatedAt']),
             'status': RunStatus.from_string(response['status']),
             'reason': response['reason'],
             'created_by': response['createdByEmail'],
             'priority': response['priority'],
             'max_retries': response.get('maxRetries'),
             'preemptible': response['preemptible'],
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/__init__.py` & `mosaicml-cli-0.5.4/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_create_interactive_run.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_create_interactive_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 mutation CreateInteractiveRun(${VARIABLE_DATA_NAME}: CreateInteractiveRunInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_create_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 mutation CreateRun(${VARIABLE_DATA_NAME}: CreateRunInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_delete_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 mutation DeleteRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_get_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
   {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
   runs {{
     id
     name
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
@@ -56,16 +54,14 @@
 query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
   {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
   runs {{
     id
     name
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_start_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 mutation StartRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_stop_runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 mutation StopRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_update_run.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_update_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 mutation UpdateRun(${VARIABLE_DATA_GET_RUNS}: GetRunsInput!, ${VARIABLE_DATA_UPDATE_RUN}: UpdateRunInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_GET_RUNS}: ${VARIABLE_DATA_GET_RUNS}, {VARIABLE_DATA_UPDATE_RUN}: ${VARIABLE_DATA_UPDATE_RUN}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_update_run_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 mutation UpdateRunMetadata(${VARIABLE_DATA_GET_RUNS}: GetRunsInput!, ${VARIABLE_DATA_UPDATE_RUN_METADATA}: UpdateRunMetadataInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_GET_RUNS}: ${VARIABLE_DATA_GET_RUNS}, {VARIABLE_DATA_UPDATE_RUN_METADATA}: ${VARIABLE_DATA_UPDATE_RUN_METADATA}) {{
     id
     name
     createdByEmail
     status
     createdAt
-    startedAt
-    completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     resumptions {{
```

### Comparing `mosaicml-cli-0.5.3/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.5.4/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.5.4/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.5.4/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.5.4/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.5.4/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/typing_future.py` & `mosaicml-cli-0.5.4/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.5.4/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/api/utils.py` & `mosaicml-cli-0.5.4/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/cli.py` & `mosaicml-cli-0.5.4/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.5.4/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.5.4/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.5.4/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.5.4/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.5.4/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.5.4/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.5.4/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.5.4/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_clusters.py` & `mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.5.4/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.5.4/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/display.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_get/users.py` & `mosaicml-cli-0.5.4/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.5.4/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.5.4/mcli/cli/m_interactive/m_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         help='Name for the interactive session. '
         'Default: "interactive-<gpu type>-<gpu num>"',
     )
 
     parser.add_argument(
         '--image',
         default='mosaicml/pytorch',
-        help='Docker image to use',
+        help='Docker image to use (default: %(default)s)',
     )
 
     parser.add_argument('--max-duration',
                         type=float,
                         help='The maximum time that a run should run for (in hours). If the run exceeds this '
                         'duration, it will be stopped.')
```

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.5.4/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.5.4/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.5.4/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.5.4/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.5.4/mcli/cli/m_log/m_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,16 +111,17 @@
             # replicated in `follow_run_logs`. We'll do that here for parity
             if line:
                 last_line = line
                 print(line, end='')
         return last_line, int(0)
 
 
-def _get_deployment_logs(deploy: InferenceDeployment, restart, failed) -> Tuple[Optional[str], int]:
-    log_lines = get_inference_deployment_logs(deploy, restart=restart, failed=failed)
+def _get_deployment_logs(deploy: InferenceDeployment, follow: bool, restart: Optional[int],
+                         failed: bool) -> Tuple[Optional[str], int]:
+    log_lines = get_inference_deployment_logs(deploy, restart=restart, failed=failed, follow=follow)
     last_line: Optional[str] = None
     for line in log_lines:
         # When using progress bars we randomly get newlines added. By default,
         # kubernetes does not return empty lines when streaming, which is
         # replicated in `follow_run_logs`. We'll do that here for parity
         if line:
             last_line = line
@@ -171,15 +172,15 @@
         last_line: Optional[str] = None
         #Have to check type to satisfy pyright
         if isinstance(submissions[0], Run):
             last_line, err = _get_run_logs(submissions[0], follow, rank, failed, resumption)
             if err == 1:
                 return 1
         elif isinstance(submissions[0], InferenceDeployment):
-            last_line, err = _get_deployment_logs(submissions[0], restart, failed)
+            last_line, err = _get_deployment_logs(submissions[0], follow, restart, failed)
             if err == 1:
                 return 1
 
         # Progress bars are weird. Let's add a final newline so that if the printing
         # ends on an incompleted progress bar, it isn't erased
         if last_line:
             print('', file=sys.stderr)
@@ -207,25 +208,40 @@
 
     submission_parser = parser.add_argument(
         'submission_name',
         metavar='DEPLOYMENT',
         help='The name of the inference deployment to fetch logs for.',
     )
     submission_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
+
     restart_grp = parser.add_mutually_exclusive_group()
     restart_grp.add_argument(
         '--restart',
         type=int,
         default=None,
         help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
     restart_grp.add_argument('--failed',
                              action='store_true',
                              dest='failed',
                              default=False,
                              help='Get the logs of the latest failed deployment')
+    follow_grp = parser.add_mutually_exclusive_group()
+    follow_grp.add_argument('--no-follow',
+                            action='store_false',
+                            dest='follow',
+                            default=False,
+                            help='Do not follow the logs of an in-progress deployment. '
+                            'Simply print any existing logs and exit. This is the default behavior.')
+    follow_grp.add_argument('-f',
+                            '--follow',
+                            action='store_true',
+                            dest='follow',
+                            default=False,
+                            help='Follow the logs of an in-progress deployment.')
+
     return parser
 
 
 def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.TRAINING))
     submimssion_name_parser = parser.add_argument(
         'submission_name',
```

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.5.4/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.5.4/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.5.4/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.5.4/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/organization.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/organization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.5.4/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.5.4/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_update/m_update.py` & `mosaicml-cli-0.5.4/mcli/cli/m_update/m_update.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.5.4/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_util/util.py` & `mosaicml-cli-0.5.4/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/cli/m_watchdog/m_watchdog.py` & `mosaicml-cli-0.5.4/mcli/cli/m_watchdog/m_watchdog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/config.py` & `mosaicml-cli-0.5.4/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/models/__init__.py` & `mosaicml-cli-0.5.4/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/models/gpu_type.py` & `mosaicml-cli-0.5.4/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.5.4/mcli/models/inference_deployment_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,19 @@
 
         return translated_config
 
 
 class BatchingConfigTranslation(Translation[BatchingConfig, Dict[str, Any]]):
     """Translate batching configs to and from MAPI"""
 
-    _property_translations = {'max_batch_size': 'maxBatchSize', 'max_timeout_ms': 'maxTimeoutMs'}
+    _property_translations = {
+        'max_batch_size': 'maxBatchSize',
+        'max_timeout_ms': 'maxTimeoutMs',
+        'max_queue_size': 'maxQueueSize'
+    }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> BatchingConfig:
         translated_config = {}
         for mcli_key, mapi_key in cls._property_translations.items():
             translated_config[mcli_key] = value.get(mapi_key)
```

### Comparing `mosaicml-cli-0.5.3/mcli/models/mcli_secret.py` & `mosaicml-cli-0.5.4/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/models/run_config.py` & `mosaicml-cli-0.5.4/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.5.4/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.5.4/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/sdk/__init__.py` & `mosaicml-cli-0.5.4/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_cli.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_completers.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_completers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_config.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_date.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_finetune.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_finetune.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_logging.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_model.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_rich.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_types.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.5.4/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mcli/version.py` & `mosaicml-cli-0.5.4/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.5.3'
+__version__ = '0.5.4'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.5.4/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.3
+Version: 0.5.4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.5.4/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.5.4/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 rich>=12.6.0
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 requests<3,>=2.26.0
 
 [all]
+sphinx-argparse==0.4.0
+pylint>=2.12.2
 sphinx-copybutton==0.5.2
-pytest-cov>=4.0.0
-pytest>=6.2.5
-radon>=5.1.0
 yapf>=0.33.0
-furo==2022.9.29
+isort>=5.9.3
 sphinx-rtd-theme==1.0.0
-sphinx-argparse==0.4.0
+sphinxemoji==0.2.0
+pytest>=6.2.5
+furo==2022.9.29
+sphinxcontrib-jsmath>=1.0.1
 sphinxcontrib-qthelp>=1.0.3
-sphinx-markdown-tables==0.0.17
-sphinxext-opengraph==0.8.2
+pytest-mock>=3.7.0
+pyright==1.1.256
+sphinxcontrib-applehelp>=1.0.2
+sphinx-panels==0.6.0
+sphinxcontrib-images>=0.9.4
 build>=0.10.0
-sphinxcontrib-devhelp>=1.0.2
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxemoji==0.2.0
 docutils>=0.17.0
-sphinx_external_toc==0.3.0
-sphinxcontrib-katex==0.9.4
-myst-parser>=0.16.1
-sphinxcontrib-images>=0.9.4
-pyright==1.1.256
-isort>=5.9.3
-pytest-mock>=3.7.0
+pre-commit>=2.17.0
+sphinxcontrib-devhelp>=1.0.2
+sphinx-markdown-tables==0.0.17
 sphinx==4.4.0
-sphinx-design
+sphinx_external_toc==0.3.0
 twine>=4.0.2
-sphinxcontrib-jsmath>=1.0.1
-sphinxcontrib-applehelp>=1.0.2
-toml>=0.10.2
+sphinxcontrib-katex==0.9.4
 sphinxcontrib-serializinghtml==1.1.5
-pre-commit>=2.17.0
-pylint>=2.12.2
-sphinx-panels==0.6.0
+pytest-cov>=4.0.0
+toml>=0.10.2
+sphinx-design
+sphinxext-opengraph==0.8.2
+myst-parser>=0.16.1
+radon>=5.1.0
+sphinxcontrib-htmlhelp>=2.0.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.5.3/pyproject.toml` & `mosaicml-cli-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/setup.py` & `mosaicml-cli-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/tests/test_config.py` & `mosaicml-cli-0.5.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.3/tests/test_upgrade.py` & `mosaicml-cli-0.5.4/tests/test_upgrade.py`

 * *Files identical despite different names*

