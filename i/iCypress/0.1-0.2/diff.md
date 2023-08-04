# Comparing `tmp/iCypress-0.1.tar.gz` & `tmp/iCypress-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iCypress-0.1.tar", last modified: Fri Aug  4 02:43:11 2023, max compression
+gzip compressed data, was "iCypress-0.2.tar", last modified: Fri Aug  4 04:41:31 2023, max compression
```

## Comparing `iCypress-0.1.tar` & `iCypress-0.2.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:10.779092 iCypress-0.1/
--rw-rw-rw-   0        0        0     1077 2023-08-04 02:24:55.000000 iCypress-0.1/LICENSE
--rw-rw-rw-   0        0        0      717 2023-08-04 02:43:10.780091 iCypress-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-08-04 01:58:34.000000 iCypress-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.785090 iCypress-0.1/graphgym/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/__init__.py
--rw-rw-rw-   0        0        0     2442 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/checkpoint.py
--rw-rw-rw-   0        0        0      955 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/cmd_args.py
--rw-rw-rw-   0        0        0    18756 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/config.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.788090 iCypress-0.1/graphgym/contrib/
--rw-rw-rw-   0        0        0      450 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.802101 iCypress-0.1/graphgym/contrib/act/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/act/__init__.py
--rw-rw-rw-   0        0        0      576 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/act/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.817617 iCypress-0.1/graphgym/contrib/config/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/config/__init__.py
--rw-rw-rw-   0        0        0      736 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/config/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.843621 iCypress-0.1/graphgym/contrib/feature_augment/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/feature_augment/__init__.py
--rw-rw-rw-   0        0        0      680 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/feature_augment/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.861618 iCypress-0.1/graphgym/contrib/feature_encoder/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/feature_encoder/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/feature_encoder/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.875621 iCypress-0.1/graphgym/contrib/head/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/head/__init__.py
--rw-rw-rw-   0        0        0      844 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/head/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.949146 iCypress-0.1/graphgym/contrib/layer/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/__init__.py
--rw-rw-rw-   0        0        0    24433 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/attconv.py
--rw-rw-rw-   0        0        0     3475 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/example.py
--rw-rw-rw-   0        0        0     9176 2023-05-31 18:32:46.000000 iCypress-0.1/graphgym/contrib/layer/generalconv.py
--rw-rw-rw-   0        0        0     5053 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/generalconv_ogb.py
--rw-rw-rw-   0        0        0    10967 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/generalconv_v2.py
--rw-rw-rw-   0        0        0    17970 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/idconv.py
--rw-rw-rw-   0        0        0     4468 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/layer/sageinitconv.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:05.967146 iCypress-0.1/graphgym/contrib/loader/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/loader/__init__.py
--rw-rw-rw-   0        0        0      487 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/loader/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.013671 iCypress-0.1/graphgym/contrib/loss/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/loss/__init__.py
--rw-rw-rw-   0        0        0      325 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/loss/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.067973 iCypress-0.1/graphgym/contrib/network/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/network/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/network/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.116194 iCypress-0.1/graphgym/contrib/optimizer/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/optimizer/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/optimizer/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.149196 iCypress-0.1/graphgym/contrib/pooling/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/pooling/__init__.py
--rw-rw-rw-   0        0        0      317 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/pooling/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.167194 iCypress-0.1/graphgym/contrib/stage/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/stage/__init__.py
--rw-rw-rw-   0        0        0      864 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/stage/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.200203 iCypress-0.1/graphgym/contrib/train/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/train/__init__.py
--rw-rw-rw-   0        0        0     2734 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/train/example.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:06.520314 iCypress-0.1/graphgym/contrib/transform/
--rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/transform/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/contrib/transform/identity.py
--rw-rw-rw-   0        0        0     1450 2023-07-26 03:23:22.000000 iCypress-0.1/graphgym/custom_dataset.py
--rw-rw-rw-   0        0        0      509 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/init.py
--rw-rw-rw-   0        0        0    10803 2023-07-27 17:30:25.000000 iCypress-0.1/graphgym/loader.py
--rw-rw-rw-   0        0        0    12164 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/loader_pyg.py
--rw-rw-rw-   0        0        0     8121 2023-06-13 02:59:57.000000 iCypress-0.1/graphgym/logger.py
--rw-rw-rw-   0        0        0     1490 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/loss.py
--rw-rw-rw-   0        0        0      986 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/model_builder.py
--rw-rw-rw-   0        0        0      948 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/model_builder_pyg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:07.720733 iCypress-0.1/graphgym/models/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/__init__.py
--rw-rw-rw-   0        0        0      558 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/act.py
--rw-rw-rw-   0        0        0    14518 2023-05-08 18:27:57.000000 iCypress-0.1/graphgym/models/feature_augment.py
--rw-rw-rw-   0        0        0     3709 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/feature_encoder.py
--rw-rw-rw-   0        0        0     3406 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/feature_encoder_pyg.py
--rw-rw-rw-   0        0        0     8435 2023-07-26 15:12:56.000000 iCypress-0.1/graphgym/models/gnn.py
--rw-rw-rw-   0        0        0     5177 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/gnn_pyg.py
--rw-rw-rw-   0        0        0     4918 2023-06-05 19:57:20.000000 iCypress-0.1/graphgym/models/head.py
--rw-rw-rw-   0        0        0     4571 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/head_pyg.py
--rw-rw-rw-   0        0        0     9202 2023-07-26 02:45:19.000000 iCypress-0.1/graphgym/models/layer.py
--rw-rw-rw-   0        0        0     8622 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/layer_pyg.py
--rw-rw-rw-   0        0        0     1502 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/pooling.py
--rw-rw-rw-   0        0        0     4594 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/models/transform.py
--rw-rw-rw-   0        0        0     2086 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/optimizer.py
--rw-rw-rw-   0        0        0     5458 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/register.py
--rw-rw-rw-   0        0        0     2936 2023-07-26 02:45:19.000000 iCypress-0.1/graphgym/train.py
--rw-rw-rw-   0        0        0     3064 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/train_pyg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:09.482513 iCypress-0.1/graphgym/utils/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/__init__.py
--rw-rw-rw-   0        0        0     9767 2023-07-26 02:45:19.000000 iCypress-0.1/graphgym/utils/agg_runs.py
--rw-rw-rw-   0        0        0     3120 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/comp_budget.py
--rw-rw-rw-   0        0        0     2776 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/device.py
--rw-rw-rw-   0        0        0      692 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/epoch.py
--rw-rw-rw-   0        0        0     2144 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/io.py
--rw-rw-rw-   0        0        0     1368 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/plot.py
--rw-rw-rw-   0        0        0      205 2023-03-25 16:28:28.000000 iCypress-0.1/graphgym/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:10.463282 iCypress-0.1/iCypress.egg-info/
--rw-rw-rw-   0        0        0      717 2023-08-04 02:43:04.000000 iCypress-0.1/iCypress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2536 2023-08-04 02:43:05.000000 iCypress-0.1/iCypress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:43:04.000000 iCypress-0.1/iCypress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-08-04 02:43:04.000000 iCypress-0.1/iCypress.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 02:43:04.000000 iCypress-0.1/iCypress.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 02:43:10.777092 iCypress-0.1/run/
--rw-rw-rw-   0        0        0      113 2023-08-04 01:58:21.000000 iCypress-0.1/run/Cypress.py
--rw-rw-rw-   0        0        0     9566 2023-07-26 04:54:01.000000 iCypress-0.1/run/CytokinesDataSet.py
--rw-rw-rw-   0        0        0     4644 2023-07-26 02:45:19.000000 iCypress-0.1/run/Visualization.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.1/run/__init__.py
--rw-rw-rw-   0        0        0      614 2023-03-25 16:28:28.000000 iCypress-0.1/run/agg_batch.py
--rw-rw-rw-   0        0        0    10352 2023-07-26 02:45:19.000000 iCypress-0.1/run/configs_gen.py
--rw-rw-rw-   0        0        0     6259 2023-07-31 05:23:57.000000 iCypress-0.1/run/main.py
--rw-rw-rw-   0        0        0     2158 2023-03-25 16:28:29.000000 iCypress-0.1/run/main_pyg.py
--rw-rw-rw-   0        0        0       86 2023-08-04 02:43:10.782094 iCypress-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1307 2023-08-04 02:33:36.000000 iCypress-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.964257 iCypress-0.2/
+-rw-rw-rw-   0        0        0     1077 2023-08-04 02:24:55.000000 iCypress-0.2/LICENSE
+-rw-rw-rw-   0        0        0      717 2023-08-04 04:41:30.964257 iCypress-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-08-04 01:58:34.000000 iCypress-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.810232 iCypress-0.2/graphgym/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/checkpoint.py
+-rw-rw-rw-   0        0        0      955 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/cmd_args.py
+-rw-rw-rw-   0        0        0    18756 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/config.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.810232 iCypress-0.2/graphgym/contrib/
+-rw-rw-rw-   0        0        0      450 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.838159 iCypress-0.2/graphgym/contrib/act/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/act/__init__.py
+-rw-rw-rw-   0        0        0      576 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/act/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.852174 iCypress-0.2/graphgym/contrib/config/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/config/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/config/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.871173 iCypress-0.2/graphgym/contrib/feature_augment/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/feature_augment/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/feature_augment/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.892174 iCypress-0.2/graphgym/contrib/feature_encoder/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/feature_encoder/__init__.py
+-rw-rw-rw-   0        0        0     1671 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/feature_encoder/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.898172 iCypress-0.2/graphgym/contrib/head/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/head/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/head/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.942704 iCypress-0.2/graphgym/contrib/layer/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/__init__.py
+-rw-rw-rw-   0        0        0    24433 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/attconv.py
+-rw-rw-rw-   0        0        0     3475 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/example.py
+-rw-rw-rw-   0        0        0     9176 2023-05-31 18:32:46.000000 iCypress-0.2/graphgym/contrib/layer/generalconv.py
+-rw-rw-rw-   0        0        0     5053 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/generalconv_ogb.py
+-rw-rw-rw-   0        0        0    10967 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/generalconv_v2.py
+-rw-rw-rw-   0        0        0    17970 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/idconv.py
+-rw-rw-rw-   0        0        0     4468 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/layer/sageinitconv.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.948702 iCypress-0.2/graphgym/contrib/loader/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/loader/__init__.py
+-rw-rw-rw-   0        0        0      487 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/loader/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.960701 iCypress-0.2/graphgym/contrib/loss/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/loss/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/loss/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.973703 iCypress-0.2/graphgym/contrib/network/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/network/__init__.py
+-rw-rw-rw-   0        0        0     2450 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/network/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.977702 iCypress-0.2/graphgym/contrib/optimizer/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/optimizer/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/optimizer/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.995703 iCypress-0.2/graphgym/contrib/pooling/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/pooling/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/pooling/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:29.998703 iCypress-0.2/graphgym/contrib/stage/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/stage/__init__.py
+-rw-rw-rw-   0        0        0      864 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/stage/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.007702 iCypress-0.2/graphgym/contrib/train/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/train/__init__.py
+-rw-rw-rw-   0        0        0     2734 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/train/example.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.076239 iCypress-0.2/graphgym/contrib/transform/
+-rw-rw-rw-   0        0        0      229 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/transform/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/contrib/transform/identity.py
+-rw-rw-rw-   0        0        0     1450 2023-07-26 03:23:22.000000 iCypress-0.2/graphgym/custom_dataset.py
+-rw-rw-rw-   0        0        0      509 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/init.py
+-rw-rw-rw-   0        0        0    10803 2023-07-27 17:30:25.000000 iCypress-0.2/graphgym/loader.py
+-rw-rw-rw-   0        0        0    12164 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/loader_pyg.py
+-rw-rw-rw-   0        0        0     8121 2023-06-13 02:59:57.000000 iCypress-0.2/graphgym/logger.py
+-rw-rw-rw-   0        0        0     1490 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/loss.py
+-rw-rw-rw-   0        0        0      986 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/model_builder.py
+-rw-rw-rw-   0        0        0      948 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/model_builder_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.217794 iCypress-0.2/graphgym/models/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/act.py
+-rw-rw-rw-   0        0        0    14518 2023-05-08 18:27:57.000000 iCypress-0.2/graphgym/models/feature_augment.py
+-rw-rw-rw-   0        0        0     3709 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/feature_encoder.py
+-rw-rw-rw-   0        0        0     3406 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/feature_encoder_pyg.py
+-rw-rw-rw-   0        0        0     8435 2023-07-26 15:12:56.000000 iCypress-0.2/graphgym/models/gnn.py
+-rw-rw-rw-   0        0        0     5177 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/gnn_pyg.py
+-rw-rw-rw-   0        0        0     4918 2023-06-05 19:57:20.000000 iCypress-0.2/graphgym/models/head.py
+-rw-rw-rw-   0        0        0     4571 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/head_pyg.py
+-rw-rw-rw-   0        0        0     9202 2023-07-26 02:45:19.000000 iCypress-0.2/graphgym/models/layer.py
+-rw-rw-rw-   0        0        0     8622 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/layer_pyg.py
+-rw-rw-rw-   0        0        0     1502 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/pooling.py
+-rw-rw-rw-   0        0        0     4594 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/models/transform.py
+-rw-rw-rw-   0        0        0     2086 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/optimizer.py
+-rw-rw-rw-   0        0        0     5458 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/register.py
+-rw-rw-rw-   0        0        0     2936 2023-07-26 02:45:19.000000 iCypress-0.2/graphgym/train.py
+-rw-rw-rw-   0        0        0     3064 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/train_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.279322 iCypress-0.2/graphgym/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/__init__.py
+-rw-rw-rw-   0        0        0     9767 2023-07-26 02:45:19.000000 iCypress-0.2/graphgym/utils/agg_runs.py
+-rw-rw-rw-   0        0        0     3120 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/comp_budget.py
+-rw-rw-rw-   0        0        0     2776 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/device.py
+-rw-rw-rw-   0        0        0      692 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/epoch.py
+-rw-rw-rw-   0        0        0     2144 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/io.py
+-rw-rw-rw-   0        0        0     1368 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/plot.py
+-rw-rw-rw-   0        0        0      205 2023-03-25 16:28:28.000000 iCypress-0.2/graphgym/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.372068 iCypress-0.2/iCYPRESS/
+-rw-rw-rw-   0        0        0      113 2023-08-04 01:58:21.000000 iCypress-0.2/iCYPRESS/Cypress.py
+-rw-rw-rw-   0        0        0     9566 2023-07-26 04:54:01.000000 iCypress-0.2/iCYPRESS/CytokinesDataSet.py
+-rw-rw-rw-   0        0        0     4644 2023-07-26 02:45:19.000000 iCypress-0.2/iCYPRESS/Visualization.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.2/iCYPRESS/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-03-25 16:28:28.000000 iCypress-0.2/iCYPRESS/agg_batch.py
+-rw-rw-rw-   0        0        0    10352 2023-07-26 02:45:19.000000 iCypress-0.2/iCYPRESS/configs_gen.py
+-rw-rw-rw-   0        0        0     6259 2023-07-31 05:23:57.000000 iCypress-0.2/iCYPRESS/main.py
+-rw-rw-rw-   0        0        0     2158 2023-03-25 16:28:29.000000 iCypress-0.2/iCYPRESS/main_pyg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:41:30.961258 iCypress-0.2/iCypress.egg-info/
+-rw-rw-rw-   0        0        0      717 2023-08-04 04:41:29.000000 iCypress-0.2/iCypress.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-08-04 04:41:29.000000 iCypress-0.2/iCypress.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:28:28.000000 iCypress-0.2/iCypress.egg-info/__init__.py
+-rw-rw-rw-   0        0        0        1 2023-08-04 04:41:29.000000 iCypress-0.2/iCypress.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-08-04 04:41:29.000000 iCypress-0.2/iCypress.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 04:41:29.000000 iCypress-0.2/iCypress.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-04 04:41:31.058793 iCypress-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2023-08-04 04:41:19.000000 iCypress-0.2/setup.py
```

### Comparing `iCypress-0.1/LICENSE` & `iCypress-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/PKG-INFO` & `iCypress-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCypress
-Version: 0.1
+Version: 0.2
 Summary: iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks
 Home-page: https://github.com/luciancahil/iCYPRESS
 Download-URL: https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz
 Author: royhe
 Author-email: royhe62@yahoo.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iCypress-0.1/graphgym/checkpoint.py` & `iCypress-0.2/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/cmd_args.py` & `iCypress-0.2/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/config.py` & `iCypress-0.2/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/act/example.py` & `iCypress-0.2/graphgym/contrib/act/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/config/example.py` & `iCypress-0.2/graphgym/contrib/config/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/feature_augment/example.py` & `iCypress-0.2/graphgym/contrib/feature_augment/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/feature_encoder/example.py` & `iCypress-0.2/graphgym/contrib/feature_encoder/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/head/example.py` & `iCypress-0.2/graphgym/contrib/head/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/attconv.py` & `iCypress-0.2/graphgym/contrib/layer/attconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/example.py` & `iCypress-0.2/graphgym/contrib/layer/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/generalconv.py` & `iCypress-0.2/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/generalconv_ogb.py` & `iCypress-0.2/graphgym/contrib/layer/generalconv_ogb.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/generalconv_v2.py` & `iCypress-0.2/graphgym/contrib/layer/generalconv_v2.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/idconv.py` & `iCypress-0.2/graphgym/contrib/layer/idconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/layer/sageinitconv.py` & `iCypress-0.2/graphgym/contrib/layer/sageinitconv.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/network/example.py` & `iCypress-0.2/graphgym/contrib/network/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/optimizer/example.py` & `iCypress-0.2/graphgym/contrib/optimizer/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/stage/example.py` & `iCypress-0.2/graphgym/contrib/stage/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/train/example.py` & `iCypress-0.2/graphgym/contrib/train/example.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/contrib/transform/identity.py` & `iCypress-0.2/graphgym/contrib/transform/identity.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/custom_dataset.py` & `iCypress-0.2/graphgym/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/loader.py` & `iCypress-0.2/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/loader_pyg.py` & `iCypress-0.2/graphgym/loader_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/logger.py` & `iCypress-0.2/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/loss.py` & `iCypress-0.2/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/model_builder.py` & `iCypress-0.2/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/model_builder_pyg.py` & `iCypress-0.2/graphgym/model_builder_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/act.py` & `iCypress-0.2/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/feature_augment.py` & `iCypress-0.2/graphgym/models/feature_augment.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/feature_encoder.py` & `iCypress-0.2/graphgym/models/feature_encoder.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/feature_encoder_pyg.py` & `iCypress-0.2/graphgym/models/feature_encoder_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/gnn.py` & `iCypress-0.2/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/gnn_pyg.py` & `iCypress-0.2/graphgym/models/gnn_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/head.py` & `iCypress-0.2/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/head_pyg.py` & `iCypress-0.2/graphgym/models/head_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/layer.py` & `iCypress-0.2/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/layer_pyg.py` & `iCypress-0.2/graphgym/models/layer_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/pooling.py` & `iCypress-0.2/graphgym/models/pooling.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/models/transform.py` & `iCypress-0.2/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/optimizer.py` & `iCypress-0.2/graphgym/optimizer.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/register.py` & `iCypress-0.2/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/train.py` & `iCypress-0.2/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/train_pyg.py` & `iCypress-0.2/graphgym/train_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/agg_runs.py` & `iCypress-0.2/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/comp_budget.py` & `iCypress-0.2/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/device.py` & `iCypress-0.2/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/epoch.py` & `iCypress-0.2/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/io.py` & `iCypress-0.2/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/graphgym/utils/plot.py` & `iCypress-0.2/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/iCypress.egg-info/PKG-INFO` & `iCypress-0.2/iCypress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iCypress
