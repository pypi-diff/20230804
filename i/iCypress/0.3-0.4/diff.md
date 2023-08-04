# Comparing `tmp/iCypress-0.3.tar.gz` & `tmp/iCypress-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iCypress-0.3.tar", last modified: Fri Aug  4 16:44:48 2023, max compression
+gzip compressed data, was "iCypress-0.4.tar", last modified: Fri Aug  4 17:37:10 2023, max compression
```

## Comparing `iCypress-0.3.tar` & `iCypress-0.4.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.590834 iCypress-0.3/
--rw-rw-rw-   0        0        0     1077 2023-08-04 02:24:55.000000 iCypress-0.3/LICENSE
--rw-rw-rw-   0        0        0      821 2023-08-04 16:44:48.591831 iCypress-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-08-04 05:58:40.000000 iCypress-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.012904 iCypress-0.3/graphgym/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/__init__.py
--rw-rw-rw-   0        0        0     2442 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/checkpoint.py
--rw-rw-rw-   0        0        0     1016 2023-08-04 15:52:56.000000 iCypress-0.3/graphgym/cmd_args.py
--rw-rw-rw-   0        0        0    18756 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/config.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.018913 iCypress-0.3/graphgym/contrib/
--rw-rw-rw-   0        0        0      450 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.034981 iCypress-0.3/graphgym/contrib/act/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/act/__init__.py
--rw-rw-rw-   0        0        0      576 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/act/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.060059 iCypress-0.3/graphgym/contrib/config/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/config/__init__.py
--rw-rw-rw-   0        0        0      736 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/config/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.183135 iCypress-0.3/graphgym/contrib/feature_augment/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/feature_augment/__init__.py
--rw-rw-rw-   0        0        0      680 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/feature_augment/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.335105 iCypress-0.3/graphgym/contrib/feature_encoder/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/feature_encoder/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/feature_encoder/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.410498 iCypress-0.3/graphgym/contrib/head/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/head/__init__.py
--rw-rw-rw-   0        0        0      844 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/head/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.646443 iCypress-0.3/graphgym/contrib/layer/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/__init__.py
--rw-rw-rw-   0        0        0    24433 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/attconv.py
--rw-rw-rw-   0        0        0     3475 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/example.py
--rw-rw-rw-   0        0        0     9176 2023-05-31 18:32:46.000000 iCypress-0.3/graphgym/contrib/layer/generalconv.py
--rw-rw-rw-   0        0        0     5053 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/generalconv_ogb.py
--rw-rw-rw-   0        0        0    10967 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/generalconv_v2.py
--rw-rw-rw-   0        0        0    17970 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/idconv.py
--rw-rw-rw-   0        0        0     4468 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/layer/sageinitconv.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.741026 iCypress-0.3/graphgym/contrib/loader/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/loader/__init__.py
--rw-rw-rw-   0        0        0      487 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/loader/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:42.983687 iCypress-0.3/graphgym/contrib/loss/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/loss/__init__.py
--rw-rw-rw-   0        0        0      325 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/loss/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.079551 iCypress-0.3/graphgym/contrib/network/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/network/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/network/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.173357 iCypress-0.3/graphgym/contrib/optimizer/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/optimizer/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/optimizer/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.447484 iCypress-0.3/graphgym/contrib/pooling/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/pooling/__init__.py
--rw-rw-rw-   0        0        0      317 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/pooling/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.777929 iCypress-0.3/graphgym/contrib/stage/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/stage/__init__.py
--rw-rw-rw-   0        0        0      864 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/stage/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.784978 iCypress-0.3/graphgym/contrib/train/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/train/__init__.py
--rw-rw-rw-   0        0        0     2734 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/train/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:43.932971 iCypress-0.3/graphgym/contrib/transform/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/transform/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/contrib/transform/identity.py
--rw-rw-rw-   0        0        0     1450 2023-07-26 03:23:22.000000 iCypress-0.3/graphgym/custom_dataset.py
--rw-rw-rw-   0        0        0      509 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/init.py
--rw-rw-rw-   0        0        0    10803 2023-07-27 17:30:25.000000 iCypress-0.3/graphgym/loader.py
--rw-rw-rw-   0        0        0    12164 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/loader_pyg.py
--rw-rw-rw-   0        0        0     8121 2023-06-13 02:59:57.000000 iCypress-0.3/graphgym/logger.py
--rw-rw-rw-   0        0        0     1490 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/loss.py
--rw-rw-rw-   0        0        0      986 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/model_builder.py
--rw-rw-rw-   0        0        0      948 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/model_builder_pyg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:45.881844 iCypress-0.3/graphgym/models/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/__init__.py
--rw-rw-rw-   0        0        0      558 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/act.py
--rw-rw-rw-   0        0        0    14518 2023-05-08 18:27:57.000000 iCypress-0.3/graphgym/models/feature_augment.py
--rw-rw-rw-   0        0        0     3709 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/feature_encoder.py
--rw-rw-rw-   0        0        0     3406 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/feature_encoder_pyg.py
--rw-rw-rw-   0        0        0     8435 2023-07-26 15:12:56.000000 iCypress-0.3/graphgym/models/gnn.py
--rw-rw-rw-   0        0        0     5177 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/gnn_pyg.py
--rw-rw-rw-   0        0        0     4918 2023-06-05 19:57:20.000000 iCypress-0.3/graphgym/models/head.py
--rw-rw-rw-   0        0        0     4571 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/head_pyg.py
--rw-rw-rw-   0        0        0     9202 2023-07-26 02:45:19.000000 iCypress-0.3/graphgym/models/layer.py
--rw-rw-rw-   0        0        0     8622 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/layer_pyg.py
--rw-rw-rw-   0        0        0     1502 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/pooling.py
--rw-rw-rw-   0        0        0     4594 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/models/transform.py
--rw-rw-rw-   0        0        0     2086 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/optimizer.py
--rw-rw-rw-   0        0        0     5458 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/register.py
--rw-rw-rw-   0        0        0     2936 2023-07-26 02:45:19.000000 iCypress-0.3/graphgym/train.py
--rw-rw-rw-   0        0        0     3064 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/train_pyg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:46.950523 iCypress-0.3/graphgym/utils/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/__init__.py
--rw-rw-rw-   0        0        0     9767 2023-07-26 02:45:19.000000 iCypress-0.3/graphgym/utils/agg_runs.py
--rw-rw-rw-   0        0        0     3120 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/comp_budget.py
--rw-rw-rw-   0        0        0     2776 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/device.py
--rw-rw-rw-   0        0        0      692 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/epoch.py
--rw-rw-rw-   0        0        0     2144 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/io.py
--rw-rw-rw-   0        0        0     1368 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/plot.py
--rw-rw-rw-   0        0        0      205 2023-03-25 16:28:28.000000 iCypress-0.3/graphgym/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.387896 iCypress-0.3/iCYPRESS/
--rw-rw-rw-   0        0        0     3330 2023-08-04 06:08:30.000000 iCypress-0.3/iCYPRESS/Cypress.py
--rw-rw-rw-   0        0        0     9566 2023-07-26 04:54:01.000000 iCypress-0.3/iCYPRESS/CytokinesDataSet.py
--rw-rw-rw-   0        0        0     4644 2023-07-26 02:45:19.000000 iCypress-0.3/iCYPRESS/Visualization.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/__init__.py
--rw-rw-rw-   0        0        0      614 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/agg_batch.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.514335 iCypress-0.3/iCYPRESS/configs/
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.632071 iCypress-0.3/iCYPRESS/configs/IDGNN/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/IDGNN/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.925528 iCypress-0.3/iCYPRESS/configs/design/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/design/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.927526 iCypress-0.3/iCYPRESS/configs/example_custom_grid_example_custom/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/example_custom_grid_example_custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.932039 iCypress-0.3/iCYPRESS/configs/example_grid_example/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/example_grid_example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.934065 iCypress-0.3/iCYPRESS/configs/pyg/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/configs/pyg/__init__.py
--rw-rw-rw-   0        0        0    10352 2023-07-26 02:45:19.000000 iCypress-0.3/iCYPRESS/configs_gen.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.936064 iCypress-0.3/iCYPRESS/datasets/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.938064 iCypress-0.3/iCYPRESS/grids/
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:47.942581 iCypress-0.3/iCYPRESS/grids/IDGNN/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/grids/IDGNN/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/grids/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.099588 iCypress-0.3/iCYPRESS/grids/design/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/grids/design/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.103098 iCypress-0.3/iCYPRESS/grids/pyg/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/grids/pyg/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-08-04 15:52:32.000000 iCypress-0.3/iCYPRESS/main.py
--rw-rw-rw-   0        0        0     2158 2023-03-25 16:28:29.000000 iCypress-0.3/iCYPRESS/main_pyg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.106125 iCypress-0.3/iCYPRESS/results/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/results/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.111125 iCypress-0.3/iCYPRESS/sample/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCYPRESS/sample/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:44:48.588834 iCypress-0.3/iCypress.egg-info/
--rw-rw-rw-   0        0        0      821 2023-08-04 16:44:40.000000 iCypress-0.3/iCypress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3065 2023-08-04 16:44:41.000000 iCypress-0.3/iCypress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.3/iCypress.egg-info/__init__.py
--rw-rw-rw-   0        0        0        1 2023-08-04 16:44:40.000000 iCypress-0.3/iCypress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-08-04 16:44:40.000000 iCypress-0.3/iCypress.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-04 16:44:40.000000 iCypress-0.3/iCypress.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-04 16:44:48.596370 iCypress-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1279 2023-08-04 16:33:32.000000 iCypress-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:09.275044 iCypress-0.4/
+-rw-rw-rw-   0        0        0     1077 2023-08-04 02:24:55.000000 iCypress-0.4/LICENSE
+-rw-rw-rw-   0        0        0      821 2023-08-04 17:37:09.277562 iCypress-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-08-04 05:58:40.000000 iCypress-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:56.673442 iCypress-0.4/graphgym/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/checkpoint.py
+-rw-rw-rw-   0        0        0     1016 2023-08-04 15:52:56.000000 iCypress-0.4/graphgym/cmd_args.py
+-rw-rw-rw-   0        0        0    18756 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/config.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:56.719966 iCypress-0.4/graphgym/contrib/
+-rw-rw-rw-   0        0        0      450 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:56.774986 iCypress-0.4/graphgym/contrib/act/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/act/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/act/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:56.993590 iCypress-0.4/graphgym/contrib/config/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/config/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/config/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:57.005591 iCypress-0.4/graphgym/contrib/feature_augment/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/feature_augment/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/feature_augment/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:57.010590 iCypress-0.4/graphgym/contrib/feature_encoder/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/feature_encoder/__init__.py
+-rw-rw-rw-   0        0        0     1671 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/feature_encoder/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:57.023592 iCypress-0.4/graphgym/contrib/head/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/head/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/head/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:57.472738 iCypress-0.4/graphgym/contrib/layer/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/__init__.py
+-rw-rw-rw-   0        0        0    24433 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/attconv.py
+-rw-rw-rw-   0        0        0     3475 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/example.py
+-rw-rw-rw-   0        0        0     9176 2023-05-31 18:32:46.000000 iCypress-0.4/graphgym/contrib/layer/generalconv.py
+-rw-rw-rw-   0        0        0     5053 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/generalconv_ogb.py
+-rw-rw-rw-   0        0        0    10967 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/generalconv_v2.py
+-rw-rw-rw-   0        0        0    17970 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/idconv.py
+-rw-rw-rw-   0        0        0     4468 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/layer/sageinitconv.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:57.807831 iCypress-0.4/graphgym/contrib/loader/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/loader/__init__.py
+-rw-rw-rw-   0        0        0      487 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/loader/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:58.427025 iCypress-0.4/graphgym/contrib/loss/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/loss/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/loss/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:58.434024 iCypress-0.4/graphgym/contrib/network/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/network/__init__.py
+-rw-rw-rw-   0        0        0     2450 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/network/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:58.639097 iCypress-0.4/graphgym/contrib/optimizer/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/optimizer/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/optimizer/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:59.102766 iCypress-0.4/graphgym/contrib/pooling/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/pooling/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/pooling/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:59.809507 iCypress-0.4/graphgym/contrib/stage/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/stage/__init__.py
+-rw-rw-rw-   0        0        0      864 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/stage/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:36:59.822506 iCypress-0.4/graphgym/contrib/train/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/train/__init__.py
+-rw-rw-rw-   0        0        0     2734 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/train/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:00.241663 iCypress-0.4/graphgym/contrib/transform/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/transform/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/contrib/transform/identity.py
+-rw-rw-rw-   0        0        0     1450 2023-07-26 03:23:22.000000 iCypress-0.4/graphgym/custom_dataset.py
+-rw-rw-rw-   0        0        0      509 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/init.py
+-rw-rw-rw-   0        0        0    10803 2023-07-27 17:30:25.000000 iCypress-0.4/graphgym/loader.py
+-rw-rw-rw-   0        0        0    12164 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/loader_pyg.py
+-rw-rw-rw-   0        0        0     8121 2023-06-13 02:59:57.000000 iCypress-0.4/graphgym/logger.py
+-rw-rw-rw-   0        0        0     1490 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/loss.py
+-rw-rw-rw-   0        0        0      986 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/model_builder.py
+-rw-rw-rw-   0        0        0      948 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/model_builder_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:05.124101 iCypress-0.4/graphgym/models/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/act.py
+-rw-rw-rw-   0        0        0    14518 2023-05-08 18:27:57.000000 iCypress-0.4/graphgym/models/feature_augment.py
+-rw-rw-rw-   0        0        0     3709 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/feature_encoder.py
+-rw-rw-rw-   0        0        0     3406 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/feature_encoder_pyg.py
+-rw-rw-rw-   0        0        0     8435 2023-07-26 15:12:56.000000 iCypress-0.4/graphgym/models/gnn.py
+-rw-rw-rw-   0        0        0     5177 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/gnn_pyg.py
+-rw-rw-rw-   0        0        0     4918 2023-06-05 19:57:20.000000 iCypress-0.4/graphgym/models/head.py
+-rw-rw-rw-   0        0        0     4571 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/head_pyg.py
+-rw-rw-rw-   0        0        0     9202 2023-07-26 02:45:19.000000 iCypress-0.4/graphgym/models/layer.py
+-rw-rw-rw-   0        0        0     8622 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/layer_pyg.py
+-rw-rw-rw-   0        0        0     1502 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/pooling.py
+-rw-rw-rw-   0        0        0     4594 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/models/transform.py
+-rw-rw-rw-   0        0        0     2086 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/optimizer.py
+-rw-rw-rw-   0        0        0     5458 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/register.py
+-rw-rw-rw-   0        0        0     2936 2023-07-26 02:45:19.000000 iCypress-0.4/graphgym/train.py
+-rw-rw-rw-   0        0        0     3064 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/train_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:06.067014 iCypress-0.4/graphgym/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/__init__.py
+-rw-rw-rw-   0        0        0     9767 2023-07-26 02:45:19.000000 iCypress-0.4/graphgym/utils/agg_runs.py
+-rw-rw-rw-   0        0        0     3120 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/comp_budget.py
+-rw-rw-rw-   0        0        0     2776 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/device.py
+-rw-rw-rw-   0        0        0      692 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/epoch.py
+-rw-rw-rw-   0        0        0     2144 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/io.py
+-rw-rw-rw-   0        0        0     1368 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/plot.py
+-rw-rw-rw-   0        0        0      205 2023-03-25 16:28:28.000000 iCypress-0.4/graphgym/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:06.992449 iCypress-0.4/iCYPRESS/
+-rw-rw-rw-   0        0        0     3330 2023-08-04 06:08:30.000000 iCypress-0.4/iCYPRESS/Cypress.py
+-rw-rw-rw-   0        0        0     9566 2023-07-26 04:54:01.000000 iCypress-0.4/iCYPRESS/CytokinesDataSet.py
+-rw-rw-rw-   0        0        0     4644 2023-07-26 02:45:19.000000 iCypress-0.4/iCYPRESS/Visualization.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/agg_batch.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.162685 iCypress-0.4/iCYPRESS/configs/
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.275074 iCypress-0.4/iCYPRESS/configs/IDGNN/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/IDGNN/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.418634 iCypress-0.4/iCYPRESS/configs/design/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/design/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-07-18 14:28:21.000000 iCypress-0.4/iCYPRESS/configs/example_custom.yaml
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.661505 iCypress-0.4/iCYPRESS/configs/example_custom_grid_example_custom/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/example_custom_grid_example_custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.662505 iCypress-0.4/iCYPRESS/configs/example_grid_example/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/example_grid_example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.667030 iCypress-0.4/iCYPRESS/configs/pyg/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/configs/pyg/__init__.py
+-rw-rw-rw-   0        0        0    10352 2023-07-26 02:45:19.000000 iCypress-0.4/iCYPRESS/configs_gen.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.671044 iCypress-0.4/iCYPRESS/datasets/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.673040 iCypress-0.4/iCYPRESS/grids/
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.675046 iCypress-0.4/iCYPRESS/grids/IDGNN/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/grids/IDGNN/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/grids/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:07.978231 iCypress-0.4/iCYPRESS/grids/design/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/grids/design/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:08.586766 iCypress-0.4/iCYPRESS/grids/pyg/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/grids/pyg/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-08-04 15:52:32.000000 iCypress-0.4/iCYPRESS/main.py
+-rw-rw-rw-   0        0        0     2158 2023-03-25 16:28:29.000000 iCypress-0.4/iCYPRESS/main_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:08.828518 iCypress-0.4/iCYPRESS/results/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/results/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:08.832545 iCypress-0.4/iCYPRESS/sample/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCYPRESS/sample/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:37:09.273046 iCypress-0.4/iCypress.egg-info/
+-rw-rw-rw-   0        0        0      821 2023-08-04 17:36:54.000000 iCypress-0.4/iCypress.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-08-04 17:36:54.000000 iCypress-0.4/iCypress.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.4/iCypress.egg-info/__init__.py
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:36:54.000000 iCypress-0.4/iCypress.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-08-04 17:36:54.000000 iCypress-0.4/iCypress.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 17:36:54.000000 iCypress-0.4/iCypress.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-04 17:37:09.943855 iCypress-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1344 2023-08-04 17:36:11.000000 iCypress-0.4/setup.py
```

### Comparing `iCypress-0.3/LICENSE` & `iCypress-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/PKG-INFO` & `iCypress-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCypress
-Version: 0.3
+Version: 0.4
 Summary: iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks
 Home-page: https://github.com/luciancahil/iCYPRESS
 Download-URL: https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz
 Author: royhe
 Author-email: royhe62@yahoo.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iCypress-0.3/graphgym/checkpoint.py` & `iCypress-0.4/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/cmd_args.py` & `iCypress-0.4/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/config.py` & `iCypress-0.4/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/act/example.py` & `iCypress-0.4/graphgym/contrib/act/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/config/example.py` & `iCypress-0.4/graphgym/contrib/config/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/feature_augment/example.py` & `iCypress-0.4/graphgym/contrib/feature_augment/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/feature_encoder/example.py` & `iCypress-0.4/graphgym/contrib/feature_encoder/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/head/example.py` & `iCypress-0.4/graphgym/contrib/head/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/attconv.py` & `iCypress-0.4/graphgym/contrib/layer/attconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/example.py` & `iCypress-0.4/graphgym/contrib/layer/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/generalconv.py` & `iCypress-0.4/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/generalconv_ogb.py` & `iCypress-0.4/graphgym/contrib/layer/generalconv_ogb.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/generalconv_v2.py` & `iCypress-0.4/graphgym/contrib/layer/generalconv_v2.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/idconv.py` & `iCypress-0.4/graphgym/contrib/layer/idconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/layer/sageinitconv.py` & `iCypress-0.4/graphgym/contrib/layer/sageinitconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/network/example.py` & `iCypress-0.4/graphgym/contrib/network/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/optimizer/example.py` & `iCypress-0.4/graphgym/contrib/optimizer/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/stage/example.py` & `iCypress-0.4/graphgym/contrib/stage/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/train/example.py` & `iCypress-0.4/graphgym/contrib/train/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/contrib/transform/identity.py` & `iCypress-0.4/graphgym/contrib/transform/identity.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/custom_dataset.py` & `iCypress-0.4/graphgym/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/loader.py` & `iCypress-0.4/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/loader_pyg.py` & `iCypress-0.4/graphgym/loader_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/logger.py` & `iCypress-0.4/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/loss.py` & `iCypress-0.4/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/model_builder.py` & `iCypress-0.4/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/model_builder_pyg.py` & `iCypress-0.4/graphgym/model_builder_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/act.py` & `iCypress-0.4/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/feature_augment.py` & `iCypress-0.4/graphgym/models/feature_augment.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/feature_encoder.py` & `iCypress-0.4/graphgym/models/feature_encoder.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/feature_encoder_pyg.py` & `iCypress-0.4/graphgym/models/feature_encoder_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/gnn.py` & `iCypress-0.4/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/gnn_pyg.py` & `iCypress-0.4/graphgym/models/gnn_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/head.py` & `iCypress-0.4/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/head_pyg.py` & `iCypress-0.4/graphgym/models/head_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/layer.py` & `iCypress-0.4/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/layer_pyg.py` & `iCypress-0.4/graphgym/models/layer_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/pooling.py` & `iCypress-0.4/graphgym/models/pooling.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/models/transform.py` & `iCypress-0.4/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/optimizer.py` & `iCypress-0.4/graphgym/optimizer.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/register.py` & `iCypress-0.4/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/train.py` & `iCypress-0.4/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/train_pyg.py` & `iCypress-0.4/graphgym/train_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/agg_runs.py` & `iCypress-0.4/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/comp_budget.py` & `iCypress-0.4/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/device.py` & `iCypress-0.4/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/epoch.py` & `iCypress-0.4/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/io.py` & `iCypress-0.4/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/graphgym/utils/plot.py` & `iCypress-0.4/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/Cypress.py` & `iCypress-0.4/iCYPRESS/Cypress.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/CytokinesDataSet.py` & `iCypress-0.4/iCYPRESS/CytokinesDataSet.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/Visualization.py` & `iCypress-0.4/iCYPRESS/Visualization.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/agg_batch.py` & `iCypress-0.4/iCYPRESS/agg_batch.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/configs_gen.py` & `iCypress-0.4/iCYPRESS/configs_gen.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/main.py` & `iCypress-0.4/iCYPRESS/main.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCYPRESS/main_pyg.py` & `iCypress-0.4/iCYPRESS/main_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.3/iCypress.egg-info/PKG-INFO` & `iCypress-0.4/iCypress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCypress
-Version: 0.3
+Version: 0.4
 Summary: iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks
 Home-page: https://github.com/luciancahil/iCYPRESS
 Download-URL: https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz
 Author: royhe
 Author-email: royhe62@yahoo.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iCypress-0.3/iCypress.egg-info/SOURCES.txt` & `iCypress-0.4/iCypress.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 iCYPRESS/Visualization.py
 iCYPRESS/__init__.py
 iCYPRESS/agg_batch.py
 iCYPRESS/configs_gen.py
 iCYPRESS/main.py
 iCYPRESS/main_pyg.py
 iCYPRESS/configs/__init__.py
+iCYPRESS/configs/example_custom.yaml
 iCYPRESS/configs/IDGNN/__init__.py
 iCYPRESS/configs/design/__init__.py
 iCYPRESS/configs/example_custom_grid_example_custom/__init__.py
 iCYPRESS/configs/example_grid_example/__init__.py
 iCYPRESS/configs/pyg/__init__.py
 iCYPRESS/datasets/__init__.py
 iCYPRESS/grids/__init__.py
```

### Comparing `iCypress-0.3/setup.py` & `iCypress-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iCypress",
-    version="0.3",
+    version="0.4",
     author="royhe",
+    package_data={'iCYPRESS': ['configs/example_custom.yaml']},
     author_email="royhe62@yahoo.ca",
     description="iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luciancahil/iCYPRESS",
     download_url = 'https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz', 
     packages=setuptools.find_packages(),
```