-Version: 0.1
+Version: 0.2
 Summary: iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks
 Home-page: https://github.com/luciancahil/iCYPRESS
 Download-URL: https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz
 Author: royhe
 Author-email: royhe62@yahoo.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iCypress-0.1/iCypress.egg-info/SOURCES.txt` & `iCypress-0.2/iCypress.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -70,20 +70,21 @@
 graphgym/utils/agg_runs.py
 graphgym/utils/comp_budget.py
 graphgym/utils/device.py
 graphgym/utils/epoch.py
 graphgym/utils/io.py
 graphgym/utils/plot.py
 graphgym/utils/tools.py
+iCYPRESS/Cypress.py
+iCYPRESS/CytokinesDataSet.py
+iCYPRESS/Visualization.py
+iCYPRESS/__init__.py
+iCYPRESS/agg_batch.py
+iCYPRESS/configs_gen.py
+iCYPRESS/main.py
+iCYPRESS/main_pyg.py
 iCypress.egg-info/PKG-INFO
 iCypress.egg-info/SOURCES.txt
+iCypress.egg-info/__init__.py
 iCypress.egg-info/dependency_links.txt
 iCypress.egg-info/requires.txt
-iCypress.egg-info/top_level.txt
-run/Cypress.py
-run/CytokinesDataSet.py
-run/Visualization.py
-run/__init__.py
-run/agg_batch.py
-run/configs_gen.py
-run/main.py
-run/main_pyg.py
+iCypress.egg-info/top_level.txt
```

### Comparing `iCypress-0.1/run/CytokinesDataSet.py` & `iCypress-0.2/iCYPRESS/CytokinesDataSet.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/run/Visualization.py` & `iCypress-0.2/iCYPRESS/Visualization.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/run/agg_batch.py` & `iCypress-0.2/iCYPRESS/agg_batch.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/run/configs_gen.py` & `iCypress-0.2/iCYPRESS/configs_gen.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/run/main.py` & `iCypress-0.2/iCYPRESS/main.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/run/main_pyg.py` & `iCypress-0.2/iCYPRESS/main_pyg.py`

 * *Files identical despite different names*

### Comparing `iCypress-0.1/setup.py` & `iCypress-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iCypress",
-    version="0.1",
+    version="0.2",
     author="royhe",
     author_email="royhe62@yahoo.ca",
     description="iCYPRESS: identifying CYtokine PREdictors of diSeaSe. A library that analyzes cytokines using Graph Neural Networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luciancahil/iCYPRESS",
     download_url = 'https://github.com/luciancahil/iCYPRESS/archive/refs/tags/v_01.tar.gz',    # I explain this later on
```

