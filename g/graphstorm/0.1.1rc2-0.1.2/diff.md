# Comparing `tmp/graphstorm-0.1.1rc2-py3-none-any.whl.zip` & `tmp/graphstorm-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,96 +1,102 @@
-Zip file size: 226887 bytes, number of entries: 94
--rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-22 00:23 graphstorm/__init__.py
--rw-rw-r--  2.0 unx    21084 b- defN 23-Jun-22 00:23 graphstorm/gsf.py
--rw-rw-r--  2.0 unx    13143 b- defN 23-Jun-22 00:23 graphstorm/utils.py
--rw-rw-r--  2.0 unx     1320 b- defN 23-Jun-22 00:23 graphstorm/config/__init__.py
--rw-rw-r--  2.0 unx    75206 b- defN 23-Jun-22 00:23 graphstorm/config/argument.py
--rw-rw-r--  2.0 unx     2164 b- defN 23-Jun-22 00:23 graphstorm/config/config.py
--rw-rw-r--  2.0 unx      989 b- defN 23-Jun-22 00:23 graphstorm/config/utils.py
--rw-rw-r--  2.0 unx      941 b- defN 23-Jun-22 00:23 graphstorm/data/__init__.py
--rw-rw-r--  2.0 unx      997 b- defN 23-Jun-22 00:23 graphstorm/data/constants.py
--rw-rw-r--  2.0 unx     3265 b- defN 23-Jun-22 00:23 graphstorm/data/dataset.py
--rw-rw-r--  2.0 unx     8270 b- defN 23-Jun-22 00:23 graphstorm/data/mag_lsc.py
--rw-rw-r--  2.0 unx    14665 b- defN 23-Jun-22 00:23 graphstorm/data/movielens.py
--rw-rw-r--  2.0 unx    11231 b- defN 23-Jun-22 00:23 graphstorm/data/ogbn_datasets.py
--rw-rw-r--  2.0 unx     9541 b- defN 23-Jun-22 00:23 graphstorm/data/ogbn_mag.py
--rw-rw-r--  2.0 unx     4907 b- defN 23-Jun-22 00:23 graphstorm/data/text_dataset.py
--rw-rw-r--  2.0 unx    10819 b- defN 23-Jun-22 00:23 graphstorm/data/utils.py
--rw-rw-r--  2.0 unx     1831 b- defN 23-Jun-22 00:23 graphstorm/dataloading/__init__.py
--rw-rw-r--  2.0 unx    28498 b- defN 23-Jun-22 00:23 graphstorm/dataloading/dataloading.py
--rw-rw-r--  2.0 unx    25845 b- defN 23-Jun-22 00:23 graphstorm/dataloading/dataset.py
--rw-rw-r--  2.0 unx     9483 b- defN 23-Jun-22 00:23 graphstorm/dataloading/sampler.py
--rw-rw-r--  2.0 unx     3145 b- defN 23-Jun-22 00:23 graphstorm/dataloading/utils.py
--rw-rw-r--  2.0 unx     1261 b- defN 23-Jun-22 00:23 graphstorm/eval/__init__.py
--rw-rw-r--  2.0 unx    13568 b- defN 23-Jun-22 00:23 graphstorm/eval/eval_func.py
--rw-rw-r--  2.0 unx    31913 b- defN 23-Jun-22 00:23 graphstorm/eval/evaluator.py
--rw-rw-r--  2.0 unx     9574 b- defN 23-Jun-22 00:23 graphstorm/eval/utils.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/__init__.py
--rw-rw-r--  2.0 unx    30122 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/construct_graph.py
--rw-rw-r--  2.0 unx    12338 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/file_io.py
--rw-rw-r--  2.0 unx     6619 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/id_map.py
--rw-rw-r--  2.0 unx    38750 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/transform.py
--rw-rw-r--  2.0 unx    17952 b- defN 23-Jun-22 00:23 graphstorm/gconstruct/utils.py
--rw-rw-r--  2.0 unx      769 b- defN 23-Jun-22 00:23 graphstorm/inference/__init__.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-22 00:23 graphstorm/inference/ep_infer.py
--rw-rw-r--  2.0 unx     3697 b- defN 23-Jun-22 00:23 graphstorm/inference/graphstorm_infer.py
--rw-rw-r--  2.0 unx     4155 b- defN 23-Jun-22 00:23 graphstorm/inference/lp_infer.py
--rw-rw-r--  2.0 unx     6446 b- defN 23-Jun-22 00:23 graphstorm/inference/np_infer.py
--rw-rw-r--  2.0 unx     1834 b- defN 23-Jun-22 00:23 graphstorm/model/__init__.py
--rw-rw-r--  2.0 unx    34792 b- defN 23-Jun-22 00:23 graphstorm/model/edge_decoder.py
--rw-rw-r--  2.0 unx     9963 b- defN 23-Jun-22 00:23 graphstorm/model/edge_gnn.py
--rw-rw-r--  2.0 unx    13433 b- defN 23-Jun-22 00:23 graphstorm/model/embed.py
--rw-rw-r--  2.0 unx    26383 b- defN 23-Jun-22 00:23 graphstorm/model/gnn.py
--rw-rw-r--  2.0 unx     5783 b- defN 23-Jun-22 00:23 graphstorm/model/gnn_encoder_base.py
--rw-rw-r--  2.0 unx     2573 b- defN 23-Jun-22 00:23 graphstorm/model/gs_layer.py
--rw-rw-r--  2.0 unx    17036 b- defN 23-Jun-22 00:23 graphstorm/model/lm_embed.py
--rw-rw-r--  2.0 unx     4830 b- defN 23-Jun-22 00:23 graphstorm/model/loss_func.py
--rw-rw-r--  2.0 unx     5718 b- defN 23-Jun-22 00:23 graphstorm/model/lp_gnn.py
--rw-rw-r--  2.0 unx     4502 b- defN 23-Jun-22 00:23 graphstorm/model/node_decoder.py
--rw-rw-r--  2.0 unx     9019 b- defN 23-Jun-22 00:23 graphstorm/model/node_gnn.py
--rw-rw-r--  2.0 unx     6096 b- defN 23-Jun-22 00:23 graphstorm/model/rgat_encoder.py
--rw-rw-r--  2.0 unx     7156 b- defN 23-Jun-22 00:23 graphstorm/model/rgcn_encoder.py
--rw-rw-r--  2.0 unx    32293 b- defN 23-Jun-22 00:23 graphstorm/model/utils.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Jun-22 00:23 graphstorm/model/lm_model/__init__.py
--rw-rw-r--  2.0 unx    11149 b- defN 23-Jun-22 00:23 graphstorm/model/lm_model/hf_bert.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-22 00:23 graphstorm/model/lm_model/lm_model.py
--rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-22 00:23 graphstorm/model/lm_model/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-22 00:23 graphstorm/run/__init__.py
--rw-rw-r--  2.0 unx     1648 b- defN 23-Jun-22 00:23 graphstorm/run/gs_edge_classification.py
--rw-rw-r--  2.0 unx     1640 b- defN 23-Jun-22 00:23 graphstorm/run/gs_edge_regression.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-22 00:23 graphstorm/run/gs_link_prediction.py
--rw-rw-r--  2.0 unx     1523 b- defN 23-Jun-22 00:23 graphstorm/run/gs_node_classification.py
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-22 00:23 graphstorm/run/gs_node_regression.py
--rw-rw-r--  2.0 unx    30523 b- defN 23-Jun-22 00:23 graphstorm/run/launch.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_ep/__init__.py
--rw-rw-r--  2.0 unx     4113 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_ep/ep_infer_gnn.py
--rw-rw-r--  2.0 unx     3950 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_ep/ep_infer_lm.py
--rw-rw-r--  2.0 unx     8075 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_ep/gsgnn_ep.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_ep/gsgnn_lm_ep.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_lp/__init__.py
--rw-rw-r--  2.0 unx     8422 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_lp/gsgnn_lm_lp.py
--rw-rw-r--  2.0 unx     8770 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_lp/gsgnn_lp.py
--rw-rw-r--  2.0 unx     3853 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_lp/lp_infer_gnn.py
--rw-rw-r--  2.0 unx     3833 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_lp/lp_infer_lm.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_np/__init__.py
--rw-rw-r--  2.0 unx     7002 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_np/gsgnn_np.py
--rw-rw-r--  2.0 unx     3781 b- defN 23-Jun-22 00:23 graphstorm/run/gsgnn_np/np_infer_gnn.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-22 00:23 graphstorm/sagemaker/__init__.py
--rw-rw-r--  2.0 unx    10664 b- defN 23-Jun-22 00:23 graphstorm/sagemaker/sagemaker_infer.py
--rw-rw-r--  2.0 unx     9046 b- defN 23-Jun-22 00:23 graphstorm/sagemaker/sagemaker_train.py
--rw-rw-r--  2.0 unx    10422 b- defN 23-Jun-22 00:23 graphstorm/sagemaker/utils.py
--rw-rw-r--  2.0 unx     1306 b- defN 23-Jun-22 00:23 graphstorm/tracker/__init__.py
--rw-rw-r--  2.0 unx     4370 b- defN 23-Jun-22 00:23 graphstorm/tracker/graphstorm_tracker.py
--rw-rw-r--  2.0 unx    10002 b- defN 23-Jun-22 00:23 graphstorm/tracker/sagemaker_tracker.py
--rw-rw-r--  2.0 unx      817 b- defN 23-Jun-22 00:23 graphstorm/trainer/__init__.py
--rw-rw-r--  2.0 unx    13648 b- defN 23-Jun-22 00:23 graphstorm/trainer/ep_trainer.py
--rw-rw-r--  2.0 unx    13436 b- defN 23-Jun-22 00:23 graphstorm/trainer/gsgnn_trainer.py
--rw-rw-r--  2.0 unx    12971 b- defN 23-Jun-22 00:23 graphstorm/trainer/lp_trainer.py
--rw-rw-r--  2.0 unx    13000 b- defN 23-Jun-22 00:23 graphstorm/trainer/np_trainer.py
--rw-rw-r--  2.0 unx    10142 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      208 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/METADATA
--rw-rw-r--  2.0 unx       67 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     8327 b- defN 23-Jun-22 00:23 graphstorm-0.1.1rc2.dist-info/RECORD
-94 files, 847707 bytes uncompressed, 213669 bytes compressed:  74.8%
+Zip file size: 252024 bytes, number of entries: 100
+-rw-rw-r--  2.0 unx     1030 b- defN 23-Aug-04 01:31 graphstorm/__init__.py
+-rw-rw-r--  2.0 unx    21690 b- defN 23-Aug-04 01:31 graphstorm/gsf.py
+-rw-rw-r--  2.0 unx    13370 b- defN 23-Aug-04 01:31 graphstorm/utils.py
+-rw-rw-r--  2.0 unx     1320 b- defN 23-Aug-04 01:31 graphstorm/config/__init__.py
+-rw-rw-r--  2.0 unx    81412 b- defN 23-Aug-04 01:31 graphstorm/config/argument.py
+-rw-rw-r--  2.0 unx     2164 b- defN 23-Aug-04 01:31 graphstorm/config/config.py
+-rw-rw-r--  2.0 unx      989 b- defN 23-Aug-04 01:31 graphstorm/config/utils.py
+-rw-rw-r--  2.0 unx      941 b- defN 23-Aug-04 01:31 graphstorm/data/__init__.py
+-rw-rw-r--  2.0 unx      997 b- defN 23-Aug-04 01:31 graphstorm/data/constants.py
+-rw-rw-r--  2.0 unx     3265 b- defN 23-Aug-04 01:31 graphstorm/data/dataset.py
+-rw-rw-r--  2.0 unx     8270 b- defN 23-Aug-04 01:31 graphstorm/data/mag_lsc.py
+-rw-rw-r--  2.0 unx    14665 b- defN 23-Aug-04 01:31 graphstorm/data/movielens.py
+-rw-rw-r--  2.0 unx    11231 b- defN 23-Aug-04 01:31 graphstorm/data/ogbn_datasets.py
+-rw-rw-r--  2.0 unx     9541 b- defN 23-Aug-04 01:31 graphstorm/data/ogbn_mag.py
+-rw-rw-r--  2.0 unx     4907 b- defN 23-Aug-04 01:31 graphstorm/data/text_dataset.py
+-rw-rw-r--  2.0 unx    10819 b- defN 23-Aug-04 01:31 graphstorm/data/utils.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Aug-04 01:31 graphstorm/dataloading/__init__.py
+-rw-rw-r--  2.0 unx    32504 b- defN 23-Aug-04 01:31 graphstorm/dataloading/dataloading.py
+-rw-rw-r--  2.0 unx    28233 b- defN 23-Aug-04 01:31 graphstorm/dataloading/dataset.py
+-rw-rw-r--  2.0 unx    15791 b- defN 23-Aug-04 01:31 graphstorm/dataloading/sampler.py
+-rw-rw-r--  2.0 unx     3097 b- defN 23-Aug-04 01:31 graphstorm/dataloading/utils.py
+-rw-rw-r--  2.0 unx     1261 b- defN 23-Aug-04 01:31 graphstorm/eval/__init__.py
+-rw-rw-r--  2.0 unx    14472 b- defN 23-Aug-04 01:31 graphstorm/eval/eval_func.py
+-rw-rw-r--  2.0 unx    32353 b- defN 23-Aug-04 01:31 graphstorm/eval/evaluator.py
+-rw-rw-r--  2.0 unx     9574 b- defN 23-Aug-04 01:31 graphstorm/eval/utils.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/__init__.py
+-rw-rw-r--  2.0 unx    32393 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/construct_graph.py
+-rw-rw-r--  2.0 unx    11781 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/file_io.py
+-rw-rw-r--  2.0 unx     7626 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/id_map.py
+-rw-rw-r--  2.0 unx    43616 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/transform.py
+-rw-rw-r--  2.0 unx    24737 b- defN 23-Aug-04 01:31 graphstorm/gconstruct/utils.py
+-rw-rw-r--  2.0 unx      769 b- defN 23-Aug-04 01:31 graphstorm/inference/__init__.py
+-rw-rw-r--  2.0 unx     5816 b- defN 23-Aug-04 01:31 graphstorm/inference/ep_infer.py
+-rw-rw-r--  2.0 unx     3533 b- defN 23-Aug-04 01:31 graphstorm/inference/graphstorm_infer.py
+-rw-rw-r--  2.0 unx     4074 b- defN 23-Aug-04 01:31 graphstorm/inference/lp_infer.py
+-rw-rw-r--  2.0 unx     6586 b- defN 23-Aug-04 01:31 graphstorm/inference/np_infer.py
+-rw-rw-r--  2.0 unx     1834 b- defN 23-Aug-04 01:31 graphstorm/model/__init__.py
+-rw-rw-r--  2.0 unx    34792 b- defN 23-Aug-04 01:31 graphstorm/model/edge_decoder.py
+-rw-rw-r--  2.0 unx    10215 b- defN 23-Aug-04 01:31 graphstorm/model/edge_gnn.py
+-rw-rw-r--  2.0 unx    14220 b- defN 23-Aug-04 01:31 graphstorm/model/embed.py
+-rw-rw-r--  2.0 unx    26383 b- defN 23-Aug-04 01:31 graphstorm/model/gnn.py
+-rw-rw-r--  2.0 unx     5982 b- defN 23-Aug-04 01:31 graphstorm/model/gnn_encoder_base.py
+-rw-rw-r--  2.0 unx     2573 b- defN 23-Aug-04 01:31 graphstorm/model/gs_layer.py
+-rw-rw-r--  2.0 unx    17036 b- defN 23-Aug-04 01:31 graphstorm/model/lm_embed.py
+-rw-rw-r--  2.0 unx     4830 b- defN 23-Aug-04 01:31 graphstorm/model/loss_func.py
+-rw-rw-r--  2.0 unx     5718 b- defN 23-Aug-04 01:31 graphstorm/model/lp_gnn.py
+-rw-rw-r--  2.0 unx     2385 b- defN 23-Aug-04 01:31 graphstorm/model/ngnn_mlp.py
+-rw-rw-r--  2.0 unx     4502 b- defN 23-Aug-04 01:31 graphstorm/model/node_decoder.py
+-rw-rw-r--  2.0 unx    13943 b- defN 23-Aug-04 01:31 graphstorm/model/node_glem.py
+-rw-rw-r--  2.0 unx     9425 b- defN 23-Aug-04 01:31 graphstorm/model/node_gnn.py
+-rw-rw-r--  2.0 unx     6901 b- defN 23-Aug-04 01:31 graphstorm/model/rgat_encoder.py
+-rw-rw-r--  2.0 unx     7944 b- defN 23-Aug-04 01:31 graphstorm/model/rgcn_encoder.py
+-rw-rw-r--  2.0 unx    32304 b- defN 23-Aug-04 01:31 graphstorm/model/utils.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-Aug-04 01:31 graphstorm/model/lm_model/__init__.py
+-rw-rw-r--  2.0 unx    11149 b- defN 23-Aug-04 01:31 graphstorm/model/lm_model/hf_bert.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Aug-04 01:31 graphstorm/model/lm_model/lm_model.py
+-rw-rw-r--  2.0 unx     2294 b- defN 23-Aug-04 01:31 graphstorm/model/lm_model/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-04 01:31 graphstorm/run/__init__.py
+-rw-rw-r--  2.0 unx     1648 b- defN 23-Aug-04 01:31 graphstorm/run/gs_edge_classification.py
+-rw-rw-r--  2.0 unx     1640 b- defN 23-Aug-04 01:31 graphstorm/run/gs_edge_regression.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Aug-04 01:31 graphstorm/run/gs_link_prediction.py
+-rw-rw-r--  2.0 unx     1523 b- defN 23-Aug-04 01:31 graphstorm/run/gs_node_classification.py
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Aug-04 01:31 graphstorm/run/gs_node_regression.py
+-rw-rw-r--  2.0 unx    31201 b- defN 23-Aug-04 01:31 graphstorm/run/launch.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_ep/__init__.py
+-rw-rw-r--  2.0 unx     4631 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_ep/ep_infer_gnn.py
+-rw-rw-r--  2.0 unx     3990 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_ep/ep_infer_lm.py
+-rw-rw-r--  2.0 unx     8118 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_ep/gsgnn_ep.py
+-rw-rw-r--  2.0 unx     7135 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_ep/gsgnn_lm_ep.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_lp/__init__.py
+-rw-rw-r--  2.0 unx     8610 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_lp/gsgnn_lm_lp.py
+-rw-rw-r--  2.0 unx    10098 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_lp/gsgnn_lp.py
+-rw-rw-r--  2.0 unx     4157 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_lp/lp_infer_gnn.py
+-rw-rw-r--  2.0 unx     4025 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_lp/lp_infer_lm.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_np/__init__.py
+-rw-rw-r--  2.0 unx     7293 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_np/gsgnn_np.py
+-rw-rw-r--  2.0 unx     4299 b- defN 23-Aug-04 01:31 graphstorm/run/gsgnn_np/np_infer_gnn.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/__init__.py
+-rw-rw-r--  2.0 unx     9144 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/partition_algorithm.py
+-rw-rw-r--  2.0 unx     1939 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/s3_utils.py
+-rw-rw-r--  2.0 unx    10790 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/sagemaker_infer.py
+-rw-rw-r--  2.0 unx    14911 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/sagemaker_partition.py
+-rw-rw-r--  2.0 unx     9127 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/sagemaker_train.py
+-rw-rw-r--  2.0 unx    12568 b- defN 23-Aug-04 01:31 graphstorm/sagemaker/utils.py
+-rw-rw-r--  2.0 unx     1306 b- defN 23-Aug-04 01:31 graphstorm/tracker/__init__.py
+-rw-rw-r--  2.0 unx     4370 b- defN 23-Aug-04 01:31 graphstorm/tracker/graphstorm_tracker.py
+-rw-rw-r--  2.0 unx    10152 b- defN 23-Aug-04 01:31 graphstorm/tracker/sagemaker_tracker.py
+-rw-rw-r--  2.0 unx      872 b- defN 23-Aug-04 01:31 graphstorm/trainer/__init__.py
+-rw-rw-r--  2.0 unx    14072 b- defN 23-Aug-04 01:31 graphstorm/trainer/ep_trainer.py
+-rw-rw-r--  2.0 unx    10396 b- defN 23-Aug-04 01:31 graphstorm/trainer/glem_np_trainer.py
+-rw-rw-r--  2.0 unx    13255 b- defN 23-Aug-04 01:31 graphstorm/trainer/gsgnn_trainer.py
+-rw-rw-r--  2.0 unx    13092 b- defN 23-Aug-04 01:31 graphstorm/trainer/lp_trainer.py
+-rw-rw-r--  2.0 unx    13422 b- defN 23-Aug-04 01:31 graphstorm/trainer/np_trainer.py
+-rw-rw-r--  2.0 unx    10142 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      384 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       67 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     8866 b- defN 23-Aug-04 01:31 graphstorm-0.1.2.dist-info/RECORD
+100 files, 947778 bytes uncompressed, 237968 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -132,17 +132,23 @@
 
 Filename: graphstorm/model/loss_func.py
 Comment: 
 
 Filename: graphstorm/model/lp_gnn.py
 Comment: 
 
+Filename: graphstorm/model/ngnn_mlp.py
+Comment: 
+
 Filename: graphstorm/model/node_decoder.py
 Comment: 
 
+Filename: graphstorm/model/node_glem.py
+Comment: 
+
 Filename: graphstorm/model/node_gnn.py
 Comment: 
 
 Filename: graphstorm/model/rgat_encoder.py
 Comment: 
 
 Filename: graphstorm/model/rgcn_encoder.py
@@ -222,17 +228,26 @@
 
 Filename: graphstorm/run/gsgnn_np/np_infer_gnn.py
 Comment: 
 
 Filename: graphstorm/sagemaker/__init__.py
 Comment: 
 
+Filename: graphstorm/sagemaker/partition_algorithm.py
+Comment: 
+
+Filename: graphstorm/sagemaker/s3_utils.py
+Comment: 
+
 Filename: graphstorm/sagemaker/sagemaker_infer.py
 Comment: 
 
+Filename: graphstorm/sagemaker/sagemaker_partition.py
+Comment: 
+
 Filename: graphstorm/sagemaker/sagemaker_train.py
 Comment: 
 
 Filename: graphstorm/sagemaker/utils.py
 Comment: 
 
 Filename: graphstorm/tracker/__init__.py
@@ -246,38 +261,41 @@
 
 Filename: graphstorm/trainer/__init__.py
 Comment: 
 
 Filename: graphstorm/trainer/ep_trainer.py
 Comment: 
 
+Filename: graphstorm/trainer/glem_np_trainer.py
+Comment: 
+
 Filename: graphstorm/trainer/gsgnn_trainer.py
 Comment: 
 
 Filename: graphstorm/trainer/lp_trainer.py
 Comment: 
 
 Filename: graphstorm/trainer/np_trainer.py
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/LICENSE
+Filename: graphstorm-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/METADATA
+Filename: graphstorm-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/NOTICE
+Filename: graphstorm-0.1.2.dist-info/NOTICE
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/WHEEL
+Filename: graphstorm-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/top_level.txt
+Filename: graphstorm-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/zip-safe
+Filename: graphstorm-0.1.2.dist-info/zip-safe
 Comment: 
 
-Filename: graphstorm-0.1.1rc2.dist-info/RECORD
+Filename: graphstorm-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## graphstorm/__init__.py

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Graphstorm package.
 """
-__version__ = "0.1.1rc2"
+__version__ = "0.1.2"
 
 from .utils import get_rank
 from .gsf import initialize, get_feat_size
 from .gsf import create_builtin_node_gnn_model
 from .gsf import create_builtin_edge_gnn_model
 from .gsf import create_builtin_task_tracker
 from .gsf import create_builtin_lp_gnn_model
```

## graphstorm/gsf.py

```diff
@@ -29,14 +29,15 @@
 from .config import BUILTIN_LP_DOT_DECODER
 from .config import BUILTIN_LP_DISTMULT_DECODER
 from .model.embed import GSNodeEncoderInputLayer
 from .model.lm_embed import GSLMNodeEncoderInputLayer, GSPureLMNodeInputLayer
 from .model.rgcn_encoder import RelationalGCNEncoder
 from .model.rgat_encoder import RelationalGATEncoder
 from .model.node_gnn import GSgnnNodeModel
+from .model.node_glem import GLEM
 from .model.edge_gnn import GSgnnEdgeModel
 from .model.lp_gnn import GSgnnLinkPredictionModel
 from .model.loss_func import (ClassifyLossFunc,
                               RegressionLossFunc,
                               LinkPredictLossFunc,
                               WeightedLinkPredictLossFunc)
 from .model.node_decoder import EntityClassifier, EntityRegression
@@ -58,14 +59,15 @@
         File path of ip_config file
     backend: str
         Torch distributed backend
     """
     # We need to use socket for communication in DGL 0.8. The tensorpipe backend has a bug.
     # This problem will be fixed in the future.
     dgl.distributed.initialize(ip_config, net_type='socket')
+    assert th.cuda.is_available() or backend == "gloo", "Gloo backend required for a CPU setting."
     th.distributed.init_process_group(backend=backend)
     sys_tracker.check("load DistDGL")
 
 def get_feat_size(g, node_feat_names):
     """ Get the feature's size on each node type in the input graph.
 
     Parameters
@@ -146,15 +148,18 @@
     train_task : bool
         Whether this model is used for training.
 
     Returns
     -------
     GSgnnModel : The GNN model.
     """
-    model = GSgnnNodeModel(config.alpha_l2norm)
+    if config.training_method["name"] == "glem":
+        model = GLEM(config.alpha_l2norm, **config.training_method["kwargs"])
+    elif config.training_method["name"] == "default":
+        model = GSgnnNodeModel(config.alpha_l2norm)
     set_encoder(model, g, config, train_task)
 
     if config.task_type == BUILTIN_TASK_NODE_CLASSIFICATION:
         model.set_decoder(EntityClassifier(model.gnn_encoder.out_dims \
                                             if model.gnn_encoder is not None \
                                             else model.node_input_encoder.out_dims,
                                            config.num_classes,
@@ -436,15 +441,16 @@
                                                 num_train=config.lm_train_nodes,
                                                 lm_infer_batch_size=config.lm_infer_batch_size,
                                                 dropout=config.dropout,
                                                 use_node_embeddings=config.use_node_embeddings)
     else:
         encoder = GSNodeEncoderInputLayer(g, feat_size, config.hidden_size,
                                           dropout=config.dropout,
-                                          use_node_embeddings=config.use_node_embeddings)
+                                          use_node_embeddings=config.use_node_embeddings,
+                                          num_ffn_layers_in_input=config.num_ffn_layers_in_input)
     model.set_node_input_encoder(encoder)
 
     # Set GNN encoders
     dropout = config.dropout if train_task else 0
     if model_encoder_type == "mlp" or model_encoder_type == "lm":
         # Only input encoder is used
         assert config.num_layers == 0, "No GNN layers"
@@ -454,24 +460,26 @@
         # we need to set the num_layers -1 because there is an output layer
         # that is hard coded.
         gnn_encoder = RelationalGCNEncoder(g,
                                            config.hidden_size, config.hidden_size,
                                            num_bases=num_bases,
                                            num_hidden_layers=config.num_layers -1,
                                            dropout=dropout,
-                                           use_self_loop=config.use_self_loop)
+                                           use_self_loop=config.use_self_loop,
+                                           num_ffn_layers_in_gnn=config.num_ffn_layers_in_gnn)
     elif model_encoder_type == "rgat":
         # we need to set the num_layers -1 because there is an output layer that is hard coded.
         gnn_encoder = RelationalGATEncoder(g,
                                            config.hidden_size,
                                            config.hidden_size,
                                            config.num_heads,
                                            num_hidden_layers=config.num_layers -1,
                                            dropout=dropout,
-                                           use_self_loop=config.use_self_loop)
+                                           use_self_loop=config.use_self_loop,
+                                           num_ffn_layers_in_gnn=config.num_ffn_layers_in_gnn)
     else:
         assert False, "Unknown gnn model type {}".format(model_encoder_type)
     model.set_gnn_encoder(gnn_encoder)
 
 def create_builtin_task_tracker(config, rank):
     tracker_class = get_task_tracker_class(config.task_tracker)
     return tracker_class(config, rank)
```

## graphstorm/utils.py

```diff
@@ -25,14 +25,25 @@
 import pandas as pd
 import dgl
 import torch as th
 import numpy as np
 
 TORCH_MAJOR_VER = int(th.__version__.split('.', maxsplit=1)[0])
 
+def setup_device(local_rank):
+    """Setup computation device
+    """
+    if th.cuda.is_available():
+        device = 'cuda:%d' % local_rank
+        th.cuda.set_device(device)
+    else:
+        device='cpu'
+
+    return device
+
 def get_rank():
     """ Get rank of a process
     """
     try:
         return th.distributed.get_rank()
     except RuntimeError:
         # If Pytorch distributed is not set up correctly, we should set
```

## graphstorm/config/argument.py

```diff
@@ -199,28 +199,149 @@
                 if arg_key == "save_prediction_path" and arg_val.lower() == "none":
                     arg_val = None
 
                 # for basic attributes
                 setattr(self, f"_{arg_key}", arg_val)
                 print(f"Overriding Argument: {arg_key}")
 
+    def verify_arguments(self, is_train):
+        """ Verify the correctness of arguments.
+
+        Parameters
+        ----------
+        is_train : bool
+            Whether this is for training.
+        """
+        # Trigger the checks in the arguments.
+        _ = self.save_perf_results_path
+        _ = self.profile_path
+        _ = self.graph_name
+        _ = self.backend
+        _ = self.ip_config
+        _ = self.part_config
+        _ = self.node_id_mapping_file
+        _ = self.edge_id_mapping_file
+        _ = self.verbose
+
+        # Data
+        _ = self.node_feat_name
+        _ = self.decoder_edge_feat
+
+        # Evaluation
+        _ = self.eval_fanout
+        _ = self.use_mini_batch_infer
+        _ = self.eval_batch_size
+        _ = self.eval_frequency
+        _ = self.no_validation
+        _ = self.save_prediction_path
+        _ = self.eval_etype
+        if self.task_type is not None:
+            _ = self.eval_metric
+
+        # Model training.
+        if is_train:
+            _ = self.batch_size
+            _ = self.fanout
+            _ = self.lm_train_nodes
+            _ = self.lm_tune_lr
+            _ = self.lr
+            _ = self.sparse_optimizer_lr
+            _ = self.num_epochs
+            _ = self.save_model_path
+            _ = self.save_model_frequency
+            _ = self.topk_model_to_save
+            _ = self.early_stop_burnin_rounds
+            _ = self.early_stop_rounds
+            _ = self.early_stop_strategy
+            _ = self.use_early_stop
+            _ = self.wd_l2norm
+            _ = self.train_negative_sampler
+            _ = self.train_etype
+            _ = self.remove_target_edge_type
+
+        # LM module
+        if self.node_lm_configs:
+            _ = self.lm_infer_batch_size
+            _ = self.freeze_lm_encoder_epochs
+
+        # I/O related
+        _ = self.restore_model_layers
+        _ = self.restore_model_path
+        _ = self.restore_optimizer_path
+        _ = self.save_embed_path
+
+        # Model architecture
+        _ = self.dropout
+        _ = self.decoder_type
+        _ = self.num_decoder_basis
+        # Encoder related
+        encoder_type = self.model_encoder_type
+        if encoder_type == "lm":
+            assert self.node_lm_configs is not None
+        else:
+            _ = self.hidden_size
+            _ = self.num_layers
+            _ = self.use_self_loop
+            _ = self.use_node_embeddings
+            _ = self.num_bases
+            _ = self.num_heads
+
+        _ = self.return_proba
+        _ = self.alpha_l2norm
+
+        # Logging.
+        _ = self.task_tracker
+        _ = self.log_report_frequency
+
+        _ = self.task_type
+        # For classification tasks.
+        if self.task_type in [BUILTIN_TASK_NODE_CLASSIFICATION, BUILTIN_TASK_EDGE_CLASSIFICATION]:
+            _ = self.label_field
+            _ = self.num_classes
+            _ = self.multilabel
+            _ = self.multilabel_weights
+            _ = self.imbalance_class_weights
+        if self.task_type in [BUILTIN_TASK_NODE_CLASSIFICATION, BUILTIN_TASK_NODE_REGRESSION]:
+            _ = self.target_ntype
+        if self.task_type in [BUILTIN_TASK_EDGE_CLASSIFICATION, BUILTIN_TASK_EDGE_REGRESSION]:
+            _ = self.target_etype
+        if self.task_type in [BUILTIN_TASK_EDGE_CLASSIFICATION, BUILTIN_TASK_EDGE_REGRESSION,
+                              BUILTIN_TASK_LINK_PREDICTION] and is_train:
+            _ = self.exclude_training_targets
+            _ = self.reverse_edge_types_map
+        if self.task_type == BUILTIN_TASK_LINK_PREDICTION:
+            _ = self.gamma
+            _ = self.lp_decoder_type
+            _ = self.lp_edge_weight_for_loss
+            _ = self.lp_loss_func
+            _ = self.num_negative_edges
+            _ = self.eval_negative_sampler
+            _ = self.num_negative_edges_eval
+
+    def _turn_off_gradient_checkpoint(self, reason):
+        """Turn off `gradient_checkpoint` flags in `node_lm_configs`
+        """
+        for i, _ in enumerate(self.node_lm_configs):
+            if self.node_lm_configs[i]["gradient_checkpoint"]:
+                print(f"WARNING: {reason} can not work with " \
+                        "gradient checkpoint. Turn gradient checkpoint to False")
+                self.node_lm_configs[i]["gradient_checkpoint"] = False
+
     def handle_argument_conflicts(self):
         """Check and resolve argument conflicts
         """
         # 1. language model conflicts
         if self.node_lm_configs is not None:
             # gradient checkpoint does not work with freeze_lm_encoder_epochs
             # When freeze_lm_encoder_epochs is set, turn off gradient checkpoint
             if self.freeze_lm_encoder_epochs > 0:
-                for i, _ in enumerate(self.node_lm_configs):
-                    if self.node_lm_configs[i]["gradient_checkpoint"]:
-                        print("WARNING: freeze_lm_encoder_epochs can not work with " \
-                              "gradient checkpoint. Turn gradient checkpoint to False")
-                        self.node_lm_configs[i]["gradient_checkpoint"] = False
-
+                self._turn_off_gradient_checkpoint("freeze_lm_encoder_epochs")
+            # GLEM fine-tuning of LM conflicts with gradient checkpoint
+            if self.training_method["name"] == "glem":
+                self._turn_off_gradient_checkpoint("GLEM model")
         # TODO(xiangsx): Add more check
 
     ###################### Environment Info ######################
     @property
     def save_perf_results_path(self):
         """ Save performance flag
         """
@@ -382,14 +503,33 @@
                 "Encoder type lm (language model) and mlp (encoder layer only) " \
                 "do not work with language model warmup. It will cause torch " \
                 "DDP error"
             return self._freeze_lm_encoder_epochs
 
         return 0
 
+    @property
+    def training_method(self):
+        """ Setting up the LM/GNN co-training method
+        """
+        if hasattr(self, "_training_method"):
+            training_method_name = self._training_method["name"]
+            assert training_method_name in ("default", "glem"),\
+                f"Training method {training_method_name} is unavailable"
+            if training_method_name == "glem":
+                glem_defaults = {
+                    "em_order_gnn_first": False,
+                    "inference_using_gnn": True,
+                    "pl_weight": 0.5
+                }
+                for key, val in glem_defaults.items():
+                    self._training_method["kwargs"].setdefault(key, val)
+            return self._training_method
+        return {"name": "default", "kwargs": {}}
+
     def _check_lm_config(self, lm_config):
         assert "lm_type" in lm_config, "lm_type (type of language model," \
             "e.g., bert) must be provided for node_lm_models."
         assert "model_name" in lm_config, "language model model_name must " \
             "be provided for node_lm_models."
         if "gradient_checkpoint" not in lm_config:
             lm_config["gradient_checkpoint"] = False
@@ -455,17 +595,16 @@
 
             for feat_name in feat_names:
                 feat_info = feat_name.split(":")
                 assert len(feat_info) == 2, \
                         f"Unknown format of the feature name: {feat_name}, " + \
                         "must be NODE_TYPE:FEAT_NAME"
                 ntype = feat_info[0]
-                if ntype in fname_dict:
-                    assert False, \
-                        f"You already specify the feature names of {ntype}" \
+                assert ntype not in fname_dict, \
+                        f"You already specify the feature names of {ntype} " \
                         f"as {fname_dict[ntype]}"
                 assert isinstance(feat_info[1], str), \
                     f"Feature name of {ntype} should be a string not {feat_info[1]}"
                 # multiple features separated by ','
                 fname_dict[ntype] = feat_info[1].split(",")
             return fname_dict
 
@@ -500,19 +639,21 @@
         return fanout
 
     @property
     def fanout(self):
         """ training fanout
         """
         # pylint: disable=no-member
-        assert hasattr(self, "_fanout"), \
-            "Training fanout must be provided"
+        if self.model_encoder_type in BUILTIN_GNN_ENCODER:
+            assert hasattr(self, "_fanout"), \
+                    "Training fanout must be provided"
 
-        fanout = self._fanout.split(",")
-        return self._check_fanout(fanout, "Train")
+            fanout = self._fanout.split(",")
+            return self._check_fanout(fanout, "Train")
+        return 0
 
     @property
     def eval_fanout(self):
         """ evaluation fanout
         """
         # pylint: disable=no-member
         if hasattr(self, "_eval_fanout"):
@@ -1157,16 +1298,14 @@
     def num_decoder_basis(self):
         """ The number of basis for the decoder in edge prediction task.
         """
         # pylint: disable=no-member
         if hasattr(self, "_num_decoder_basis"):
             assert self._num_decoder_basis > 1, \
                 "Decoder basis must be larger than 1"
-            assert self.decoder_type == "DenseBiDecoder", \
-                "num-decoder-basis only works with DenseBiDecoder"
             return self._num_decoder_basis
 
         # By default, return 2
         return 2
 
     @property
     def decoder_edge_feat(self):
@@ -1363,16 +1502,14 @@
             "Reverse edge types map must be provided."
         return True
 
     @property
     def gamma(self):
         """ Gamma for DistMult
         """
-        assert self.lp_decoder_type == BUILTIN_LP_DISTMULT_DECODER, \
-            "Only used with DistMult"
         if hasattr(self, "_gamma"):
             return float(self._gamma)
 
         # We use this value in DGL-KE
         return 12.0
 
     @property
@@ -1388,21 +1525,21 @@
         return BUILTIN_LP_LOSS_CROSS_ENTROPY
 
     @property
     def task_type(self):
         """ Task type
         """
         # pylint: disable=no-member
-        assert hasattr(self, "_task_type"), \
-            "Task type must be specified"
-        assert self._task_type in SUPPORTED_TASKS, \
-            f"Supported task types include {SUPPORTED_TASKS}, " \
-            f"but got {self._task_type}"
-
-        return self._task_type
+        if hasattr(self, "_task_type"):
+            assert self._task_type in SUPPORTED_TASKS, \
+                    f"Supported task types include {SUPPORTED_TASKS}, " \
+                    f"but got {self._task_type}"
+            return self._task_type
+        else:
+            return None
 
     @property
     def eval_metric(self):
         """ Evaluation metric used during evaluation
 
             The input can be a string specifying the evaluation metric to report
             or a list of strings specifying a list of  evaluation metrics to report.
@@ -1488,14 +1625,38 @@
             else:
                 eval_metric = ["mrr"]
         else:
             assert False, "Unknow task type"
 
         return eval_metric
 
+    @property
+    def num_ffn_layers_in_input(self):
+        """ Number of extra feedforward neural network layers in the input layer
+        """
+        # pylint: disable=no-member
+        if hasattr(self, "_num_ffn_layers_in_input"):
+            assert self._num_ffn_layers_in_input >= 0, \
+                "Number of extra MLP layers in input layer must be larger or equal than 0"
+            return self._num_ffn_layers_in_input
+        # Set default mlp layer number in the input layer to 0
+        return 0
+
+    @property
+    def num_ffn_layers_in_gnn(self):
+        """ Number of extra feedforward neural network layers between GNN layers
+        """
+        # pylint: disable=no-member
+        if hasattr(self, "_num_ffn_layers_in_gnn"):
+            assert self._num_ffn_layers_in_gnn >= 0, \
+                "Number of extra MLP layers between GNN layers must be larger or equal than 0"
+            return self._num_ffn_layers_in_gnn
+        # Set default mlp layer number between gnn layer to 0
+        return 0
+
 def _add_initialization_args(parser):
     group = parser.add_argument_group(title="initialization")
     group.add_argument(
         "--verbose",
         type=lambda x: (str(x).lower() in ['true', '1']),
         default=argparse.SUPPRESS,
         help="Print more information.",
@@ -1541,14 +1702,18 @@
                  "--eval-fanout etype2:20@etype3:20@etype1:20,etype2:10@etype3:4@etype1:2"
                  "Each etype (e.g., etype2) should be a canonical etype in format of"
                  "srcntype/relation/dstntype")
     group.add_argument("--hidden-size", type=int, default=argparse.SUPPRESS,
             help="The number of features in the hidden state")
     group.add_argument("--num-layers", type=int, default=argparse.SUPPRESS,
             help="number of layers in the GNN")
+    group.add_argument("--num-ffn-layers-in-input", type=int, default=argparse.SUPPRESS,
+                       help="number of extra feedforward neural network layers in input layer.")
+    group.add_argument("--num-ffn-layers-in-gnn", type=int, default=argparse.SUPPRESS,
+                       help="number of extra feedforward neural network layers between GNN layers.")
     parser.add_argument(
             "--use-mini-batch-infer",
             help="Whether to use mini-batch or full graph inference during evalution",
             type=lambda x: (str(x).lower() in ['true', '1']),
             default=argparse.SUPPRESS
     )
```

## graphstorm/dataloading/__init__.py

```diff
@@ -21,22 +21,30 @@
 from .dataloading import GSgnnLPLocalJointNegDataLoader
 from .dataloading import GSgnnAllEtypeLPJointNegDataLoader
 from .dataloading import GSgnnAllEtypeLinkPredictionDataLoader
 from .dataloading import GSgnnEdgeDataLoader
 from .dataloading import GSgnnNodeDataLoader
 from .dataloading import GSgnnLinkPredictionTestDataLoader
 from .dataloading import GSgnnLinkPredictionJointTestDataLoader
+from .dataloading import (FastGSgnnLinkPredictionDataLoader,
+                          FastGSgnnLPLocalJointNegDataLoader,
+                          FastGSgnnLPJointNegDataLoader,
+                          FastGSgnnLPLocalUniformNegDataLoader)
 
 from .dataset import GSgnnEdgeTrainData
 from .dataset import GSgnnEdgeInferData
 from .dataset import GSgnnNodeTrainData
 from .dataset import GSgnnNodeInferData
 
 from .dataloading import BUILTIN_LP_UNIFORM_NEG_SAMPLER
 from .dataloading import BUILTIN_LP_JOINT_NEG_SAMPLER
 from .dataloading import BUILTIN_LP_LOCALUNIFORM_NEG_SAMPLER
 from .dataloading import BUILTIN_LP_LOCALJOINT_NEG_SAMPLER
 from .dataloading import BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER
 from .dataloading import BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER
+from .dataloading import (BUILTIN_FAST_LP_UNIFORM_NEG_SAMPLER,
+                          BUILTIN_FAST_LP_JOINT_NEG_SAMPLER,
+                          BUILTIN_FAST_LP_LOCALUNIFORM_NEG_SAMPLER,
+                          BUILTIN_FAST_LP_LOCALJOINT_NEG_SAMPLER)
 
 from .dataloading import (LP_DECODER_EDGE_WEIGHT,
                           EP_DECODER_EDGE_FEAT)
```

## graphstorm/dataloading/dataloading.py

```diff
@@ -20,15 +20,18 @@
 import torch as th
 
 import dgl
 from dgl.dataloading import DistDataLoader
 from dgl.dataloading import EdgeCollator
 from dgl.dataloading.dist_dataloader import _remove_kwargs_dist
 
-from .sampler import LocalUniform, JointUniform, GlobalUniform, JointLocalUniform
+from .sampler import (LocalUniform,
+                      JointUniform,
+                      GlobalUniform,
+                      JointLocalUniform, FastMultiLayerNeighborSampler)
 from .utils import trim_data, modify_fanout_for_target_etype
 
 ################ Minibatch DataLoader (Edge Prediction) #######################
 EP_DECODER_EDGE_FEAT = "ep_edge_feat"
 
 class GSgnnEdgeDataLoader():
     """ The minibatch dataloader for edge prediction
@@ -146,14 +149,18 @@
 
 BUILTIN_LP_UNIFORM_NEG_SAMPLER = 'uniform'
 BUILTIN_LP_JOINT_NEG_SAMPLER = 'joint'
 BUILTIN_LP_LOCALUNIFORM_NEG_SAMPLER = 'localuniform'
 BUILTIN_LP_LOCALJOINT_NEG_SAMPLER = 'localjoint'
 BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER = 'all_etype_uniform'
 BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER = 'all_etype_joint'
+BUILTIN_FAST_LP_UNIFORM_NEG_SAMPLER = 'fast_uniform'
+BUILTIN_FAST_LP_JOINT_NEG_SAMPLER = 'fast_joint'
+BUILTIN_FAST_LP_LOCALUNIFORM_NEG_SAMPLER = 'fast_localuniform'
+BUILTIN_FAST_LP_LOCALJOINT_NEG_SAMPLER = 'fast_localjoint'
 
 LP_DECODER_EDGE_WEIGHT = "lp_edge_weight"
 
 class GSgnnLinkPredictionDataLoader():
     """ Link prediction minibatch dataloader
 
     The negative edges are sampled uniformly.
@@ -301,14 +308,88 @@
     """ Link prediction dataloader with local joint negative sampler
 
     """
 
     def _prepare_negative_sampler(self, num_negative_edges):
         # the default negative sampler is uniform sampler
         negative_sampler = JointLocalUniform(num_negative_edges)
+        return negative_sampler
+
+class FastGSgnnLinkPredictionDataLoader(GSgnnLinkPredictionDataLoader):
+    """ Link prediction dataloader that does not send train_mask to
+        DGL sampler but use the train_mask to trim the sampled graph.
+    """
+
+    def _prepare_dataloader(self, g, target_idxs, fanout,
+                            num_negative_edges, batch_size, device, train_task=True,
+                            exclude_training_targets=False, reverse_edge_types_map=None,
+                            edge_mask_for_gnn_embeddings=None):
+        # The dataloader can only sample neighbors from the training graph.
+        # This can avoid information leak during the link prediction training.
+        # This avoids two types of information leak: it avoids sampling neighbors
+        # from the test graph during the training; it also avoid sampling neighbors
+        # from the test graph to generate embeddings for evaluating the model performance
+        # on the test set.
+        if edge_mask_for_gnn_embeddings is not None and \
+                any(edge_mask_for_gnn_embeddings in g.edges[etype].data
+                    for etype in g.canonical_etypes):
+            sampler = FastMultiLayerNeighborSampler(fanout,
+                                                    mask=edge_mask_for_gnn_embeddings)
+        else:
+            sampler = dgl.dataloading.MultiLayerNeighborSampler(fanout)
+        negative_sampler = self._prepare_negative_sampler(num_negative_edges)
+
+        # edge loader
+        if isinstance(target_idxs, dict):
+            for etype in target_idxs:
+                target_idxs[etype] = trim_data(target_idxs[etype], device)
+        else:
+            target_idxs = trim_data(target_idxs, device)
+        exclude = 'reverse_types' if exclude_training_targets else None
+        reverse_etypes = reverse_edge_types_map if exclude_training_targets else None
+        loader = dgl.dataloading.DistEdgeDataLoader(g,
+                                                    target_idxs,
+                                                    sampler,
+                                                    batch_size=batch_size,
+                                                    negative_sampler=negative_sampler,
+                                                    shuffle=train_task,
+                                                    drop_last=False,
+                                                    num_workers=0,
+                                                    exclude=exclude,
+                                                    reverse_etypes=reverse_etypes)
+        return loader
+
+class FastGSgnnLPJointNegDataLoader(FastGSgnnLinkPredictionDataLoader):
+    """ Link prediction dataloader with joint negative sampler
+
+    """
+
+    def _prepare_negative_sampler(self, num_negative_edges):
+        # the default negative sampler is uniform sampler
+        negative_sampler = JointUniform(num_negative_edges)
+        return negative_sampler
+
+class FastGSgnnLPLocalUniformNegDataLoader(FastGSgnnLinkPredictionDataLoader):
+    """ Link prediction dataloader with local uniform negative sampler
+
+    """
+
+    def _prepare_negative_sampler(self, num_negative_edges):
+        # the default negative sampler is uniform sampler
+        negative_sampler = LocalUniform(num_negative_edges)
+        return negative_sampler
+
+class FastGSgnnLPLocalJointNegDataLoader(FastGSgnnLinkPredictionDataLoader):
+    """ Link prediction dataloader with local joint negative sampler
+
+    """
+
+    def _prepare_negative_sampler(self, num_negative_edges):
+        # the default negative sampler is uniform sampler
+        negative_sampler = JointLocalUniform(num_negative_edges)
         return negative_sampler
 
 ######## Per etype sampler ########
 
 class AllEtypeDistEdgeDataLoader(DistDataLoader):
     """ Distributed edge data sampler that samples at least one
         edge for each edge type in a minibatch
```

## graphstorm/dataloading/dataset.py

```diff
@@ -253,14 +253,19 @@
         labels = {}
         for etype, eid in eids.items():
             assert etype in self._labels
             labels[etype] = self._labels[etype][eid].to(device)
         return labels
 
     @property
+    def labels(self):
+        """Labels"""
+        return self._labels
+
+    @property
     def train_idxs(self):
         """train set's indexes"""
         return self._train_idxs
 
     @property
     def val_idxs(self):
         """validation set's indexes"""
@@ -342,34 +347,37 @@
                     g.edges[canonical_etype].data['train_mask'],
                     pb, etype=canonical_etype, force_even=True)
             else:
                 # If there are no training masks, we assume all edges can be used for training.
                 # Therefore, we use a more memory efficient way to split the edge list.
                 # TODO(zhengda) we need to split the edges properly to increase the data locality.
                 train_idx = split_full_edge_list(g, canonical_etype, get_rank())
+            assert train_idx is not None, "There is no training data."
             num_train += len(train_idx)
             train_idxs[canonical_etype] = train_idx
 
         # If eval_etypes is None, we use all edge types.
         if self.eval_etypes is None:
             self._eval_etypes = g.canonical_etypes
         for canonical_etype in self.eval_etypes:
             # user must provide validation mask
             if 'val_mask' in g.edges[canonical_etype].data:
                 val_idx = dgl.distributed.edge_split(
                     g.edges[canonical_etype].data['val_mask'],
                     pb, etype=canonical_etype, force_even=True)
+                val_idx = [] if val_idx is None else val_idx
                 num_val += len(val_idx)
                 # If there are validation data globally, we should add them to the dict.
                 if dist_sum(len(val_idx)) > 0:
                     val_idxs[canonical_etype] = val_idx
             if 'test_mask' in g.edges[canonical_etype].data:
                 test_idx = dgl.distributed.edge_split(
                     g.edges[canonical_etype].data['test_mask'],
                     pb, etype=canonical_etype, force_even=True)
+                test_idx = [] if test_idx is None else test_idx
                 num_test += len(test_idx)
                 # If there are test data globally, we should add them to the dict.
                 if dist_sum(len(test_idx)) > 0:
                     test_idxs[canonical_etype] = test_idx
         print('part {}, train: {}, val: {}, test: {}'.format(get_rank(), num_train,
                                                              num_val, num_test))
 
@@ -429,36 +437,53 @@
 
         Arguement
         ---------
         g: Dist DGLGraph
         """
         pb = g.get_partition_book()
         test_idxs = {}
+        infer_idxs = {}
         # If eval_etypes is None, we use all edge types.
         if self.eval_etypes is None:
             self._eval_etypes = g.canonical_etypes
-        # test_mask exists
         for canonical_etype in self.eval_etypes:
             if 'test_mask' in g.edges[canonical_etype].data:
+                # test_mask exists
+                # we will do evaluation.
                 test_idx = dgl.distributed.edge_split(
                     g.edges[canonical_etype].data['test_mask'],
                     pb, etype=canonical_etype, force_even=True)
                 # If there are test data globally, we should add them to the dict.
-                if dist_sum(len(test_idx)) > 0:
+                if test_idx is not None and dist_sum(len(test_idx)) > 0:
                     test_idxs[canonical_etype] = test_idx
             else:
-                print(f"WARNING: {canonical_etype} does not contains " \
-                      "test_mask, skip testing {canonical_etype}")
+                # Inference only
+                # we will do inference on the entire edge set
+                print(f"NOTE: {canonical_etype} does not contains " \
+                      f"test_mask, skip testing {canonical_etype}. \n" \
+                      "We will do inference on the entire edge set.")
+                infer_idx = dgl.distributed.edge_split(
+                    th.full((g.num_edges(canonical_etype),), True, dtype=th.bool),
+                    pb, etype=canonical_etype, force_even=True)
+                infer_idxs[canonical_etype] = infer_idx
+
         self._test_idxs = test_idxs
+        self._infer_idxs = infer_idxs
 
     @property
     def eval_etypes(self):
         """edge type for evaluation"""
         return self._eval_etypes
 
+    @property
+    def infer_idxs(self):
+        """ Set of edges to do inference.
+        """
+        return self._infer_idxs
+
 #### Node classification/regression Task Data ####
 class GSgnnNodeData(GSgnnData):  # pylint: disable=abstract-method
     """ Data for node tasks
 
     Parameters
     ----------
     graph_name : str
@@ -506,14 +531,19 @@
         labels = {}
         for ntype, nid in nids.items():
             assert ntype in self._labels
             labels[ntype] = self._labels[ntype][nid].to(device)
         return labels
 
     @property
+    def labels(self):
+        """Labels"""
+        return self._labels
+
+    @property
     def train_idxs(self):
         """train set's indexes"""
         return self._train_idxs
 
     @property
     def val_idxs(self):
         """validation set's indexes"""
@@ -582,28 +612,33 @@
                 node_trainer_ids = g.nodes[ntype].data['trainer_id']
                 train_idx = dgl.distributed.node_split(g.nodes[ntype].data['train_mask'],
                                                        pb, ntype=ntype, force_even=True,
                                                        node_trainer_ids=node_trainer_ids)
             else:
                 train_idx = dgl.distributed.node_split(g.nodes[ntype].data['train_mask'],
                                                        pb, ntype=ntype, force_even=True)
+            assert train_idx is not None, "There is no training data."
             num_train += len(train_idx)
             train_idxs[ntype] = train_idx
 
         for ntype in self.eval_ntypes:
             if 'val_mask' in g.nodes[ntype].data:
                 val_idx = dgl.distributed.node_split(g.nodes[ntype].data['val_mask'],
                                                      pb, ntype=ntype, force_even=True)
+                # If there is no validation data, val_idx is None.
+                val_idx = [] if val_idx is None else val_idx
                 num_val += len(val_idx)
                 # If there are validation data globally, we should add them to the dict.
                 if dist_sum(len(val_idx)) > 0:
                     val_idxs[ntype] = val_idx
             if 'test_mask' in g.nodes[ntype].data:
                 test_idx = dgl.distributed.node_split(g.nodes[ntype].data['test_mask'],
                                                       pb, ntype=ntype, force_even=True)
+                # If there is no test data, test_idx is None.
+                test_idx = [] if test_idx is None else test_idx
                 num_test += len(test_idx)
                 # If there are test data globally, we should add them to the dict.
                 if dist_sum(len(test_idx)) > 0:
                     test_idxs[ntype] = test_idx
 
         print('part {}, train: {}, val: {}, test: {}'.format(get_rank(), num_train,
                                                              num_val, num_test))
@@ -665,23 +700,46 @@
         Arguement
         ---------
         g: DistGraph
             The distributed graph.
         """
         pb = g.get_partition_book()
         test_idxs = {}
+        infer_idxs = {}
         for ntype in self.eval_ntypes:
+            node_trainer_ids = g.nodes[ntype].data['trainer_id'] \
+                if 'trainer_id' in g.nodes[ntype].data else None
             if 'test_mask' in g.nodes[ntype].data:
-                node_trainer_ids = g.nodes[ntype].data['trainer_id'] \
-                        if 'trainer_id' in g.nodes[ntype].data else None
+                # test_mask exists
+                # we will do evaluation.
                 test_idx = dgl.distributed.node_split(g.nodes[ntype].data['test_mask'],
                                                       pb, ntype=ntype, force_even=True,
                                                       node_trainer_ids=node_trainer_ids)
                 # If there are test data globally, we should add them to the dict.
-                if dist_sum(len(test_idx)) > 0:
+                if test_idx is not None and dist_sum(len(test_idx)) > 0:
                     test_idxs[ntype] = test_idx
+                elif test_idx is None:
+                    print(f"WARNING: {ntype} does not contains test data, skip testing {ntype}")
+            else:
+                # Inference only
+                # we will do inference on the entire edge set
+                print(f"NOTE: {ntype} does not contains " \
+                      f"test_mask, skip testing {ntype}. \n" \
+                      "We will do inference on the entire node set.")
+                infer_idx = dgl.distributed.node_split(
+                    th.full((g.num_nodes(ntype),), True, dtype=th.bool),
+                    pb, ntype=ntype, force_even=True,
+                    node_trainer_ids=node_trainer_ids)
+                infer_idxs[ntype] = infer_idx
         self._test_idxs = test_idxs
+        self._infer_idxs = infer_idxs
 
     @property
     def eval_ntypes(self):
         """node type for evaluation"""
         return self._eval_ntypes
+
+    @property
+    def infer_idxs(self):
+        """ Set of nodes to do inference.
+        """
+        return self._infer_idxs
```

## graphstorm/dataloading/sampler.py

```diff
@@ -15,16 +15,19 @@
 
     Addtional graph samplers for GSF
 """
 from collections.abc import Mapping
 import torch as th
 import numpy as np
 from dgl import backend as F
+from dgl import EID, NID
 from dgl.distributed import node_split
 from dgl.dataloading.negative_sampler import Uniform
+from dgl.dataloading import NeighborSampler
+from dgl.transforms import to_block
 
 class LocalUniform(Uniform):
     """Negative sampler that randomly chooses negative destination nodes
     for each source node according to a uniform distribution.
     For each edge ``(u, v)`` of type ``(srctype, etype, dsttype)``, DGL generates
     :attr:`k` pairs of negative edges ``(u, v')``, where ``v'`` is chosen
     uniformly from all the nodes of type ``dsttype``.  The resulting edges will
@@ -239,7 +242,150 @@
                                     pb, ntype=vtype, force_even=True)
             self._local_neg_nids[vtype] = neg_idx
 
         dst = th.randint(len(self._local_neg_nids[vtype]), (shape[0],), dtype=dtype, device=ctx)
         dst = self._local_neg_nids[vtype][dst]
         dst = np.tile(dst, self.k)
         return th.as_tensor(src), th.as_tensor(dst)
+
+class FastMultiLayerNeighborSampler(NeighborSampler):
+    """ Fast MultiLayerNeighborSampler
+
+        If mask is None, it acts the same as dgl.dataloading.MultiLayerNeighborSampler
+
+    Parameters
+    ----------
+    reverse_edge_types_map: dict
+        A map for reverse edge type
+    fanouts : list[int] or list[dict[etype, int]]
+        List of neighbors to sample per edge type for each GNN layer, with the i-th
+        element being the fanout for the i-th GNN layer.
+
+        If only a single integer is provided, DGL assumes that every edge type
+        will have the same fanout.
+
+        If -1 is provided for one edge type on one layer, then all inbound edges
+        of that edge type will be included.
+    edge_dir : str, default ``'in'``
+        Can be either ``'in' `` where the neighbors will be sampled according to
+        incoming edges, or ``'out'`` otherwise, same as :func:`dgl.sampling.sample_neighbors`.
+    prob : str, optional
+        If given, the probability of each neighbor being sampled is proportional
+        to the edge feature value with the given name in ``g.edata``.  The feature must be
+        a scalar on each edge.
+    mask : str, optional
+        If given, a neighbor could be picked only if the edge mask with the given
+        name in ``g.edata`` is True.  The data must be boolean on each edge.
+
+        This argument is mutually exclusive with :attr:`prob`.  If you want to
+        specify both a mask and a probability, consider multiplying the probability
+        with the mask instead.
+    replace : bool, default False
+        Whether to sample with replacement
+    prefetch_node_feats : list[str] or dict[ntype, list[str]], optional
+        The source node data to prefetch for the first MFG, corresponding to the
+        input node features necessary for the first GNN layer.
+    prefetch_labels : list[str] or dict[ntype, list[str]], optional
+        The destination node data to prefetch for the last MFG, corresponding to
+        the node labels of the minibatch.
+    prefetch_edge_feats : list[str] or dict[etype, list[str]], optional
+        The edge data names to prefetch for all the MFGs, corresponding to the
+        edge features necessary for all GNN layers.
+    output_device : device, optional
+        The device of the output subgraphs or MFGs.  Default is the same as the
+        minibatch of seed nodes.
+    reverse_edge_types_map: dict
+        A dict of reverse edge type info.
+    """
+    def __init__(
+        self,
+        fanouts,
+        edge_dir="in",
+        prob=None,
+        mask=None,
+        replace=False,
+        prefetch_node_feats=None,
+        prefetch_labels=None,
+        prefetch_edge_feats=None,
+        output_device=None,
+        reverse_edge_types_map=None,
+    ):
+        self.mask = mask
+        self.reverse_edge_types_map = reverse_edge_types_map
+        # original_edge_types_map is the reverse map of reverse_edge_types_map
+        self.original_edge_types_map = {
+            val: key for key, val in reverse_edge_types_map.items()
+        } if reverse_edge_types_map is not None else None
+
+        super().__init__(
+            fanouts=fanouts,
+            edge_dir=edge_dir,
+            prob=prob,
+            mask=None, # Do neighbor sampling with out edge mask
+            replace=replace,
+            prefetch_node_feats=prefetch_node_feats,
+            prefetch_labels=prefetch_labels,
+            prefetch_edge_feats=prefetch_edge_feats,
+            output_device=output_device
+        )
+
+    def sample_blocks(self, g, seed_nodes, exclude_eids=None):
+        """Generates a list of blocks from the given seed nodes.
+
+        This function must return a triplet where the first element is the input node IDs
+        for the first GNN layer (a tensor or a dict of tensors for heterogeneous graphs),
+        the second element is the output node IDs for the last GNN layer, and the third
+        element is the said list of blocks.
+
+        Parameters
+        ----------
+        g: DGLGraph
+            Graph to sample blocks.
+        seed_nodes: dict of tensors
+            Seed nodes.
+        exclude_eids: func
+            Operations to exlude eids.
+        """
+        output_nodes = seed_nodes
+        blocks = []
+        for fanout in reversed(self.fanouts):
+            frontier = g.sample_neighbors(
+                seed_nodes,
+                fanout,
+                edge_dir=self.edge_dir,
+                prob=self.prob,
+                replace=self.replace,
+                output_device=self.output_device,
+                exclude_edges=exclude_eids,
+            )
+            eid = frontier.edata[EID]
+            new_eid = dict(eid)
+            if self.mask is not None:
+                new_edges = {}
+                for etype in frontier.canonical_etypes:
+                    if self.mask in g.edges[etype].data:
+                        # train mask in data
+                        if etype in eid:
+                            mask = g.edges[etype].data[self.mask][eid[etype]].bool()
+                            new_edges[etype] = mask
+                            new_eid[etype] = eid[etype][mask]
+
+                    elif self.original_edge_types_map is not None and \
+                        self.mask in g.edges[self.original_edge_types_map[etype]].data:
+                        # handle rev-etype edges
+                        # get etype from rev-etype.
+                        original_etype = self.original_edge_types_map[etype]
+                        rev_mask = g.edges[original_etype].data[self.mask][eid[etype]].bool()
+                        new_edges[etype] = rev_mask
+                        new_eid[etype] = eid[etype][rev_mask]
+                    else:
+                        # There is no train mask here
+                        new_edges[etype] = th.full(eid[etype].shape, True, dtype=th.bool)
+                new_frontier = frontier.edge_subgraph(new_edges, relabel_nodes=False)
+            else:
+                new_frontier = frontier
+            block = to_block(new_frontier, seed_nodes)
+            block.edata[EID] = new_eid
+            seed_nodes = block.srcdata[NID]
+            blocks.insert(0, block)
+
+        return seed_nodes, output_nodes, blocks
```

## graphstorm/dataloading/utils.py

```diff
@@ -33,17 +33,15 @@
         device: th.device
             Device
 
         Returns
         -------
         Trimed nids: th.Tensor
     """
-    # NCCL backend only supports GPU tensors, thus here we need to allocate it to gpu
     num_nodes = th.tensor(nids.numel()).to(device)
-    assert num_nodes.is_cuda, "NCCL does not support CPU all_reduce"
     dist.all_reduce(num_nodes, dist.ReduceOp.MIN)
     min_num_nodes = int(num_nodes)
     nids_length = nids.shape[0]
     if min_num_nodes < nids_length:
         new_nids = nids[:min_num_nodes]
         print(f"Pad nids from {nids_length} to {min_num_nodes}")
     else:
@@ -59,16 +57,19 @@
     size : int
         The size in the local process
 
     Returns
     -------
     int : the global size.
     """
-    dev_id = th.cuda.current_device()
-    size = th.tensor([size], device=th.device(dev_id))
+    if th.cuda.is_available():
+        dev_id = th.cuda.current_device()
+        size = th.tensor([size], device=th.device(dev_id))
+    else:
+        size = th.tensor([size], device=th.device("cpu"))
     dist.all_reduce(size, dist.ReduceOp.SUM)
     return int(size.cpu())
 
 def modify_fanout_for_target_etype(g, fanout, target_etypes):
     """ This function specifies a zero fanout for the target etype
         removing this etype from the message passing graph
```

## graphstorm/eval/eval_func.py

```diff
@@ -22,15 +22,15 @@
 import numpy as np
 import torch as th
 from sklearn.metrics import roc_auc_score
 from sklearn.metrics import precision_recall_curve, auc, classification_report
 
 SUPPORTED_CLASSIFICATION_METRICS = {'accuracy', 'precision_recall', \
     'roc_auc', 'f1_score', 'per_class_f1_score'}
-SUPPORTED_REGRESSION_METRICS = {'rmse', 'mse'}
+SUPPORTED_REGRESSION_METRICS = {'rmse', 'mse', 'mae'}
 SUPPORTED_LINK_PREDICTION_METRICS = {"mrr"}
 
 class ClassificationMetrics:
     """ object that compute metrics for classification tasks.
     """
     def __init__(self, multilabel):
         self.supported_metrics = SUPPORTED_CLASSIFICATION_METRICS
@@ -88,19 +88,21 @@
     def __init__(self):
         self.supported_metrics = SUPPORTED_REGRESSION_METRICS
 
         # This is the operator used to compare whether current value is better than the current best
         self.metric_comparator = {}
         self.metric_comparator["rmse"] = operator.ge
         self.metric_comparator["mse"] = operator.ge
+        self.metric_comparator["mae"] = operator.ge
 
         # This is the operator used to measure each metric performance
         self.metric_function = {}
         self.metric_function["rmse"] = compute_rmse
         self.metric_function["mse"] = compute_mse
+        self.metric_function["mae"] = compute_mae
 
     def assert_supported_metric(self, metric):
         """ check if the given metric is supported.
         """
         assert metric in self.supported_metrics, \
             f"Metric {metric} not supported for regression"
 
@@ -367,7 +369,25 @@
         warnings.warn("prediction and labels have different data types: "
                       f"{pred.dtype} vs. {labels.dtype}")
         warnings.warn("casting pred to the same dtype as labels")
         pred = pred.type(labels.dtype) # cast pred to the same dtype as labels.
 
     diff = pred.cpu() - labels.cpu()
     return th.mean(diff * diff).cpu().item()
+
+def compute_mae(pred, labels):
+    """ compute MAE for regression
+    """
+    # TODO: check dtype of label before training or evaluation
+    assert th.is_floating_point(pred) and th.is_floating_point(labels), \
+        "prediction and labels must be floating points"
+
+    assert pred.shape == labels.shape, \
+        f"prediction and labels have different shapes. {pred.shape} vs. {labels.shape}"
+    if pred.dtype != labels.dtype:
+        warnings.warn("prediction and labels have different data types: "
+                      f"{pred.dtype} vs. {labels.dtype}")
+        warnings.warn("casting pred to the same dtype as labels")
+        pred = pred.type(labels.dtype) # cast pred to the same dtype as labels.
+
+    diff = th.abs(pred.cpu() - labels.cpu())
+    return th.mean(diff).cpu().item()
```

## graphstorm/eval/evaluator.py

```diff
@@ -385,16 +385,18 @@
                 Test MSE
         """
         # exchange preds and labels between runners
         local_rank = th.distributed.get_rank()
         world_size = th.distributed.get_world_size()
         val_pred = broadcast_data(local_rank, world_size, val_pred)
         val_labels = broadcast_data(local_rank, world_size, val_labels)
-        test_pred = broadcast_data(local_rank, world_size, test_pred)
-        test_labels = broadcast_data(local_rank, world_size, test_labels)
+        test_pred = broadcast_data(local_rank, world_size, test_pred) \
+            if test_pred is not None else None
+        test_labels = broadcast_data(local_rank, world_size, test_labels) \
+            if test_labels is not None else None
 
         with th.no_grad():
             val_score = self.compute_score(val_pred, val_labels)
             test_score = self.compute_score(test_pred, test_labels)
 
         for metric in self.metric:
             # be careful whether > or < it might change per metric.
@@ -418,19 +420,22 @@
                 Label
 
             Returns
             -------
             Evaluation metric values: dict
         """
         scores = {}
-        pred = th.squeeze(pred)
-        labels = th.squeeze(labels)
-        for metric in self.metric:
-            scores[metric] = self.metrics_obj.metric_function[metric](pred, labels) \
-                    if pred is not None and labels is not None else -1
+        if pred is None or labels is None:
+            for metric in self.metric:
+                scores[metric] = "N/A"
+        else: # pred is not None and labels is not None
+            pred = th.squeeze(pred)
+            labels = th.squeeze(labels)
+            for metric in self.metric:
+                scores[metric] = self.metrics_obj.metric_function[metric](pred, labels)
         return scores
 
 class GSgnnAccEvaluator(GSgnnInstanceEvaluator):
     """ The class for user defined evaluator.
 
     Parameters
     ----------
@@ -494,16 +499,18 @@
                 Test Score
         """
         # exchange preds and labels between runners
         local_rank = th.distributed.get_rank()
         world_size = th.distributed.get_world_size()
         val_pred = broadcast_data(local_rank, world_size, val_pred)
         val_labels = broadcast_data(local_rank, world_size, val_labels)
-        test_pred = broadcast_data(local_rank, world_size, test_pred)
-        test_labels = broadcast_data(local_rank, world_size, test_labels)
+        test_pred = broadcast_data(local_rank, world_size, test_pred) \
+            if test_pred is not None else None
+        test_labels = broadcast_data(local_rank, world_size, test_labels) \
+            if test_labels is not None else None
 
         with th.no_grad():
             val_score = self.compute_score(val_pred, val_labels, train=False)
             test_score = self.compute_score(test_pred, test_labels, train=False)
 
         for metric in self.metric:
             # be careful whether > or < it might change per metric.
@@ -540,15 +547,15 @@
                 else:
                     # validation or testing may have a different
                     # evaluation function, in our case the evaluation code
                     # may return a dictionary with the metric values for each label
                     results[metric] = self.metrics_obj.metric_eval_function[metric](pred, labels)
             else:
                 # if the pred is None or the labels is None the metric can not me computed
-                results[metric] = -1
+                results[metric] = "N/A"
         return results
 
 class GSgnnLPEvaluator():
     """ Template class for user defined evaluator.
 
     Parameters
     ----------
@@ -858,24 +865,27 @@
         -----------
         val_mrr: float
             Validation mrr
         test_mrr: float
             Test mrr
         """
         with th.no_grad():
-            test_score = self.compute_score(test_scores)
+            if test_scores is not None:
+                test_score = self.compute_score(test_scores)
+            else:
+                test_score = {"mrr": "N/A"} # Dummy
 
             if val_scores is not None:
                 val_score = self.compute_score(val_scores)
 
                 if get_rank() == 0:
                     for metric in self.metric:
                         # be careful whether > or < it might change per metric.
                         if self.metrics_obj.metric_comparator[metric](
                             self._best_val_score[metric], val_score[metric]):
                             self._best_val_score[metric] = val_score[metric]
                             self._best_test_score[metric] = test_score[metric]
                             self._best_iter[metric] = total_iters
             else:
-                val_score = {"mrr": -1} # Dummy
+                val_score = {"mrr": "N/A"} # Dummy
 
         return val_score, test_score
```

## graphstorm/gconstruct/construct_graph.py

```diff
@@ -27,31 +27,29 @@
 
 import numpy as np
 import torch as th
 import dgl
 
 from ..utils import sys_tracker
 from .file_io import parse_node_file_format, parse_edge_file_format
-from .file_io import get_in_files, HDF5Array
+from .file_io import get_in_files
 from .transform import parse_feat_ops, process_features, preprocess_features
 from .transform import parse_label_ops, process_labels
-from .transform import (do_multiprocess_transform,
-                        TwoPhaseFeatTransform,
-                        GlobalProcessFeatTransform)
+from .transform import do_multiprocess_transform
 from .id_map import NoopMap, IdMap, map_node_ids
 from .utils import (multiprocessing_data_read,
                     update_two_phase_feat_ops, ExtMemArrayMerger,
-                    partition_graph)
+                    partition_graph, ExtMemArrayWrapper)
 
 def prepare_node_data(in_file, feat_ops, read_file):
-    """ Parse node data.
+    """ Prepare node data information for data transformation.
 
-    The function parses a node file that contains node IDs, features and labels
+    The function parses a node file that contains node features
     The node file is parsed according to users' configuration
-    and performs some feature transformation.
+    and transformation related information is extracted.
 
     Parameters
     ----------
     in_file : str
         The path of the input node file.
     feat_ops : dict of FeatTransform
         The operations run on the node features of the node file.
@@ -97,14 +95,40 @@
     if label_ops is not None:
         label_data = process_labels(data, label_ops)
         for key, val in label_data.items():
             feat_data[key] = val
     node_ids = data[node_id_col] if node_id_col in data else None
     return (node_ids, feat_data)
 
+def prepare_edge_data(in_file, feat_ops, read_file):
+    """ Prepare edge data information for data transformation.
+
+    The function parses a edge file that contains edge features
+    The edge file is parsed according to users' configuration
+    and transformation related information is extracted.
+
+    Parameters
+    ----------
+    in_file : str
+        The path of the input edge file.
+    feat_ops : dict of FeatTransform
+        The operations run on the edge features of the edge file.
+    read_file : callable
+        The function to read the edge file
+
+    Returns
+    -------
+    dict : A dict of edge feature info.
+    """
+    data = read_file(in_file)
+    assert feat_ops is not None, "feat_ops must exist when prepare_edge_data is called."
+    feat_info = preprocess_features(data, feat_ops)
+
+    return feat_info
+
 def parse_edge_data(in_file, feat_ops, label_ops, node_id_map, read_file,
                     conf, skip_nonexist_edges):
     """ Parse edge data.
 
     The function parses an edge file that contains the source and destination node
     IDs, edge features and potentially edge labels. The edge file is parsed
     according to users' configuration and performs some feature transformation.
@@ -146,14 +170,51 @@
     src_ids = data[src_id_col] if src_id_col is not None else None
     dst_ids = data[dst_id_col] if dst_id_col is not None else None
     if src_ids is not None:
         src_ids, dst_ids = map_node_ids(src_ids, dst_ids, edge_type, node_id_map,
                                         skip_nonexist_edges)
     return (src_ids, dst_ids, feat_data)
 
+def _process_data(user_pre_parser, user_parser,
+                  two_phase_feat_ops,
+                  in_files, num_proc, task_info):
+    """ Process node and edge data.
+
+    Parameter
+    ---------
+    user_pre_parser: func
+        A function that prepares data for processing.
+    user_parser: func
+        A function that processes node data or edge data.
+    two_phase_feat_ops: list of TwoPhaseFeatTransform
+        List of TwoPhaseFeatTransform transformation ops.
+    in_files: list of strings
+        The input files.
+    num_proc: int
+        Number of processes to do processing.
+    task_info: str
+        Task meta info for debugging.
+    """
+    if len(two_phase_feat_ops) > 0:
+        pre_parse_start = time.time()
+        phase_one_ret = multiprocessing_data_read(in_files, num_proc, user_pre_parser)
+        update_two_phase_feat_ops(phase_one_ret, two_phase_feat_ops)
+
+        dur = time.time() - pre_parse_start
+        logging.debug("Preprocessing data files for %s takes %.3f seconds.",
+                      task_info, dur)
+
+    start = time.time()
+    return_dict = multiprocessing_data_read(in_files, num_proc, user_parser)
+    dur = time.time() - start
+    logging.debug("Processing data files for %s takes %.3f seconds.",
+                    task_info, dur)
+    return return_dict
+
+
 def process_node_data(process_confs, arr_merger, remap_id, num_processes=1):
     """ Process node data
 
     We need to process all node data before we can process edge data.
     Processing node data will generate the ID mapping.
 
     The node data of a node type is defined as follows:
@@ -200,66 +261,53 @@
         # each iteration is to process a node type.
         assert 'node_type' in process_conf, \
                 "'node_type' must be defined for a node type"
         node_type = process_conf['node_type']
         assert 'files' in process_conf, \
                 "'files' must be defined for a node type"
         in_files = get_in_files(process_conf['files'])
-        feat_ops = parse_feat_ops(process_conf['features']) \
-                if 'features' in process_conf else None
-        label_ops = parse_label_ops(process_conf['labels'], is_node=True) \
+        (feat_ops, two_phase_feat_ops, after_merge_feat_ops) = \
+            parse_feat_ops(process_conf['features']) \
+                if 'features' in process_conf else (None, [], {})
+        label_ops = parse_label_ops(process_conf, is_node=True) \
                 if 'labels' in process_conf else None
         assert 'format' in process_conf, \
                 "'format' must be defined for a node type"
-        multiprocessing = do_multiprocess_transform(process_conf, feat_ops, label_ops, in_files)
+
         # If it requires multiprocessing, we need to read data to memory.
-        read_file = parse_node_file_format(process_conf, in_mem=multiprocessing)
         node_id_col = process_conf['node_id_col'] if 'node_id_col' in process_conf else None
+        multiprocessing = do_multiprocess_transform(process_conf,
+                                                    feat_ops,
+                                                    label_ops,
+                                                    in_files)
+        read_file = parse_node_file_format(process_conf, in_mem=multiprocessing)
         num_proc = num_processes if multiprocessing else 0
-
-        two_phase_feat_ops = []
-        after_merge_feat_ops = {}
-        if feat_ops is not None:
-            for op in feat_ops:
-                if isinstance(op, TwoPhaseFeatTransform):
-                    two_phase_feat_ops.append(op)
-                if isinstance(op, GlobalProcessFeatTransform):
-                    after_merge_feat_ops[op.feat_name] = op
-
-        if len(two_phase_feat_ops) > 0:
-            user_pre_parser = partial(prepare_node_data, feat_ops=two_phase_feat_ops,
-                                      read_file=read_file)
-            pre_parse_start = time.time()
-            phase_one_ret = multiprocessing_data_read(in_files, num_proc, user_pre_parser)
-            update_two_phase_feat_ops(phase_one_ret, two_phase_feat_ops)
-
-            dur = time.time() - pre_parse_start
-            logging.debug("Preprocessing data files for node %s takes %.3f seconds.",
-                        node_type, dur)
-
+        user_pre_parser = partial(prepare_node_data, feat_ops=two_phase_feat_ops,
+                                  read_file=read_file)
         user_parser = partial(parse_node_data, feat_ops=feat_ops,
                               label_ops=label_ops,
                               node_id_col=node_id_col,
                               read_file=read_file)
-        start = time.time()
-        return_dict = multiprocessing_data_read(in_files, num_proc, user_parser)
-        dur = time.time() - start
-        logging.debug("Processing data files for node %s takes %.3f seconds.",
-                      node_type, dur)
 
+        return_dict = _process_data(user_pre_parser,
+                                    user_parser,
+                                    two_phase_feat_ops,
+                                    in_files,
+                                    num_proc,
+                                    f"node {node_type}")
         type_node_id_map = [None] * len(return_dict)
         type_node_data = {}
         for i, (node_ids, data) in return_dict.items():
             for feat_name in data:
                 if feat_name not in type_node_data:
                     type_node_data[feat_name] = [None] * len(return_dict)
                 type_node_data[feat_name][i] = data[feat_name]
-            # If it's HDF5Array, it's better to convert it into a Numpy array.
+            # If it's ExtMemArray, it's better to convert it into a Numpy array.
             # This will make the next operations on it more efficiently.
-            if isinstance(node_ids, HDF5Array):
+            if isinstance(node_ids, ExtMemArrayWrapper):
                 type_node_id_map[i] = node_ids.to_numpy()
             else:
                 type_node_id_map[i] = node_ids
         return_dict = None
 
         # Construct node Id map.
         if type_node_id_map[0] is not None:
@@ -375,40 +423,48 @@
                 "'relation' is not defined for an edge type."
         edge_type = process_conf['relation']
         assert 'files' in process_conf, \
                 "'files' is not defined for an edge type."
         in_files = get_in_files(process_conf['files'])
         assert 'format' in process_conf, \
                 "'format' is not defined for an edge type."
-        feat_ops = parse_feat_ops(process_conf['features']) \
-                if 'features' in process_conf else None
-        label_ops = parse_label_ops(process_conf['labels'], is_node=False) \
+        (feat_ops, two_phase_feat_ops, after_merge_feat_ops) = \
+            parse_feat_ops(process_conf['features']) \
+                if 'features' in process_conf else (None, [], {})
+        label_ops = parse_label_ops(process_conf, is_node=False) \
                 if 'labels' in process_conf else None
-        multiprocessing = do_multiprocess_transform(process_conf, feat_ops, label_ops, in_files)
-        # If it requires multiprocessing, we need to read data to memory.
-        read_file = parse_edge_file_format(process_conf, in_mem=multiprocessing)
 
         # We don't need to copy all node ID maps to the worker processes.
         # Only the node ID maps of the source node type and destination node type
         # are sufficient.
         id_map = {edge_type[0]: node_id_map[edge_type[0]],
                   edge_type[2]: node_id_map[edge_type[2]]}
+
+        multiprocessing = do_multiprocess_transform(process_conf,
+                                                    feat_ops,
+                                                    label_ops,
+                                                    in_files)
+        # If it requires multiprocessing, we need to read data to memory.
+        read_file = parse_edge_file_format(process_conf, in_mem=multiprocessing)
+        num_proc = num_processes if multiprocessing else 0
+        user_pre_parser = partial(prepare_edge_data, feat_ops=two_phase_feat_ops,
+                                  read_file=read_file)
         user_parser = partial(parse_edge_data, feat_ops=feat_ops,
                               label_ops=label_ops,
                               node_id_map=id_map,
                               read_file=read_file,
                               conf=process_conf,
                               skip_nonexist_edges=skip_nonexist_edges)
-        start = time.time()
-        num_proc = num_processes if multiprocessing else 0
-        return_dict = multiprocessing_data_read(in_files, num_proc, user_parser)
-        dur = time.time() - start
-        logging.debug("Processing data files for edges of %s takes %.3f seconds",
-                      str(edge_type), dur)
 
+        return_dict = _process_data(user_pre_parser,
+                                    user_parser,
+                                    two_phase_feat_ops,
+                                    in_files,
+                                    num_proc,
+                                    f"edge {edge_type}")
         type_src_ids = [None] * len(return_dict)
         type_dst_ids = [None] * len(return_dict)
         type_edge_data = {}
         for i, (src_ids, dst_ids, part_data) in return_dict.items():
             type_src_ids[i] = src_ids
             type_dst_ids[i] = dst_ids
             for feat_name in part_data:
@@ -416,16 +472,20 @@
                     type_edge_data[feat_name] = [None] * len(return_dict)
                 type_edge_data[feat_name][i] = part_data[feat_name]
         return_dict = None
 
         # handle edge type
         for feat_name in type_edge_data:
             etype_str = "-".join(edge_type)
-            type_edge_data[feat_name] = arr_merger(type_edge_data[feat_name],
+            merged_feat = arr_merger(type_edge_data[feat_name],
                                                    etype_str + "_" + feat_name)
+            if feat_name in after_merge_feat_ops:
+                # do data transformation with the entire feat array.
+                merged_feat = after_merge_feat_ops[feat_name].after_merge_transform(merged_feat)
+            type_edge_data[feat_name] = merged_feat
             gc.collect()
             sys_tracker.check(f'Merge edge data {feat_name} of {edge_type}')
 
         edge_type = tuple(edge_type)
         if type_src_ids[0] is not None: # handle src_ids and dst_ids
             assert all(src_ids is not None for src_ids in type_src_ids)
             assert all(dst_ids is not None for dst_ids in type_dst_ids)
@@ -545,24 +605,25 @@
     verify_confs(process_confs)
     # We only store data to external memory if we partition a graph for distributed training.
     ext_mem_workspace = args.ext_mem_workspace if args.output_format == "DistDGL" else None
     convert2ext_mem = ExtMemArrayMerger(ext_mem_workspace, args.ext_mem_feat_size)
     node_id_map, node_data = process_node_data(process_confs['nodes'], convert2ext_mem,
                                                args.remap_node_id,
                                                num_processes=num_processes_for_nodes)
+    sys_tracker.check('Process the node data')
     edges, edge_data = process_edge_data(process_confs['edges'], node_id_map,
                                          convert2ext_mem,
                                          num_processes=num_processes_for_edges,
                                          skip_nonexist_edges=args.skip_nonexist_edges)
+    sys_tracker.check('Process the edge data')
     num_nodes = {ntype: len(node_id_map[ntype]) for ntype in node_id_map}
     if args.output_conf_file is not None:
         # Save the new config file.
         with open(args.output_conf_file, "w", encoding="utf8") as outfile:
             json.dump(process_confs, outfile, indent=4)
-    sys_tracker.check('Process input data')
 
     if args.add_reverse_edges:
         edges1 = {}
         for etype in edges:
             e = edges[etype]
             assert isinstance(e, tuple) and len(e) == 2
             assert isinstance(etype, tuple) and len(etype) == 3
@@ -595,21 +656,21 @@
         partition_graph(g, node_data, edge_data, args.graph_name,
                         args.num_parts, args.output_dir,
                         save_mapping=True, # always save mapping
                         part_method=args.part_method)
     elif args.output_format == "DGL":
         for ntype in node_data:
             for name, ndata in node_data[ntype].items():
-                if isinstance(ndata, HDF5Array):
+                if isinstance(ndata, ExtMemArrayWrapper):
                     g.nodes[ntype].data[name] = ndata.to_tensor()
                 else:
                     g.nodes[ntype].data[name] = th.tensor(ndata)
         for etype in edge_data:
             for name, edata in edge_data[etype].items():
-                if isinstance(edata, HDF5Array):
+                if isinstance(edata, ExtMemArrayWrapper):
                     g.edges[etype].data[name] = edata.to_tensor()
                 else:
                     g.edges[etype].data[name] = th.tensor(edata)
         dgl.save_graphs(os.path.join(args.output_dir, args.graph_name + ".dgl"), [g])
     else:
         raise ValueError('Unknown output format: {}'.format(args.output_format))
     for ntype in node_id_map:
```

## graphstorm/gconstruct/file_io.py

```diff
@@ -20,16 +20,18 @@
 import glob
 import json
 import os
 
 import pyarrow.parquet as pq
 import pyarrow as pa
 import numpy as np
-import torch as th
 import h5py
+import pandas as pd
+
+from .utils import HDF5Handle, HDF5Array
 
 def read_index_json(data_file):
     """ Read the index from a JSON file.
 
     Each row is a JSON object that contains an index.
 
     Parameters
@@ -57,14 +59,60 @@
     data_file : str
         The data file where the indices are written to.
     """
     with open(data_file, 'w', encoding="utf8") as json_file:
         for index in data:
             json_file.write(json.dumps(int(index)) + "\n")
 
+def read_data_csv(data_file, data_fields=None, delimiter=','):
+    """ Read data from a CSV file.
+
+    Parameters
+    ----------
+    data_file : str
+        The file that contains the data.
+    data_fields : list of str
+        The name of the data fields.
+    delimiter : str
+        The delimiter to separate the fields.
+
+    Returns
+    -------
+    dict of Numpy arrays.
+    """
+    data = pd.read_csv(data_file, delimiter=delimiter)
+    if data_fields is not None:
+        for field in data_fields:
+            assert field in data, f"The data field {field} does not exist in the data file."
+        return {field: data[field].to_numpy() for field in data_fields}
+    else:
+        return {field: data[field].to_numpy() for field in data}
+
+def write_data_csv(data, data_file, delimiter=','):
+    """ Write data to a CSV file.
+
+    Parameters
+    ----------
+    data : dict of Numpy arrays
+        The data arrays that need to be written to the CSV file.
+    data_file : str
+        The path of the data file.
+    delimiter : str
+        The delimiter that separates the fields.
+    """
+    data_frame = pd.DataFrame(data)
+    data_frame.to_csv(data_file, index=True, sep=delimiter)
+
+def _pad_stack(arrs):
+    max_len = max(len(arr) for arr in arrs)
+    new_arrs = np.zeros((len(arrs), max_len), dtype=arrs[0].dtype)
+    for i, arr in enumerate(arrs):
+        new_arrs[i][:len(arr)] = arr
+    return new_arrs
+
 def read_data_json(data_file, data_fields):
     """ Read data from a JSON file.
 
     Each row of the JSON file represents a data record. Each JSON object
     is single-level dict without any nested dict structure.
     The function tries to extract a set of values from the data record.
 
@@ -86,33 +134,47 @@
             data_records.append(record)
 
     data = {key: [] for key in data_fields}
     for record in data_records:
         for key in data_fields:
             assert key in record, \
                     f"The data field {key} does not exist in the record {record} of {data_file}."
-            data[key].append(record[key])
+            record1 = np.array(record[key]) if isinstance(record[key], list) else record[key]
+            data[key].append(record1)
     for key in data:
-        data[key] = np.array(data[key])
+        if isinstance(data[key][0], np.ndarray):
+            data[key] = _pad_stack(data[key])
+        else:
+            data[key] = np.array(data[key])
     return data
 
 def write_data_json(data, data_file):
     """ Write data to a json file.
     """
     records = []
     for key in data:
         if len(records) == 0:
             records = [{} for _ in range(len(data[key]))]
         assert len(records) == len(data[key])
-        if data[key].shape == 1:
-            for i, val in enumerate(data[key]):
-                records[i][key] = val
+        if isinstance(data[key], np.ndarray):
+            if data[key].shape == 1:
+                for i, val in enumerate(data[key]):
+                    records[i][key] = val
+            else:
+                for i, val in enumerate(data[key]):
+                    records[i][key] = val.tolist()
+        elif isinstance(data[key], list):
+            if isinstance(data[key][0], np.ndarray):
+                for i, val in enumerate(data[key]):
+                    records[i][key] = val.tolist()
+            else:
+                for i, val in enumerate(data[key]):
+                    records[i][key] = val
         else:
-            for i, val in enumerate(data[key]):
-                records[i][key] = val.tolist()
+            raise ValueError("Invalid data.")
     with open(data_file, 'w', encoding="utf8") as json_file:
         for record in records:
             record = json.dumps(record)
             json_file.write(record + "\n")
 
 def read_data_parquet(data_file, data_fields=None):
     """ Read data from a parquet file.
@@ -162,136 +224,25 @@
         The data to be saved to the Parquet file.
     data_file : str
         The file name of the Parquet file.
     """
     arr_dict = {}
     for key in data:
         arr = data[key]
+        assert np.prod(arr.shape) < 2 * 1024 * 1024 * 1024, \
+                "Some PyArrow versions do not support a column with over 2 billion elements."
         assert len(arr.shape) == 1 or len(arr.shape) == 2, \
                 "We can only write a vector or a matrix to a parquet file."
         if len(arr.shape) == 1:
             arr_dict[key] = arr
         else:
             arr_dict[key] = [arr[i] for i in range(len(arr))]
     table = pa.Table.from_arrays(list(arr_dict.values()), names=list(arr_dict.keys()))
     pq.write_table(table, data_file)
 
-class HDF5Handle:
-    """ HDF5 file handle
-
-    This is to reference the HDF5 handle and close it when no one
-    uses the HDF5 file.
-
-    Parameters
-    ----------
-    f : HDF5 file handle
-        The handle to access the HDF5 file.
-    """
-    def __init__(self, f):
-        self._f = f
-
-    def __del__(self):
-        return self._f.close()
-
-
-class HDF5Array:
-    """ This is an array wrapper class for HDF5 array.
-
-    The main purpose of this class is to make sure that we can close
-    the HDF5 files when the array is destroyed.
-
-    Parameters
-    ----------
-    arr : HDF5 dataset
-        The array-like object for accessing the HDF5 file.
-    handle : HDF5Handle
-        The handle that references to the opened HDF5 file.
-    """
-    def __init__(self, arr, handle):
-        self._arr = arr
-        self._handle = handle
-        self._out_dtype = None # Use the dtype of self._arr
-
-    def __len__(self):
-        return self._arr.shape[0]
-
-    def __getitem__(self, idx):
-        """ Slicing data from the array.
-
-        Parameters
-        ----------
-        idx : Numpy array or Pytorch tensor or slice.
-            The index.
-
-        Returns
-        -------
-        Numpy array : the data from the HDF5 array indexed by `idx`.
-        """
-        if isinstance(idx, slice):
-            return self._arr[idx]
-
-        if isinstance(idx, th.Tensor):
-            idx = idx.numpy()
-        # If the idx are sorted.
-        if np.all(idx[1:] - idx[:-1] > 0):
-            arr = self._arr[idx]
-        else:
-            # There are two cases here: 1) there are duplicated IDs,
-            # 2) the IDs are not sorted. Unique can return unique
-            # IDs in the ascending order that meets the requirement of
-            # HDF5 indexing.
-            uniq_ids, reverse_idx = np.unique(idx, return_inverse=True)
-            arr = self._arr[uniq_ids][reverse_idx]
-
-        if self._out_dtype is not None:
-            arr = arr.astype(self._out_dtype)
-        return arr
-
-    def to_tensor(self):
-        """ Return Pytorch tensor.
-        """
-        arr = th.tensor(self._arr)
-        if self._out_dtype is not None:
-            if self._out_dtype is np.float32:
-                arr = arr.to(th.float32)
-            elif self._out_dtype is np.float16:
-                arr = arr.to(th.float16)
-        return arr
-
-    def to_numpy(self):
-        """ Return Numpy array.
-        """
-        res = self._arr[:]
-        if self._out_dtype is not None:
-            res = res.astype(self._out_dtype)
-        return res
-
-    def astype(self, dtype):
-        """ Set the output dtype.
-
-        Parameters
-        ----------
-        dtype: numpy.dtype
-            Output dtype
-        """
-        self._out_dtype = dtype
-        return self
-
-    @property
-    def shape(self):
-        """ The shape of the HDF5 array.
-        """
-        return self._arr.shape
-
-    @property
-    def dtype(self):
-        """ The data type of the HDF5 array.
-        """
-        return self._arr.dtype
-
 def read_data_hdf5(data_file, data_fields=None, in_mem=True):
     """ Read the data from a HDF5 file.
 
     If `in_mem` is False, we don't read data into memory.
 
     Parameters
     ----------
@@ -366,14 +317,17 @@
                 keys.append(label_conf["label_col"])
     if fmt["name"] == "parquet":
         return partial(read_data_parquet, data_fields=keys)
     elif fmt["name"] == "json":
         return partial(read_data_json, data_fields=keys)
     elif fmt["name"] == "hdf5":
         return partial(read_data_hdf5, data_fields=keys, in_mem=in_mem)
+    elif fmt["name"] == "csv":
+        delimiter = fmt["delimiter"] if "delimiter" in fmt else ","
+        return partial(read_data_csv, data_fields=keys, delimiter=delimiter)
     else:
         raise ValueError('Unknown file format: {}'.format(fmt['name']))
 
 parse_node_file_format = partial(_parse_file_format, is_node=True)
 parse_edge_file_format = partial(_parse_file_format, is_node=False)
 
 def get_in_files(in_files):
```

## graphstorm/gconstruct/id_map.py

```diff
@@ -19,15 +19,15 @@
 import logging
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import numpy as np
 
-from .file_io import HDF5Array
+from .utils import ExtMemArrayWrapper
 
 class NoopMap:
     """ It doesn't map IDs.
 
     This is an identity map. It doesn't do any mapping on IDs.
 
     Parameters
@@ -73,20 +73,28 @@
 
     Parameters
     ----------
     ids : Array
         The input IDs
     """
     def __init__(self, ids):
-        # If the IDs are stored in HDF5Array, we should convert it to Numpy array.
-        # HDF5Array stores data on disks. Loading all IDs to memory can accelerate
+        # If the IDs are stored in ExtMemArray, we should convert it to Numpy array.
+        # ExtMemArray stores data on disks. Loading all IDs to memory can accelerate
         # the following operations.
-        if isinstance(ids, HDF5Array):
+        if isinstance(ids, ExtMemArrayWrapper):
             ids = ids.to_numpy()
-        self._ids = {id1: i for i, id1 in enumerate(ids)}
+
+        # We can not expect the dtype of ids is always integer or string
+        # it can be any type. So we will cast ids into string if it is not integer.
+        if isinstance(ids[0], int) or np.issubdtype(ids.dtype, np.integer):
+            # node_ids are integer ids
+            self._ids = {id1: i for i, id1 in enumerate(ids)}
+        else:
+            # cast everything else into string
+            self._ids = {str(id1): i for i, id1 in enumerate(ids)}
 
     def __len__(self):
         return len(self._ids)
 
     def map_id(self, ids):
         """ Map the input IDs to the new IDs.
 
@@ -95,35 +103,40 @@
         ids : tensor
             The input IDs
 
         Returns
         -------
         tuple of tensors : the tensor of new IDs, the location of the IDs in the input ID tensor.
         """
+        if len(ids) == 0:
+            return np.array([], dtype=np.int64), np.array([], dtype=np.int64)
         for id_ in self._ids:
-            # If the data type of the key is string, the input Ids should also be strings.
+            # If the data type of the key is string, the input Ids should not be integer.
             if isinstance(id_, str):
-                assert isinstance(ids[0], str), \
-                        "The key of ID map is string, input IDs should also be strings."
+                assert (not isinstance(ids[0], int)) and \
+                       (not np.issubdtype(ids.dtype, np.integer)), \
+                    "The key of ID map is string, input IDs are integers."
             elif isinstance(id_, int) or np.issubdtype(id_.dtype, np.integer):
                 # If the data type of the key is integer, the input Ids should
                 # also be integers.
                 assert np.issubdtype(ids.dtype, np.integer), \
                         "The key of ID map is integer, input IDs should also be integers. " \
                         + f"But get {type(ids[0])}."
             else:
-                raise ValueError(f"Unsupported key data type: {type(id_)}")
+                logging.warning("The input data type is %s. Will treat IDs as string.",
+                                type(id_))
             break
 
         # If the input ID exists in the ID map, map it to a new ID
         # and keep its location in the input ID array.
         # Otherwise, skip the ID.
         new_ids = []
         idx = []
         for i, id_ in enumerate(ids):
+            id_ = id_ if np.issubdtype(ids.dtype, np.integer) else str(id_)
             if id_ in self._ids:
                 new_ids.append(self._ids[id_])
                 idx.append(i)
         return np.array(new_ids), np.array(idx)
 
     def save(self, file_path):
         """ Save the ID map to a parquet file.
@@ -143,15 +156,16 @@
         pq.write_table(table, file_path)
         return True
 
 def map_node_ids(src_ids, dst_ids, edge_type, node_id_map, skip_nonexist_edges):
     """ Map node IDs of source and destination nodes of edges.
 
     In the ID mapping, we need to handle multiple errors in the input data:
-    1) we handle the case that endpoint nodes of edges don't exist;
+    1) we handle the case that endpoint nodes of edges don't exist; if all endpoint nodes
+    do not exist, we return an empty edge list.
     2) we handle the case that the data type of node IDs of the endpoint nodes don't
     match the data type of the keys of the ID map.
 
     Parameters
     ----------
     src_ids : tensor
         The source nodes.
@@ -169,30 +183,32 @@
     tuple of tensors : the remapped source and destination node IDs.
     """
     src_type, _, dst_type = edge_type
     new_src_ids, orig_locs = node_id_map[src_type].map_id(src_ids)
     # If some of the source nodes don't exist in the node set.
     if len(orig_locs) != len(src_ids):
         bool_mask = np.ones(len(src_ids), dtype=bool)
-        bool_mask[orig_locs] = False
+        if len(orig_locs) > 0:
+            bool_mask[orig_locs] = False
         if skip_nonexist_edges:
-            logging.warning("source nodes of %s do not exist: %s",
-                            src_type, str(src_ids[bool_mask]))
+            logging.warning("source nodes of %s do not exist. Skip %d edges",
+                            src_type, len(src_ids[bool_mask]))
         else:
             raise ValueError(f"source nodes of {src_type} do not exist: {src_ids[bool_mask]}")
-        dst_ids = dst_ids[orig_locs]
+        dst_ids = dst_ids[orig_locs] if len(orig_locs) > 0 else np.array([], dtype=dst_ids.dtype)
     src_ids = new_src_ids
 
     new_dst_ids, orig_locs = node_id_map[dst_type].map_id(dst_ids)
     # If some of the dest nodes don't exist in the node set.
     if len(orig_locs) != len(dst_ids):
         bool_mask = np.ones(len(dst_ids), dtype=bool)
-        bool_mask[orig_locs] = False
+        if len(orig_locs) > 0:
+            bool_mask[orig_locs] = False
         if skip_nonexist_edges:
-            logging.warning("dest nodes of %s do not exist: %s",
-                            dst_type, str(dst_ids[bool_mask]))
+            logging.warning("dest nodes of %s do not exist. Skip %d edges",
+                            dst_type, len(dst_ids[bool_mask]))
         else:
             raise ValueError(f"dest nodes of {dst_type} do not exist: {dst_ids[bool_mask]}")
         # We need to remove the source nodes as well.
-        src_ids = src_ids[orig_locs]
+        src_ids = src_ids[orig_locs] if len(orig_locs) > 0 else np.array([], dtype=src_ids.dtype)
     dst_ids = new_dst_ids
     return src_ids, dst_ids
```

## graphstorm/gconstruct/transform.py

```diff
@@ -16,35 +16,34 @@
     Generate example graph data using built-in datasets for node classifcation,
     node regression, edge classification and edge regression.
 """
 
 import logging
 import os
 import sys
+import abc
 
 import numpy as np
 import torch as th
 
 from scipy.special import erfinv # pylint: disable=no-name-in-module
 from transformers import BertTokenizer
 from transformers import BertModel, BertConfig
 
-from .file_io import HDF5Array, read_index_json
+from .file_io import read_index_json
+from .utils import ExtMemArrayWrapper
 
 def _get_output_dtype(dtype_str):
     if dtype_str == 'float16':
         return np.float16
     elif dtype_str == 'float32':
         return np.float32
     else:
         assert False, f"Unknown dtype {dtype_str}, only support float16 and float32"
 
-def _feat_astype(feats, dtype):
-    return feats.astype(dtype) if dtype is not None else feats
-
 class FeatTransform:
     """ The base class for feature transformation.
 
     Parameters
     ----------
     col_name : str
         The name of the column that contains the feature.
@@ -67,14 +66,71 @@
 
     @property
     def feat_name(self):
         """ The feature name.
         """
         return self._feat_name
 
+    @property
+    def out_dtype(self):
+        """ Output feature dtype
+        """
+        return self._out_dtype
+
+    def __call__(self, feats):
+        """ This transforms the features.
+
+        Parameters
+        ----------
+        feats : Numpy array
+            The feature data
+
+        Returns
+        -------
+        dict : The key is the feature name, the value is the feature.
+        """
+        feats = self.call(feats)
+        return self.as_out_dtype(feats)
+
+    @abc.abstractmethod
+    def call(self, feats):
+        """ This function implements the feature transformation logic
+
+        Parameters
+        ----------
+        feats : Numpy array
+            The feature data
+
+        Returns
+        -------
+        dict : The key is the feature name, the value is the feature.
+        """
+
+    def as_out_dtype(self, feats):
+        """ Convert feats into out_dtype
+            By default (out_dtype is None), it does nothing.
+
+        Parameters
+        ----------
+        feats: Numpy array or dict of Numpy array
+            The feature data
+
+        Returns
+        -------
+        Numpy array or dict: the output feature with dtype of out_dtype
+        """
+        if self.out_dtype is None:
+            return feats
+
+        if isinstance(feats, dict):
+            return {key: feat.astype(self.out_dtype) \
+                        for key, feat in feats.items()}
+        else:
+            return feats.astype(self.out_dtype)
+
 class GlobalProcessFeatTransform(FeatTransform):
     """ The base class for transformations that can only be done using a single process.
 
         Some transformations need to do complex operations on the entire feature set,
         such as ranking. GlobalProcessFeatTransform loads features from files first,
         which can be done with multi-processing, and then do feature transformation
         after features are merged.
@@ -84,16 +140,22 @@
         """ Do feature transformation after features are merged into a single
             array.
 
         Parameters
         ----------
         feats:
             feats to be processed
+
+        Return:
+            np.array: processed feature
         """
 
+    def call(self, feats):
+        raise NotImplementedError
+
 class TwoPhaseFeatTransform(FeatTransform):
     """ The base class for two phasefeature transformation.
 
         The first phase is going to collect global information
         for data processing, e.g., collecting max and min value of floating
         point data or collecting the cardinality of categorical data.
         The second phase is to transform data using
@@ -115,14 +177,17 @@
 
         Parameters
         ----------
         info:
             Information to be collected
         """
 
+    def call(self, feats):
+        raise NotImplementedError
+
 class CategoricalTransform(TwoPhaseFeatTransform):
     """ Convert the data into categorical values.
 
     The categorical values are stored as integers.
 
     Parameters
     ----------
@@ -153,31 +218,33 @@
         feats: np.array
             Data to be processed
         """
         # If the mapping already exists, we don't need to do anything.
         if len(self._val_dict) > 0:
             return {}
 
-        assert isinstance(feats, (np.ndarray, HDF5Array)), \
-            "Feature of CategoricalTransform must be numpy array or HDF5Array"
-        if isinstance(feats, HDF5Array):
+        assert isinstance(feats, (np.ndarray, ExtMemArrayWrapper)), \
+            "Feature of CategoricalTransform must be numpy array or ExtMemArray"
+        if isinstance(feats, ExtMemArrayWrapper):
             # TODO(xiangsx): This is not memory efficient.
             # It will load all data into main memory.
             feats = feats.to_numpy()
 
+        feats = feats[feats != None] # pylint: disable=singleton-comparison
         if self._separator is None:
             return {self.feat_name: np.unique(feats)}
         else:
             assert feats.dtype.type is np.str_, \
                     "We can only convert strings to multiple categorical values with separaters."
             vals = []
             for feat in feats:
                 vals.extend(feat.split(self._separator))
             return {self.feat_name: np.unique(vals)}
 
+
     def update_info(self, info):
         """ Store global information for the second phase data processing
 
         Parameters
         ----------
         info: list
             Information to be collected
@@ -188,32 +255,36 @@
             return
 
         self._val_dict = {key: i for i, key in enumerate(np.unique(np.concatenate(info)))}
         # We need to save the mapping in the config object.
         if self._conf is not None:
             self._conf['mapping'] = self._val_dict
 
-    def __call__(self, feats):
+    def call(self, feats):
         """ Assign IDs to categorical values.
 
         Parameters
         ----------
         feats : np array
             Data with categorical values.
 
         Returns
         -------
         np.array
         """
         encoding = np.zeros((len(feats), len(self._val_dict)), dtype=np.int8)
         if self._separator is None:
             for i, feat in enumerate(feats):
+                if feat is None:
+                    continue
                 encoding[i, self._val_dict[feat]] = 1
         else:
             for i, feat in enumerate(feats):
+                if feat is None:
+                    continue
                 idx = [self._val_dict[val] for val in feat.split(self._separator)]
                 encoding[i, idx] = 1
         return {self.feat_name: encoding}
 
 class NumericalMinMaxTransform(TwoPhaseFeatTransform):
     """ Numerical value with Min-Max normalization.
         $val = (val-min) / (max-min)$
@@ -234,35 +305,44 @@
     """
     def __init__(self, col_name, feat_name,
                  max_bound=sys.float_info.max,
                  min_bound=-sys.float_info.max,
                  out_dtype=None):
         self._max_bound = max_bound
         self._min_bound = min_bound
+        out_dtype = np.float32 if out_dtype is None else out_dtype
         super(NumericalMinMaxTransform, self).__init__(col_name, feat_name, out_dtype)
 
     def pre_process(self, feats):
         """ Pre-process data
 
         Parameters
         ----------
         feats: np.array
             Data to be processed
         """
-        assert isinstance(feats, (np.ndarray, HDF5Array)), \
-            "Feature of NumericalMinMaxTransform must be numpy array or HDF5Array"
-        if isinstance(feats, HDF5Array):
+        assert isinstance(feats, (np.ndarray, ExtMemArrayWrapper)), \
+            "Feature of NumericalMinMaxTransform must be numpy array or ExtMemArray"
+        if isinstance(feats, ExtMemArrayWrapper):
             # TODO(xiangsx): This is not memory efficient.
             # It will load all data into main memory.
             feats = feats.to_numpy()
 
-        assert feats.dtype in [np.float64, np.float32, np.float16, np.int64, \
-                              np.int32, np.int16, np.int8], \
-            "Feature of NumericalMinMaxTransform must be floating points" \
-            "or integers"
+        if feats.dtype not in [np.float64, np.float32, np.float16, np.int64, \
+                              np.int32, np.int16, np.int8]:
+            logging.warning("The feature %s has to be floating points or integers,"
+                            "but get %s. Try to cast it into float32",
+                            self.feat_name, feats.dtype)
+            try:
+                # if input dtype is not float or integer, we need to cast the data
+                # into float32
+                feats = feats.astype(np.float32)
+            except: # pylint: disable=bare-except
+                raise ValueError(f"The feature {self.feat_name} has to be integers or floats.")
+
         assert len(feats.shape) <= 2, "Only support 1D fp feature or 2D fp feature"
         max_val = np.amax(feats, axis=0) if len(feats.shape) == 2 \
             else np.array([np.amax(feats, axis=0)])
         min_val = np.amin(feats, axis=0) if len(feats.shape) == 2 \
             else np.array([np.amin(feats, axis=0)])
 
         max_val[max_val > self._max_bound] = self._max_bound
@@ -289,42 +369,50 @@
             else np.array([np.amax(max_vals, axis=0)])
         min_val = np.amin(min_vals, axis=0) if len(min_vals.shape) == 2 \
             else np.array([np.amin(min_vals, axis=0)])
 
         self._max_val = max_val
         self._min_val = min_val
 
-    def __call__(self, feats):
+    def call(self, feats):
         """ Do normalization for feats
 
         Parameters
         ----------
         feats : np array
             Data to be normalized
 
         Returns
         -------
         np.array
         """
-        assert isinstance(feats, (np.ndarray, HDF5Array)), \
-            "Feature of NumericalMinMaxTransform must be numpy array or HDF5Array"
+        assert isinstance(feats, (np.ndarray, ExtMemArrayWrapper)), \
+            "Feature of NumericalMinMaxTransform must be numpy array or ExtMemArray"
 
         assert not np.any(self._max_val == self._min_val), \
             f"At least one element of Max Val {self._max_val} " \
             f"and Min Val {self._min_val} is equal. This will cause divide by zero error"
 
-        if isinstance(feats, HDF5Array):
+        if isinstance(feats, ExtMemArrayWrapper):
             # TODO(xiangsx): This is not memory efficient.
             # It will load all data into main memory.
             feats = feats.to_numpy()
 
+        if feats.dtype not in [np.float64, np.float32, np.float16, np.int64, \
+                              np.int32, np.int16, np.int8]:
+            try:
+                # if input dtype is not float or integer, we need to cast the data
+                # into float32
+                feats = feats.astype(np.float32)
+            except: # pylint: disable=bare-except
+                raise ValueError(f"The feature {self.feat_name} has to be integers or floats.")
+
         feats = (feats - self._min_val) / (self._max_val - self._min_val)
         feats[feats > 1] = 1 # any value > self._max_val is set to self._max_val
         feats[feats < 0] = 0 # any value < self._min_val is set to self._min_val
-        feats = _feat_astype(feats, self._out_dtype)
 
         return {self.feat_name: feats}
 
 class RankGaussTransform(GlobalProcessFeatTransform):
     """ Use Gauss rank transformation to transform input data
 
         The idea is from
@@ -340,38 +428,57 @@
         The dtype of the transformed feature.
         Default: None, we will not do data type casting.
     epsilon: float
         Epsilon for normalization.
     """
     def __init__(self, col_name, feat_name, out_dtype=None, epsilon=None):
         self._epsilon = epsilon if epsilon is not None else 1e-6
+        out_dtype = np.float32 if out_dtype is None else out_dtype
         super(RankGaussTransform, self).__init__(col_name, feat_name, out_dtype)
 
     def __call__(self, feats):
+        # Overwrite __call__ to avoid cast the feature into out_dtype.
+        # This is not the final output, we should not cast the feature into out_dtype
+        # will cast the feature in after_merge_transform
+        return self.call(feats)
+
+    def call(self, feats):
         # do nothing. Rank Gauss is done after merging all arrays together.
-        assert isinstance(feats, (np.ndarray, HDF5Array)), \
+        assert isinstance(feats, (np.ndarray, ExtMemArrayWrapper)), \
                 f"The feature {self.feat_name} has to be NumPy array."
-        assert np.issubdtype(feats.dtype, np.integer) \
-                or np.issubdtype(feats.dtype, np.floating), \
-                f"The feature {self.feat_name} has to be integers or floats."
 
-        return {self.feat_name: feats}
+        if np.issubdtype(feats.dtype, np.integer) \
+            or np.issubdtype(feats.dtype, np.floating): \
+            return {self.feat_name: feats}
+        else:
+            logging.warning("The feature %s has to be floating points or integers,"
+                            "but get %s. Try to cast it into float32",
+                            self.feat_name, feats.dtype)
+            try:
+                # if input dtype is not float or integer, we need to cast the data
+                # into float32
+                feats = feats.astype(np.float32)
+            except: # pylint: disable=bare-except
+                raise ValueError(f"The feature {self.feat_name} has to be integers or floats.")
+
+            return {self.feat_name: feats}
 
     def after_merge_transform(self, feats):
         # The feats can be a numpy array or a numpy memmaped object
         # Get ranking information.
+        if isinstance(feats, ExtMemArrayWrapper):
+            feats = feats.to_numpy()
         feats = feats.argsort(axis=0).argsort(axis=0)
         feat_range = len(feats) - 1
         # norm to [-1, 1]
         feats = (feats / feat_range - 0.5) * 2
         feats = np.clip(feats, -1 + self._epsilon, 1 - self._epsilon)
         feats = erfinv(feats)
 
-        feats = _feat_astype(feats, self._out_dtype)
-        return feats
+        return self.as_out_dtype(feats)
 
 class Tokenizer(FeatTransform):
     """ A wrapper to a tokenizer.
 
     It is defined to process multiple strings.
 
     Parameters
@@ -386,26 +493,27 @@
         The maximal length of the tokenization results.
     """
     def __init__(self, col_name, feat_name, bert_model, max_seq_length):
         super(Tokenizer, self).__init__(col_name, feat_name)
         self.tokenizer = BertTokenizer.from_pretrained(bert_model)
         self.max_seq_length = max_seq_length
 
-    def __call__(self, strs):
+    def call(self, feats):
         """ Tokenization function.
 
         Parameters
         ----------
         strs : list of strings.
             The text data to be tokenized.
 
         Returns
         -------
         a dict of tokenization results.
         """
+        strs = feats
         tokens = []
         att_masks = []
         type_ids = []
         for s in strs:
             assert isinstance(s, str), "The input of the tokenizer has to be a string."
             t = self.tokenizer(s, max_length=self.max_seq_length,
                                truncation=True, padding='max_length', return_tensors='pt')
@@ -440,14 +548,15 @@
         The inference batch size.
     out_dtype:
         The dtype of the transformed feature.
         Default: None, we will not do data type casting.
     """
     def __init__(self, col_name, feat_name, tokenizer, model_name,
                  infer_batch_size=None, out_dtype=None):
+        out_dtype = np.float32 if out_dtype is None else out_dtype
         super(Text2BERT, self).__init__(col_name, feat_name, out_dtype)
         self.model_name = model_name
         self.lm_model = None
         self.tokenizer = tokenizer
         self.device = None
         self.infer_batch_size = infer_batch_size
 
@@ -459,40 +568,41 @@
         in the master process and passing it to the worker process.
         """
         if th.cuda.is_available():
             gpu = int(os.environ['CUDA_VISIBLE_DEVICES']) \
                     if 'CUDA_VISIBLE_DEVICES' in os.environ else 0
             self.device = f"cuda:{gpu}"
         else:
-            self.device = None
+            self.device = "cpu"
 
         if self.lm_model is None:
             config = BertConfig.from_pretrained(self.model_name)
             lm_model = BertModel.from_pretrained(self.model_name,
                                                  config=config)
             lm_model.eval()
 
             # We use the local GPU to compute BERT embeddings.
             if self.device is not None:
                 lm_model = lm_model.to(self.device)
             self.lm_model = lm_model
 
-    def __call__(self, strs):
+    def call(self, feats):
         """ Compute BERT embeddings of the strings..
 
         Parameters
         ----------
         strs : list of strings.
             The text data.
 
         Returns
         -------
         dict: BERT embeddings.
         """
         self._init()
+        strs = feats
         outputs = self.tokenizer(strs)
         if self.infer_batch_size is not None:
             tokens_list = th.split(th.tensor(outputs['input_ids']), self.infer_batch_size)
             att_masks_list = th.split(th.tensor(outputs['attention_mask']),
                                       self.infer_batch_size)
             token_types_list = th.split(th.tensor(outputs['token_type_ids']),
                                         self.infer_batch_size)
@@ -514,39 +624,50 @@
                                             token_type_ids=token_types.long())
                 out_embs.append(outputs.pooler_output.cpu().numpy())
         if len(out_embs) > 1:
             feats = np.concatenate(out_embs)
         else:
             feats = out_embs[0]
 
-        feats = _feat_astype(feats, self._out_dtype)
         return {self.feat_name: feats}
 
 class Noop(FeatTransform):
     """ This doesn't transform the feature.
+
+    Parameters
+    ----------
+    col_name : str
+        The name of the column that contains the feature.
+    feat_name : str
+        The feature name used in the constructed graph.
+    out_dtype:
+        The dtype of the transformed feature.
+        Default: None, we will not do data type casting.
     """
+    def __init__(self, col_name, feat_name, out_dtype=None):
+        out_dtype = np.float32 if out_dtype is None else out_dtype
+        super(Noop, self).__init__(col_name, feat_name, out_dtype)
 
-    def __call__(self, feats):
+    def call(self, feats):
         """ This transforms the features.
 
         Parameters
         ----------
         feats : Numpy array
             The feature data
 
         Returns
         -------
         dict : The key is the feature name, the value is the feature.
         """
-        assert isinstance(feats, (np.ndarray, HDF5Array)), \
+        assert isinstance(feats, (np.ndarray, ExtMemArrayWrapper)), \
                 f"The feature {self.feat_name} has to be NumPy array."
         assert np.issubdtype(feats.dtype, np.integer) \
                 or np.issubdtype(feats.dtype, np.floating), \
                 f"The feature {self.feat_name} has to be integers or floats."
-        feats = _feat_astype(feats, self._out_dtype)
         return {self.feat_name: feats}
 
 def parse_feat_ops(confs):
     """ Parse the configurations for processing the features
 
     The feature transformation:
     {
@@ -567,14 +688,15 @@
     ops = []
     assert isinstance(confs, list), \
             "The feature configurations need to be in a list."
     for feat in confs:
         assert 'feature_col' in feat, \
                 "'feature_col' must be defined in a feature field."
         feat_name = feat['feature_name'] if 'feature_name' in feat else feat['feature_col']
+
         out_dtype = _get_output_dtype(feat['out_dtype']) if 'out_dtype' in feat else None
         if 'transform' not in feat:
             transform = Noop(feat['feature_col'], feat_name, out_dtype=out_dtype)
         else:
             conf = feat['transform']
             assert 'name' in conf, "'name' must be defined in the transformation field."
             if conf['name'] == 'tokenize_hf':
@@ -615,15 +737,24 @@
             elif conf['name'] == 'to_categorical':
                 separator = conf['separator'] if 'separator' in conf else None
                 transform = CategoricalTransform(feat['feature_col'], feat_name,
                                                  separator=separator, transform_conf=conf)
             else:
                 raise ValueError('Unknown operation: {}'.format(conf['name']))
         ops.append(transform)
-    return ops
+
+    two_phase_feat_ops = []
+    after_merge_feat_ops = {}
+    for op in ops:
+        if isinstance(op, TwoPhaseFeatTransform):
+            two_phase_feat_ops.append(op)
+        if isinstance(op, GlobalProcessFeatTransform):
+            after_merge_feat_ops[op.feat_name] = op
+
+    return ops, two_phase_feat_ops, after_merge_feat_ops
 
 def preprocess_features(data, ops):
     """ Pre-process the data with the specified operations.
 
     This function runs the input pre-process operations on the corresponding data
     and returns the pre-process results. An example of preprocessing is getting
     the cardinality of a categorical feature.
@@ -668,15 +799,15 @@
     new_data = {}
     for op in ops:
         res = op(data[op.col_name])
         assert isinstance(res, dict)
         for key, val in res.items():
             # Check if has 1D features. If yes, convert to 2D features
             if len(val.shape) == 1:
-                if isinstance(val, HDF5Array):
+                if isinstance(val, ExtMemArrayWrapper):
                     val = val.to_numpy().reshape(-1, 1)
                 else:
                     val = val.reshape(-1, 1)
             new_data[key] = val
     return new_data
 
 def get_valid_label_index(label):
@@ -712,66 +843,71 @@
 
     Parameters
     ----------
     col_name : str
         The column name for labels.
     label_name : str
         The label name.
+    id_col : str
+        The name of the ID column.
     task_type : str
         The task type.
     train_idx : Numpy array
         The array that contains the index of training data points.
     val_idx : Numpy array
         The array that contains the index of validation data points.
     test_idx : Numpy array
         The array that contains the index of test data points.
     """
-    def __init__(self, col_name, label_name, task_type,
+    def __init__(self, col_name, label_name, id_col, task_type,
                  train_idx=None, val_idx=None, test_idx=None):
+        self._id_col = id_col
         self._col_name = col_name
         self._label_name = label_name
-        self._train_idx = train_idx
-        self._val_idx = val_idx
-        self._test_idx = test_idx
+        self._train_idx = set(train_idx.tolist()) if train_idx is not None else None
+        self._val_idx = set(val_idx.tolist()) if val_idx is not None else None
+        self._test_idx = set(test_idx.tolist()) if test_idx is not None else None
         self._task_type = task_type
 
     @property
     def col_name(self):
         """ The column name that contains the label.
         """
         return self._col_name
 
     @property
     def label_name(self):
         """ The label name.
         """
         return self._label_name
 
-    def data_split(self, num_samples):
+    def data_split(self, ids):
         """ Split the data for training/validation/test.
 
         Parameters
         ----------
-        num_samples : int
-            The total number of data points.
+        ids : numpy array
+            The array of IDs.
 
         Returns
         -------
         dict of Numpy array
             The arrays for training/validation/test masks.
         """
+        num_samples = len(ids)
         train_mask = np.zeros((num_samples,), dtype=np.int8)
         val_mask = np.zeros((num_samples,), dtype=np.int8)
         test_mask = np.zeros((num_samples,), dtype=np.int8)
-        if self._train_idx is not None:
-            train_mask[self._train_idx] = 1
-        if self._val_idx is not None:
-            val_mask[self._val_idx] = 1
-        if self._test_idx is not None:
-            test_mask[self._test_idx] = 1
+        for i, idx in enumerate(ids):
+            if self._train_idx is not None and idx in self._train_idx:
+                train_mask[i] = 1
+            elif self._val_idx is not None and idx in self._val_idx:
+                val_mask[i] = 1
+            elif self._test_idx is not None and idx in self._test_idx:
+                test_mask[i] = 1
         train_mask_name = 'train_mask'
         val_mask_name = 'val_mask'
         test_mask_name = 'test_mask'
         return {train_mask_name: train_mask,
                 val_mask_name: val_mask,
                 test_mask_name: test_mask}
 
@@ -785,24 +921,18 @@
         data : dict of Tensors
             All data associated with nodes/edges of a node/edge type.
 
         Returns
         -------
         dict of Tensors : it contains the labels as well as training/val/test splits.
         """
-        if self.col_name in data:
-            label = data[self.col_name]
-            num_samples = len(label)
-        else:
-            assert len(data) > 0, "The edge data is empty."
-            label = None
-            for val in data.values():
-                num_samples = len(val)
-                break
-        res = self.data_split(num_samples)
+        label = data[self.col_name] if self.col_name in data else None
+        assert self._id_col in data, \
+                f"The input data does not have ID column {self._id_col}."
+        res = self.data_split(data[self._id_col])
         if label is not None and self._task_type == "classification":
             res[self.label_name] = np.int32(label)
         elif label is not None:
             res[self.label_name] = label
         return res
 
 class LabelProcessor:
@@ -969,28 +1099,30 @@
     is_node : bool
         Whether the configurations are defined for nodes.
 
     Returns
     -------
     list of LabelProcessor : the label processors generated from the configurations.
     """
-    assert len(confs) == 1, "We only support one label per node/edge type."
-    label_conf = confs[0]
+    label_confs = confs['labels']
+    assert len(label_confs) == 1, "We only support one label per node/edge type."
+    label_conf = label_confs[0]
     assert 'task_type' in label_conf, "'task_type' must be defined in the label field."
     task_type = label_conf['task_type']
     if 'custom_split_filenames' in label_conf:
         custom_split = label_conf['custom_split_filenames']
         assert isinstance(custom_split, dict), \
                 "Custom data split needs to provide train/val/test index."
         train_idx = read_index_json(custom_split['train']) if 'train' in custom_split else None
         val_idx = read_index_json(custom_split['valid']) if 'valid' in custom_split else None
         test_idx = read_index_json(custom_split['test']) if 'test' in custom_split else None
         label_col = label_conf['label_col'] if 'label_col' in label_conf else None
-        return [CustomLabelProcessor(label_col, label_col, task_type,
-                                     train_idx, val_idx, test_idx)]
+        assert "node_id_col" in confs, "Custom data split only works for nodes."
+        return [CustomLabelProcessor(label_col, label_col, confs["node_id_col"],
+                                     task_type, train_idx, val_idx, test_idx)]
 
     if 'split_pct' in label_conf:
         split_pct = label_conf['split_pct']
     else:
         logging.info("'split_pct' is not found. " + \
                 "Use the default data split: train(80%), valid(10%), test(10%).")
         split_pct = [0.8, 0.1, 0.1]
```

## graphstorm/gconstruct/utils.py

```diff
@@ -16,23 +16,24 @@
     Generate example graph data using built-in datasets for node classifcation,
     node regression, edge classification and edge regression.
 """
 import os
 import queue
 import gc
 import logging
+import copy
+import traceback
 
 import numpy as np
 import dgl
 import torch as th
 from torch import multiprocessing
 from torch.multiprocessing import Process
 
 from ..utils import sys_tracker
-from .file_io import HDF5Array
 
 SHARED_MEM_OBJECT_THRESHOLD = 1.9 * 1024 * 1024 * 1024 # must < 2GB
 SHARED_MEMORY_CROSS_PROCESS_STORAGE = "shared_memory"
 PICKLE_CROSS_PROCESS_STORAGE = "pickle"
 
 def _to_shared_memory(data):
     """ Move all tensor objects into torch shared memory
@@ -160,14 +161,15 @@
     if th.cuda.is_available():
         num_gpus = th.cuda.device_count()
         gpu = worker_id % num_gpus
         os.environ['CUDA_VISIBLE_DEVICES'] = str(gpu)
         if worker_id >= num_gpus:
             logging.warning("There are more than 1 processes are attachd to GPU %d.", gpu)
     try:
+        i = 0
         while True:
             # If the queue is empty, it will raise the Empty exception.
             i, in_file = task_queue.get_nowait()
             logging.debug("%d Processing %s", worker_id, in_file)
             data = user_parser(in_file)
             size = _estimate_sizeof(data)
             # Max pickle obj size is 2 GByte
@@ -178,14 +180,17 @@
                 data = (SHARED_MEMORY_CROSS_PROCESS_STORAGE, _to_shared_memory(data))
             else:
                 data = (PICKLE_CROSS_PROCESS_STORAGE, data)
             res_queue.put((i, data))
             gc.collect()
     except queue.Empty:
         pass
+    except Exception as e:  # pylint: disable=broad-exception-caught
+        e = ''.join(traceback.TracebackException.from_exception(e).format())
+        res_queue.put((i, e))
 
 def update_two_phase_feat_ops(phase_one_info, ops):
     """ Update the ops for the second phase feat processing
 
     Parameters
     ----------
     phase_one_info: dict
@@ -242,14 +247,18 @@
             proc = Process(target=worker_fn, args=(i, task_queue, res_queue, user_parser))
             proc.start()
             processes.append(proc)
 
         return_dict = {}
         while len(return_dict) < num_files:
             file_idx, vals= res_queue.get()
+            if not isinstance(vals, tuple):
+                logging.error("Processing file %d fails.", file_idx)
+                logging.error(vals)
+                raise RuntimeError("One of the worker processes fails. Stop processing.")
             # If the size of `vals`` is larger than utils.SHARED_MEM_OBJECT_THRESHOLD
             # we will automatically convert tensors in `vals` into torch tensor
             # and copy the tensor into shared memory.
             # This helps avoid the pickle max obj size issue.
             storage_type, vals = vals
             if storage_type == SHARED_MEMORY_CROSS_PROCESS_STORAGE:
                 vals = _to_numpy_array(vals)
@@ -282,14 +291,249 @@
     shape1 = arrs[0].shape[1:]
     for arr in arrs:
         num_rows += arr.shape[0]
         assert shape1 == arr.shape[1:]
     shape = [num_rows] + list(shape1)
     return tuple(shape)
 
+def _get_arrs_out_dtype(arrs):
+    """ To get the output dtype by accessing the
+        first element of the arrays (numpy array or HDFArray)
+
+        Note: We use arrs[0][0] instead of arrs[0] because
+            arrs[0][0] is a transformed data with out_dtype
+            while arrs[0] can be a HDFArray and has not
+            been cast to out_dtype.
+
+    Parameters
+    ----------
+    arrs : list of arrays.
+        The input arrays.
+    """
+    return arrs[0][0].dtype
+
+class ExtMemArrayWrapper:
+    """ An array wrapper for external-memory array.
+    """
+
+    def to_numpy(self):
+        """ Convert the array to Numpy array.
+        """
+
+    def to_tensor(self):
+        """ Return Pytorch tensor.
+        """
+
+    def astype(self, dtype):
+        """ Set the output dtype.
+
+        Parameters
+        ----------
+        dtype: numpy.dtype
+            Output dtype
+        """
+
+    def cleanup(self):
+        """ Clean up the external-memory array.
+        """
+
+    @property
+    def shape(self):
+        """ The shape of the array.
+        """
+
+    @property
+    def dtype(self):
+        """ The data type of the array.
+        """
+
+class HDF5Handle:
+    """ HDF5 file handle
+
+    This is to reference the HDF5 handle and close it when no one
+    uses the HDF5 file.
+
+    Parameters
+    ----------
+    f : HDF5 file handle
+        The handle to access the HDF5 file.
+    """
+    def __init__(self, f):
+        self._f = f
+
+    def __del__(self):
+        return self._f.close()
+
+
+class HDF5Array(ExtMemArrayWrapper):
+    """ This is an array wrapper class for HDF5 array.
+
+    The main purpose of this class is to make sure that we can close
+    the HDF5 files when the array is destroyed.
+
+    Parameters
+    ----------
+    arr : HDF5 dataset
+        The array-like object for accessing the HDF5 file.
+    handle : HDF5Handle
+        The handle that references to the opened HDF5 file.
+    """
+    def __init__(self, arr, handle):
+        self._arr = arr
+        self._handle = handle
+        self._out_dtype = None # Use the dtype of self._arr
+
+    def __len__(self):
+        return self._arr.shape[0]
+
+    def __getitem__(self, idx):
+        """ Slicing data from the array.
+
+        Parameters
+        ----------
+        idx : Numpy array or Pytorch tensor or slice or int.
+            The index.
+
+        Returns
+        -------
+        Numpy array : the data from the HDF5 array indexed by `idx`.
+        """
+        if isinstance(idx, (slice, int)):
+            return self._arr[idx].astype(self._out_dtype)
+
+        if isinstance(idx, th.Tensor):
+            idx = idx.numpy()
+        # If the idx are sorted.
+        if np.all(idx[1:] - idx[:-1] > 0):
+            arr = self._arr[idx]
+        else:
+            # There are two cases here: 1) there are duplicated IDs,
+            # 2) the IDs are not sorted. Unique can return unique
+            # IDs in the ascending order that meets the requirement of
+            # HDF5 indexing.
+            uniq_ids, reverse_idx = np.unique(idx, return_inverse=True)
+            arr = self._arr[uniq_ids][reverse_idx]
+
+        if self._out_dtype is not None:
+            arr = arr.astype(self._out_dtype)
+        return arr
+
+    def to_tensor(self):
+        """ Return Pytorch tensor.
+        """
+        arr = th.tensor(self._arr)
+        if self._out_dtype is not None:
+            if self._out_dtype is np.float32:
+                arr = arr.to(th.float32)
+            elif self._out_dtype is np.float16:
+                arr = arr.to(th.float16)
+        return arr
+
+    def to_numpy(self):
+        """ Return Numpy array.
+        """
+        res = self._arr[:]
+        if self._out_dtype is not None:
+            res = res.astype(self._out_dtype)
+        return res
+
+    def astype(self, dtype):
+        """ Set the output dtype.
+
+        Parameters
+        ----------
+        dtype: numpy.dtype
+            Output dtype
+        """
+        arr = copy.copy(self)
+        arr._out_dtype = dtype
+        return arr
+
+    @property
+    def shape(self):
+        """ The shape of the HDF5 array.
+        """
+        return self._arr.shape
+
+    @property
+    def dtype(self):
+        """ The data type of the HDF5 array.
+        """
+        if self._out_dtype is not None:
+            return self._out_dtype
+        else:
+            return self._arr.dtype
+
+class ExtNumpyWrapper(ExtMemArrayWrapper):
+    """ The wrapper to memory-mapped Numpy array.
+
+    Parameters
+    ----------
+    arr_path : str
+        The path of memory-mapped numpy file.
+    shape : tuple
+        The shape of the array.
+    dtype : numpy dtype
+        The data type.
+    """
+    def __init__(self, arr_path, shape, dtype):
+        self._arr_path = arr_path
+        self._shape = shape
+        self._orig_dtype = self._dtype = dtype
+        self._arr = None
+
+    @property
+    def dtype(self):
+        """ The data type
+        """
+        return self._dtype
+
+    @property
+    def shape(self):
+        """ The shape of the array.
+        """
+        return self._shape
+
+    def astype(self, dtype):
+        """ Return an array with converted data type.
+        """
+        arr = copy.copy(self)
+        arr._dtype = dtype
+        return arr
+
+    def __len__(self):
+        return self._shape[0]
+
+    def __getitem__(self, idx):
+        if self._arr is None:
+            self._arr = np.memmap(self._arr_path, self._orig_dtype, mode="r", shape=self._shape)
+        return self._arr[idx].astype(self.dtype)
+
+    def cleanup(self):
+        """ Clean up the array.
+        """
+        self._arr.flush()
+        self._arr = None
+
+    def to_numpy(self):
+        """ Convert the data to Numpy array.
+        """
+        if self._arr is None:
+            arr = np.memmap(self._arr_path, self._orig_dtype, mode="r", shape=self._shape)
+            if self._dtype != self._orig_dtype:
+                arr = arr.astype(self._dtype)
+            return arr
+        else:
+            return self._arr.astype(self._dtype)
+
+    def to_tensor(self):
+        """ Return Pytorch tensor.
+        """
+        return th.tensor(self.to_numpy())
+
 def _merge_arrs(arrs, tensor_path):
     """ Merge the arrays.
 
     The merged array may be stored in a file specified by the path.
 
     Parameters
     ----------
@@ -300,23 +544,26 @@
 
     Returns
     -------
     Numpy array : the merged array.
     """
     assert isinstance(arrs, list)
     shape = _get_tot_shape(arrs)
-    dtype = arrs[0].dtype
+
+    # To get the output dtype or arrs
+    dtype = _get_arrs_out_dtype(arrs)
     if tensor_path is not None:
         out_arr = np.memmap(tensor_path, dtype, mode="w+", shape=shape)
         row_idx = 0
         for arr in arrs:
             out_arr[row_idx:(row_idx + arr.shape[0])] = arr[:]
             row_idx += arr.shape[0]
-        return out_arr
-    elif isinstance(arrs[0], HDF5Array):
+        out_arr.flush()
+        return ExtNumpyWrapper(tensor_path, out_arr.shape, out_arr.dtype)
+    elif isinstance(arrs[0], ExtMemArrayWrapper):
         arrs = [arr.to_numpy() for arr in arrs]
         return np.concatenate(arrs)
     else:
         return np.concatenate(arrs)
 
 class ExtMemArrayMerger:
     """ Merge multiple Numpy arrays.
@@ -354,32 +601,35 @@
         Numpy array : an array stored in external memory.
         """
         assert isinstance(arrs, list)
         shape = _get_tot_shape(arrs)
         # If external memory workspace is not initialized or the feature size is smaller
         # than a threshold, we don't do anything.
         if self._ext_mem_workspace is None or np.prod(shape[1:]) < self._ext_mem_feat_size:
-            if len(arrs) == 1 and isinstance(arrs[0], HDF5Array):
+            if len(arrs) == 1 and isinstance(arrs[0], ExtMemArrayWrapper):
                 return arrs[0].to_numpy()
             elif len(arrs) == 1:
                 return arrs[0]
             else:
                 return _merge_arrs(arrs, None)
 
         # We need to create the workspace directory if it doesn't exist.
         os.makedirs(self._ext_mem_workspace, exist_ok=True)
         tensor_path = os.path.join(self._ext_mem_workspace, name + ".npy")
         self._tensor_files.append(tensor_path)
         if len(arrs) > 1:
             return _merge_arrs(arrs, tensor_path)
         else:
+            # To get the output dtype or arrs
+            dtype = _get_arrs_out_dtype(arrs)
             arr = arrs[0]
-            em_arr = np.memmap(tensor_path, arr.dtype, mode="w+", shape=shape)
+            em_arr = np.memmap(tensor_path, dtype, mode="w+", shape=shape)
             em_arr[:] = arr[:]
-            return em_arr
+            em_arr.flush()
+            return ExtNumpyWrapper(tensor_path, em_arr.shape, em_arr.dtype)
 
 def save_maps(output_dir, fname, map_data):
     """ Save node id mapping or edge id mapping
 
     Parameters
     ----------
     output_dir : str
```

## graphstorm/inference/ep_infer.py

```diff
@@ -66,14 +66,19 @@
         node_id_mapping_file: str
             Path to the file storing node id mapping generated by the
             graph partition algorithm.
         return_proba: bool
             Whether to return all the predictions or the maximum prediction.
         """
         do_eval = self.evaluator is not None
+        if do_eval:
+            assert loader.data.labels is not None, \
+                "A label field must be provided for edge classification or regression " \
+                "when evaluation is required."
+
         sys_tracker.check('start inferencing')
         self._model.eval()
         embs = do_full_graph_inference(self._model, loader.data, fanout=loader.fanout,
                                        task_tracker=self.task_tracker)
         sys_tracker.check('compute embeddings')
         res = edge_mini_batch_predict(self._model, embs, loader, return_proba,
                                       return_label=do_eval)
@@ -94,16 +99,15 @@
             sys_tracker.check('run evaluation')
             if self.rank == 0:
                 self.log_print_metrics(val_score=val_score,
                                        test_score=test_score,
                                        dur_eval=time.time() - test_start,
                                        total_steps=0)
 
-        device = th.device(f"cuda:{self.dev_id}") \
-            if self.dev_id >= 0 else th.device("cpu")
+        device = self.device
 
         if save_embed_path is not None:
             target_ntypes = set()
             for etype in infer_data.eval_etypes:
                 target_ntypes.add(etype[0])
                 target_ntypes.add(etype[2])
```

## graphstorm/inference/graphstorm_infer.py

```diff
@@ -27,34 +27,30 @@
         The GNN model for node prediction.
     rank : int
         The rank.
     """
     def __init__(self, model, rank):
         self._model = model
         self._rank = rank
-        self._dev_id = -1
+        self._device = -1
         self._evaluator = None
         self._task_tracker = None
 
-    def setup_cuda(self, dev_id):
-        """ Set up the CUDA device of this trainer.
+    def setup_device(self, device):
+        """ Set up the device for the inference.
 
         The CUDA device is set up based on the local rank.
 
         Parameters
         ----------
-        dev_id : int
-            The device ID for model training.
+        device :
+            The device for inference.
         """
-        # setup cuda env
-        use_cuda = th.cuda.is_available()
-        assert use_cuda, "Only support GPU training"
-        th.cuda.set_device(dev_id)
-        self._dev_id = dev_id
-        self._model = self._model.to(self.dev_id)
+        self._device = th.device(device)
+        self._model = self._model.to(self.device)
 
     def setup_task_tracker(self, task_tracker):
         """ Set the task tracker.
 
         Parameters
         ----------
         task_tracker : GSTaskTracker
@@ -109,17 +105,17 @@
     @property
     def task_tracker(self):
         """ Get the task tracker associated with the inference.
         """
         return self._task_tracker
 
     @property
-    def dev_id(self):
-        """ Get the device ID associated with the inference.
+    def device(self):
+        """ The device associated with the inference.
         """
-        return self._dev_id
+        return self._device
 
     @property
     def rank(self):
         """ Get the rank the inference.
         """
         return self._rank
```

## graphstorm/inference/lp_infer.py

```diff
@@ -69,16 +69,15 @@
         """
         sys_tracker.check('start inferencing')
         self._model.eval()
         embs = do_full_graph_inference(self._model, data, fanout=loader.fanout,
                                        edge_mask=edge_mask_for_gnn_embeddings,
                                        task_tracker=self.task_tracker)
         sys_tracker.check('compute embeddings')
-        device = th.device(f"cuda:{self.dev_id}") \
-                if self.dev_id >= 0 else th.device("cpu")
+        device = self.device
         if save_embed_path is not None:
             save_gsgnn_embeddings(save_embed_path, embs, self.rank,
                 th.distributed.get_world_size(),
                 device=device,
                 node_id_mapping_file=node_id_mapping_file)
         th.distributed.barrier()
         sys_tracker.check('save embeddings')
```

## graphstorm/inference/np_infer.py

```diff
@@ -67,14 +67,19 @@
         node_id_mapping_file: str
             Path to the file storing node id mapping generated by the
             graph partition algorithm.
         return_proba: bool
             Whether to return all the predictions or the maximum prediction.
         """
         do_eval = self.evaluator is not None
+        if do_eval:
+            assert loader.data.labels is not None, \
+                "A label field must be provided for node classification " \
+                "or regression inference when evaluation is required."
+
         sys_tracker.check('start inferencing')
         self._model.eval()
         # TODO support multiple ntypes
         assert len(loader.data.eval_ntypes) == 1, \
             "GraphStorm only support single target node type for training and inference"
         ntype = loader.data.eval_ntypes[0]
 
@@ -91,16 +96,15 @@
                                            task_tracker=self.task_tracker)
             res = node_mini_batch_predict(self._model, embs, loader, return_proba,
                                           return_label=do_eval)
             pred = res[0]
             label = res[1] if do_eval else None
         sys_tracker.check('compute embeddings')
 
-        device = th.device(f"cuda:{self.dev_id}") \
-                if self.dev_id >= 0 else th.device("cpu")
+        device = self.device
 
         # do evaluation first
         # do evaluation if any
         if do_eval:
             test_start = time.time()
             val_score, test_score = self.evaluator.evaluate(pred, pred, label, label, 0)
             sys_tracker.check('run evaluation')
```

## graphstorm/model/edge_gnn.py

```diff
@@ -171,14 +171,15 @@
     with th.no_grad():
         for input_nodes, batch_graph, blocks in loader:
             if not isinstance(input_nodes, dict):
                 assert len(g.ntypes) == 1
                 input_nodes = {g.ntypes[0]: input_nodes}
             input_feats = data.get_node_feats(input_nodes, device)
             blocks = [block.to(device) for block in blocks]
+            batch_graph = batch_graph.to(device)
             pred = model.predict(blocks, batch_graph, input_feats, None, input_nodes,
                                  return_proba)
             preds.append(pred.cpu())
 
             if return_label:
                 # retrieving seed edge id from the graph to find labels
                 # TODO(zhengda) expand code for multiple edge types
@@ -222,14 +223,20 @@
         otherwise return the maximum result.
     Tensor : labels if return_labels is True
     """
     # find the target src and dst ntypes
     model.eval()
     decoder = model.decoder
     data = loader.data
+
+    if return_label:
+        assert data.labels is not None, \
+            "Return label is required, but the label field is not provided whem" \
+            "initlaizing the inference dataset."
+
     with th.no_grad():
         # save preds and labels together in order not to shuffle
         # the order when gather tensors from other trainers
         preds_list = []
         labels_list = []
         device = model.device
         for input_nodes, batch_graph, _ in loader:
@@ -253,8 +260,8 @@
         preds = th.cat(preds_list)
     th.distributed.barrier()
 
     model.train()
     if return_label:
         return preds, th.cat(labels_list)
     else:
-        return preds
+        return preds, None
```

## graphstorm/model/embed.py

```diff
@@ -13,19 +13,21 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Embedding layer implementation
 """
 import torch as th
 from torch import nn
+import torch.nn.functional as F
 from dgl.distributed import DistEmbedding, DistTensor, node_split
 
 from .gs_layer import GSLayer
 from ..dataloading.dataset import prepare_batch_input
 from ..utils import get_rank
+from .ngnn_mlp import NGNNMLP
 
 def init_emb(shape, dtype):
     """Create a tensor with the given shape and date type.
 
     This function is used to initialize the data in the distributed embedding layer
     and set their value with uniformly random values.
 
@@ -155,22 +157,26 @@
     activation : func
         The activation function
     dropout : float
         The dropout parameter
     use_node_embeddings : bool
         Whether we will use the node embeddings for individual nodes even when node features are
         available.
+    num_ffn_layers_in_input: int, optional
+        Number of layers of feedforward neural network for each node type in the input layers
     """
     def __init__(self,
                  g,
                  feat_size,
                  embed_size,
                  activation=None,
                  dropout=0.0,
-                 use_node_embeddings=False):
+                 use_node_embeddings=False,
+                 num_ffn_layers_in_input=0,
+                 ffn_activation=F.relu):
         super(GSNodeEncoderInputLayer, self).__init__(g)
         self.embed_size = embed_size
         self.activation = activation
         self.dropout = nn.Dropout(dropout)
         self.use_node_embeddings = use_node_embeddings
 
         # create weight embeddings for each node for each relation
@@ -210,14 +216,21 @@
                 self.proj_matrix[ntype] = proj_matrix
                 self._sparse_embeds[ntype] = DistEmbedding(g.number_of_nodes(ntype),
                                 self.embed_size,
                                 embed_name + '_' + ntype,
                                 init_emb,
                                 part_policy=part_policy)
 
+        # ngnn
+        self.num_ffn_layers_in_input = num_ffn_layers_in_input
+        self.ngnn_mlp = nn.ModuleDict({})
+        for ntype in g.ntypes:
+            self.ngnn_mlp[ntype] = NGNNMLP(embed_size, embed_size,
+                            num_ffn_layers_in_input, ffn_activation, dropout)
+
     def forward(self, input_feats, input_nodes):
         """Forward computation
 
         Parameters
         ----------
         input_feats: dict
             input features
@@ -255,14 +268,20 @@
                 emb = self.sparse_embeds[ntype](input_nodes[ntype], device)
                 emb = emb @ self.proj_matrix[ntype]
             if self.activation is not None:
                 emb = self.activation(emb)
             emb = self.dropout(emb)
             embs[ntype] = emb
 
+        def _apply(t, h):
+            if self.num_ffn_layers_in_input > 0:
+                h = self.ngnn_mlp[t](h)
+            return h
+
+        embs = {ntype: _apply(ntype, h) for ntype, h in embs.items()}
         return embs
 
     def get_sparse_params(self):
         """ get the sparse parameters.
 
         Returns
         -------
```

## graphstorm/model/gnn_encoder_base.py

```diff
@@ -11,22 +11,22 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Relational GNN
 """
-import tqdm
-
 import dgl
 import torch as th
 from torch import nn
 from dgl.distributed import DistTensor, node_split
 from .gs_layer import GSLayer
 
+from ..utils import get_rank
+
 class GraphConvEncoder(GSLayer):     # pylint: disable=abstract-method
     r"""General encoder for graph data.
 
     Parameters
     ----------
     h_dim : int
         Hidden dimension
@@ -121,15 +121,19 @@
             fanout_i = [-1] if fanout is None or len(fanout) == 0 else [fanout[i]]
             sampler = dgl.dataloading.MultiLayerNeighborSampler(fanout_i, mask=edge_mask)
             dataloader = dgl.dataloading.DistNodeDataLoader(g, infer_nodes, sampler,
                                                             batch_size=batch_size,
                                                             shuffle=False,
                                                             drop_last=False)
 
-            for iter_l, (input_nodes, output_nodes, blocks) in enumerate(tqdm.tqdm(dataloader)):
+            for iter_l, (input_nodes, output_nodes, blocks) in enumerate(dataloader):
+                if iter_l % 100000 == 0 and get_rank() == 0:
+                    print(f"[Rank 0] dist_inference: Layer [{i}] " \
+                          f"finishes [{iter_l}] iterations.")
+
                 if task_tracker is not None:
                     task_tracker.keep_alive(report_step=iter_l)
                 block = blocks[0].to(device)
                 if not isinstance(input_nodes, dict):
                     # This happens on a homogeneous graph.
                     assert len(g.ntypes) == 1
                     input_nodes = {g.ntypes[0]: input_nodes}
```

## graphstorm/model/node_gnn.py

```diff
@@ -166,14 +166,20 @@
     Tensor : GNN embeddings.
     Tensor : labels if return_labels is True
     """
     device = model.device
     data = loader.data
     g = data.g
     preds = []
+
+    if return_label:
+        assert data.labels is not None, \
+            "Return label is required, but the label field is not provided whem" \
+            "initlaizing the inference dataset."
+
     embs = []
     labels = []
     model.eval()
     with th.no_grad():
         for input_nodes, seeds, blocks in loader:
             if not isinstance(input_nodes, dict):
                 assert len(g.ntypes) == 1
@@ -191,15 +197,15 @@
     model.train()
     preds = th.cat(preds)
     embs = th.cat(embs)
     if return_label:
         labels = th.cat(labels)
         return preds, embs, labels
     else:
-        return preds, embs
+        return preds, embs, None
 
 def node_mini_batch_predict(model, emb, loader, return_proba=True, return_label=False):
     """ Perform mini-batch prediction.
 
     Parameters
     ----------
     model : GSgnnModel
@@ -216,14 +222,20 @@
     Returns
     -------
     Tensor : GNN prediction results.
     Tensor : labels if return_labels is True
     """
     device = model.device
     data = loader.data
+
+    if return_label:
+        assert data.labels is not None, \
+            "Return label is required, but the label field is not provided whem" \
+            "initlaizing the inference dataset."
+
     preds = []
     labels = []
     # TODO(zhengda) I need to check if the data loader only returns target nodes.
     model.eval()
     with th.no_grad():
         for input_nodes, seeds, _ in loader:
             assert len(input_nodes) == 1, "Currently we only support one node type"
@@ -240,8 +252,8 @@
     model.train()
 
     preds = th.cat(preds)
     if return_label:
         labels = th.cat(labels)
         return preds, labels
     else:
-        return preds
+        return preds, None
```

## graphstorm/model/rgat_encoder.py

```diff
@@ -18,16 +18,18 @@
 import warnings
 
 import torch as th
 from torch import nn
 import torch.nn.functional as F
 import dgl.nn as dglnn
 
+from .ngnn_mlp import NGNNMLP
 from .gnn_encoder_base import GraphConvEncoder
 
+
 class RelationalAttLayer(nn.Module):
     r"""Relational graph attention layer.
 
     For inner relation message aggregation we use multi-head attention network.
     For cross relation message we just use average
 
     Parameters
@@ -44,25 +46,31 @@
         True if bias is added. Default: True
     activation : callable, optional
         Activation function. Default: None
     self_loop : bool, optional
         True to include self loop message. Default: False
     dropout : float, optional
         Dropout rate. Default: 0.0
+    num_ffn_layers_in_gnn: int, optional
+        Number of layers of ngnn between gnn layers
+    ffn_actication: torch.nn.functional
+        Activation Method for ngnn
     """
     def __init__(self,
                  in_feat,
                  out_feat,
                  rel_names,
                  num_heads,
                  *,
                  bias=True,
                  activation=None,
                  self_loop=False,
-                 dropout=0.0):
+                 dropout=0.0,
+                 num_ffn_layers_in_gnn=0,
+                 fnn_activation=F.relu):
         super(RelationalAttLayer, self).__init__()
         self.in_feat = in_feat
         self.out_feat = out_feat
         self.rel_names = rel_names
         self.bias = bias
         self.activation = activation
         self.self_loop = self_loop
@@ -79,14 +87,20 @@
 
         # weight for self loop
         if self.self_loop:
             self.loop_weight = nn.Parameter(th.Tensor(in_feat, out_feat))
             nn.init.xavier_uniform_(self.loop_weight,
                                     gain=nn.init.calculate_gain('relu'))
 
+        # ngnn
+        self.num_ffn_layers_in_gnn = num_ffn_layers_in_gnn
+        self.ngnn_mlp = NGNNMLP(out_feat, out_feat,
+                                     num_ffn_layers_in_gnn, fnn_activation, dropout)
+
+        # dropout
         self.dropout = nn.Dropout(dropout)
 
     # pylint: disable=invalid-name
     def forward(self, g, inputs):
         """Forward computation
 
         Parameters
@@ -114,14 +128,16 @@
         def _apply(ntype, h):
             if self.self_loop:
                 h = h + th.matmul(inputs_dst[ntype], self.loop_weight)
             if self.bias:
                 h = h + self.h_bias
             if self.activation:
                 h = self.activation(h)
+            if self.num_ffn_layers_in_gnn > 0:
+                h = self.ngnn_mlp(h)
             return self.dropout(h)
 
         for k, _ in inputs.items():
             if g.number_of_dst_nodes(k) > 0:
                 if k not in hs:
                     warnings.warn("Warning. Graph convolution returned empty "
                           f"dictionary, for node with type: {str(k)}")
@@ -150,30 +166,34 @@
         Num hidden layers
     dropout: float
         Dropout
     use_self_loop: bool
         Self loop
     last_layer_act: bool
         Whether add activation at the last layer
+    num_ffn_layers_in_gnn: int
+        Number of ngnn gnn layers between GNN layers
     """
     def __init__(self,
                  g,
                  h_dim, out_dim, num_heads,
                  num_hidden_layers=1,
                  dropout=0,
                  use_self_loop=True,
-                 last_layer_act=False):
+                 last_layer_act=False,
+                 num_ffn_layers_in_gnn=0):
         super(RelationalGATEncoder, self).__init__(h_dim, out_dim, num_hidden_layers)
         self.num_heads = num_heads
         # h2h
         for _ in range(num_hidden_layers):
             self.layers.append(RelationalAttLayer(
                 h_dim, h_dim, g.canonical_etypes,
                 self.num_heads, activation=F.relu, self_loop=use_self_loop,
-                dropout=dropout))
+                dropout=dropout, num_ffn_layers_in_gnn=num_ffn_layers_in_gnn,
+                fnn_activation=F.relu))
         # h2o
         self.layers.append(RelationalAttLayer(
             h_dim, out_dim, g.canonical_etypes,
             self.num_heads, activation=F.relu if last_layer_act else None,
             self_loop=use_self_loop))
 
     def forward(self, blocks, h):
```

## graphstorm/model/rgcn_encoder.py

```diff
@@ -18,16 +18,18 @@
 import warnings
 
 import torch as th
 from torch import nn
 import torch.nn.functional as F
 import dgl.nn as dglnn
 
+from .ngnn_mlp import NGNNMLP
 from .gnn_encoder_base import GraphConvEncoder
 
+
 class RelGraphConvLayer(nn.Module):
     r"""Relational graph convolution layer.
 
     Parameters
     ----------
     in_feat : int
         Input feature size.
@@ -43,26 +45,32 @@
         True if bias is added. Default: True
     activation : callable, optional
         Activation function. Default: None
     self_loop : bool, optional
         True to include self loop message. Default: False
     dropout : float, optional
         Dropout rate. Default: 0.0
+    num_ffn_layers_in_gnn: int, optional
+        Number of layers of ngnn between gnn layers
+    ffn_actication: torch.nn.functional
+        Activation Method for ngnn
     """
     def __init__(self,
                  in_feat,
                  out_feat,
                  rel_names,
                  num_bases,
                  *,
                  weight=True,
                  bias=True,
                  activation=None,
                  self_loop=False,
-                 dropout=0.0):
+                 dropout=0.0,
+                 num_ffn_layers_in_gnn=0,
+                 ffn_activation=F.relu):
         super(RelGraphConvLayer, self).__init__()
         self.in_feat = in_feat
         self.out_feat = out_feat
         self.rel_names = rel_names
         self.num_bases = num_bases
         self.bias = bias
         self.activation = activation
@@ -90,14 +98,19 @@
 
         # weight for self loop
         if self.self_loop:
             self.loop_weight = nn.Parameter(th.Tensor(in_feat, out_feat))
             nn.init.xavier_uniform_(self.loop_weight,
                                     gain=nn.init.calculate_gain('relu'))
 
+        # ngnn
+        self.num_ffn_layers_in_gnn = num_ffn_layers_in_gnn
+        self.ngnn_mlp = NGNNMLP(out_feat, out_feat,
+                                     num_ffn_layers_in_gnn, ffn_activation, dropout)
+
         self.dropout = nn.Dropout(dropout)
 
     # pylint: disable=invalid-name
     def forward(self, g, inputs):
         """Forward computation
 
         Parameters
@@ -130,27 +143,30 @@
         def _apply(ntype, h):
             if self.self_loop:
                 h = h + th.matmul(inputs_dst[ntype], self.loop_weight)
             if self.bias:
                 h = h + self.h_bias
             if self.activation:
                 h = self.activation(h)
+            if self.num_ffn_layers_in_gnn > 0:
+                h = self.ngnn_mlp(h)
             return self.dropout(h)
 
         for k, _ in inputs.items():
             if g.number_of_dst_nodes(k) > 0:
                 if k not in hs:
                     warnings.warn("Warning. Graph convolution returned empty "
                         f"dictionary, for node with type: {str(k)}")
                     for _, in_v in inputs_src.items():
                         device = in_v.device
                     hs[k] = th.zeros((g.number_of_dst_nodes(k), self.out_feat), device=device)
                     # TODO the above might fail if the device is a different GPU
         return {ntype : _apply(ntype, h) for ntype, h in hs.items()}
 
+
 class RelationalGCNEncoder(GraphConvEncoder):
     r""" Relational graph conv encoder.
 
     Parameters
     ----------
     h_dim : int
         Hidden dimension
@@ -162,35 +178,39 @@
         Number of hidden layers. Total GNN layers is equal to num_hidden_layers + 1. Default 1
     dropout : float
         Dropout. Default 0.
     use_self_loop : bool
         Whether to add selfloop. Default True
     last_layer_act : torch.function
         Activation for the last layer. Default None
+    num_ffn_layers_in_gnn: int
+        Number of ngnn gnn layers between GNN layers
     """
     def __init__(self,
                  g,
                  h_dim, out_dim,
                  num_bases=-1,
                  num_hidden_layers=1,
                  dropout=0,
                  use_self_loop=True,
-                 last_layer_act=False):
+                 last_layer_act=False,
+                 num_ffn_layers_in_gnn=0):
         super(RelationalGCNEncoder, self).__init__(h_dim, out_dim, num_hidden_layers)
         if num_bases < 0 or num_bases > len(g.canonical_etypes):
             self.num_bases = len(g.canonical_etypes)
         else:
             self.num_bases = num_bases
 
         # h2h
         for _ in range(num_hidden_layers):
             self.layers.append(RelGraphConvLayer(
                 h_dim, h_dim, g.canonical_etypes,
                 self.num_bases, activation=F.relu, self_loop=use_self_loop,
-                dropout=dropout))
+                dropout=dropout, num_ffn_layers_in_gnn=num_ffn_layers_in_gnn,
+                ffn_activation=F.relu))
         # h2o
         self.layers.append(RelGraphConvLayer(
             h_dim, out_dim, g.canonical_etypes,
             self.num_bases, activation=F.relu if last_layer_act else None,
             self_loop=use_self_loop))
 
     # TODO(zhengda) refactor this to support edge features.
```

## graphstorm/model/utils.py

```diff
@@ -499,15 +499,15 @@
     else:
         checkpoint = th.load(os.path.join(model_path, 'model.bin'),
                              map_location='cpu',
                              weights_only=True)
     if 'gnn' in checkpoint and gnn_model is not None:
         gnn_model.load_state_dict(checkpoint['gnn'])
     if 'embed' in checkpoint and embed_layer is not None:
-        embed_layer.load_state_dict(checkpoint['embed'])
+        embed_layer.load_state_dict(checkpoint['embed'], strict=False)
     if 'decoder' in checkpoint and decoder is not None:
         decoder.load_state_dict(checkpoint['decoder'])
 
 def load_sparse_embeds(model_path, embed_layer, local_rank, world_size):
     """load sparse embeddings if any
 
         Sparse embeddings are stored as:
@@ -601,15 +601,15 @@
     # Load general dense models like gnn and input projection matrix
     if "dense" in checkpoint:
         assert len(dense_opts) == 1, "General dense parameters must exists in the model"
         dense_opts[0].load_state_dict(checkpoint["dense"])
     # Load language models.
     if "lm" in checkpoint:
         assert len(lm_opts) == 1, "Language model parameters must exists in the model"
-        dense_opts[0].load_state_dict(checkpoint["lm"])
+        lm_opts[0].load_state_dict(checkpoint["lm"])
 
     # TODO(zhengda) we need to change DGL to make it work.
     if 'sparse' in checkpoint and len(sparse_opts) > 0:
         raise NotImplementedError('We cannot load the state of sparse optimizer')
 
 
 def remove_saved_models(model_path):
```

## graphstorm/run/launch.py

```diff
@@ -371,15 +371,15 @@
         else "python3 "
 
     # transforms the udf_command from:
     #     path/to/dist_trainer.py arg0 arg1
     # to:
     #     python -m torch.distributed.launch [DIST TORCH ARGS] path/to/dist_trainer.py arg0 arg1
     udf_command = " ".join(udf_command)
-    new_udf_command = f"{python_bin} {torch_dist_cmd} {udf_command}"
+    new_udf_command = f"{python_bin} -u {torch_dist_cmd} {udf_command}"
 
     return new_udf_command
 
 
 def construct_dgl_server_env_vars(
     num_samplers: int,
     num_server_threads: int,
@@ -673,17 +673,17 @@
     ), "The number of graph partitions has to match the number of machines in the cluster."
 
     state_q = queue.Queue()
     tot_num_clients = args.num_trainers * (1 + args.num_samplers) * len(hosts)
 
     udf_command = update_udf_command(udf_command, args)
     # launch server tasks
-    server_cmd = f"{sys.executable} {' '.join(udf_command)}" \
+    server_cmd = f"{sys.executable} -u {' '.join(udf_command)}" \
         if sys.executable is not None and sys.executable != "" \
-        else f"python3 {' '.join(udf_command)}"
+        else f"python3 -u {' '.join(udf_command)}"
 
     server_env_vars = construct_dgl_server_env_vars(
         num_samplers=args.num_samplers,
         num_server_threads=args.num_server_threads,
         tot_num_clients=tot_num_clients,
         part_config=args.part_config,
         ip_config=args.ip_config,
@@ -854,18 +854,17 @@
         help="The file of IP configuration for server processes. \
               Absolute path is preferred. \
               Otherwise, the file should be in workspace.",
     )
     parser.add_argument(
         "--num-server-threads",
         type=int,
-        default=1,
         help="The number of OMP threads in the server process. \
                         It should be small if server processes and trainer processes run on \
-                        the same machine. By default, it is 1.",
+                        the same machine.",
     )
     parser.add_argument(
         "--graph-format",
         type=str,
         default="csc",
         help='The format of the graph structure of each partition. \
               The allowed formats are csr, csc and coo. A user can specify multiple \
@@ -910,41 +909,57 @@
     assert (
         args.num_samplers is not None and args.num_samplers >= 0
     ), "--num-samplers must be a non-negative number."
     assert (
         args.num_servers is not None and args.num_servers > 0
     ), "--num-servers must be a positive number."
     assert (
-        args.num_server_threads > 0
-    ), "--num-server-threads must be a positive number."
-    assert (
         args.part_config is not None
     ), "A user has to specify a partition configuration file with --part-onfig."
     assert (
         args.ip_config is not None
     ), "A user has to specify an IP configuration file with --ip-config."
 
     if args.workspace is None:
         # Get PWD
         args.workspace = os.getcwd()
     else:
         args.workspace = os.path.abspath(args.workspace)
 
+    total_cpu_cores = multiprocessing.cpu_count()
+
     if args.num_omp_threads is None:
         # Here we assume all machines have the same number of CPU cores as the machine
         # where the launch script runs.
+        # The total number of CPU cores consumed
+        # by trainers will be half of total cpu cores
+        cpu_cores_per_trainer = total_cpu_cores // 2 // args.num_trainers // \
+            (args.num_samplers if args.num_samplers > 1 else 1)
         args.num_omp_threads = max(
-            multiprocessing.cpu_count() // 2 // args.num_trainers, 1
+            cpu_cores_per_trainer, 1
         )
         if args.verbose:
             print(f"The number of OMP threads per trainer is set to {args.num_omp_threads}")
     else:
         assert args.num_omp_threads > 0, \
             "The number of OMP threads per trainer should be larger than 0"
 
+    if args.num_server_threads is None:
+        # The total number of CPU cores consumed
+        # by servers will be 1/4 of total cpu cores
+        cpu_cores_per_server = total_cpu_cores // 4 // args.num_servers
+        args.num_server_threads = max(
+            cpu_cores_per_server, 1
+        )
+        if args.verbose:
+            print(f"The number of OMP threads per server is set to {args.num_server_threads}")
+    else:
+        assert args.num_server_threads > 0, \
+            "The number of OMP threads per server should be larger than 1"
+
 def main():
     """Main func"""
     parser = get_argument_parser()
     # Positional arguments.
     parser.add_argument(
         "exec_script",
         type=str,
```

## graphstorm/run/gsgnn_ep/ep_infer_gnn.py

```diff
@@ -18,14 +18,15 @@
 
 import graphstorm as gs
 from graphstorm.config import get_argument_parser
 from graphstorm.config import GSConfig
 from graphstorm.inference import GSgnnEdgePredictionInfer
 from graphstorm.eval import GSgnnAccEvaluator, GSgnnRegressionEvaluator
 from graphstorm.dataloading import GSgnnEdgeInferData, GSgnnEdgeDataLoader
+from graphstorm.utils import setup_device
 
 def get_evaluator(config): # pylint: disable=unused-argument
     """ Get evaluator class
     """
     if config.task_type == "edge_regression":
         return GSgnnRegressionEvaluator(config.eval_frequency,
                                         config.eval_metric)
@@ -36,36 +37,46 @@
     else:
         raise AttributeError(config.task_type + ' is not supported.')
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(False)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
+    device = setup_device(config.local_rank)
 
     infer_data = GSgnnEdgeInferData(config.graph_name,
                                     config.part_config,
                                     eval_etypes=config.target_etype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_edge_gnn_model(infer_data.g, config, train_task=False)
     model.restore_model(config.restore_model_path)
     # TODO(zhengda) we should use a different way to get rank.
     infer = GSgnnEdgePredictionInfer(model, gs.get_rank())
-    infer.setup_cuda(dev_id=config.local_rank)
+    infer.setup_device(device=device)
     if not config.no_validation:
         evaluator = get_evaluator(config)
         infer.setup_evaluator(evaluator)
-        assert len(infer_data.test_idxs) > 0, "There is not test data for evaluation."
+        assert len(infer_data.test_idxs) > 0, \
+            "There is not test data for evaluation. " \
+            "You can use --no-validation true to avoid do testing"
+        target_idxs = infer_data.test_idxs
+    else:
+        assert len(infer_data.infer_idxs) > 0, \
+            f"To do inference on {config.target_etype} without doing evaluation, " \
+            "you should not define test_mask as its edge feature. " \
+            "GraphStorm will do inference on the whole edge set. "
+        target_idxs = infer_data.infer_idxs
     tracker = gs.create_builtin_task_tracker(config, infer.rank)
     infer.setup_task_tracker(tracker)
-    device = 'cuda:%d' % infer.dev_id
     fanout = config.eval_fanout if config.use_mini_batch_infer else []
-    dataloader = GSgnnEdgeDataLoader(infer_data, infer_data.test_idxs, fanout=fanout,
+    dataloader = GSgnnEdgeDataLoader(infer_data, target_idxs, fanout=fanout,
                                      batch_size=config.eval_batch_size,
                                      device=device, train_task=False,
                                      reverse_edge_types_map=config.reverse_edge_types_map,
                                      remove_target_edge_type=config.remove_target_edge_type,
                                      decoder_edge_feat=config.decoder_edge_feat)
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
```

## graphstorm/run/gsgnn_ep/ep_infer_lm.py

```diff
@@ -19,14 +19,15 @@
 
 import graphstorm as gs
 from graphstorm.config import get_argument_parser
 from graphstorm.config import GSConfig
 from graphstorm.inference import GSgnnEdgePredictionInfer
 from graphstorm.eval import GSgnnAccEvaluator, GSgnnRegressionEvaluator
 from graphstorm.dataloading import GSgnnEdgeInferData, GSgnnEdgeDataLoader
+from graphstorm.utils import setup_device
 
 def get_evaluator(config): # pylint: disable=unused-argument
     """ Get evaluator class
     """
     if config.task_type == "edge_regression":
         return GSgnnRegressionEvaluator(config.eval_frequency,
                                         config.eval_metric)
@@ -39,32 +40,32 @@
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
+    device = setup_device(config.local_rank)
 
     infer_data = GSgnnEdgeInferData(config.graph_name,
                                     config.part_config,
                                     eval_etypes=config.target_etype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_edge_model(infer_data.g, config, train_task=False)
     model.restore_model(config.restore_model_path)
     # TODO(zhengda) we should use a different way to get rank.
     infer = GSgnnEdgePredictionInfer(model, gs.get_rank())
-    infer.setup_cuda(dev_id=config.local_rank)
+    infer.setup_device(device=device)
     if not config.no_validation:
         evaluator = get_evaluator(config)
         infer.setup_evaluator(evaluator)
         assert len(infer_data.test_idxs) > 0, "There is not test data for evaluation."
     tracker = gs.create_builtin_task_tracker(config, infer.rank)
     infer.setup_task_tracker(tracker)
-    device = 'cuda:%d' % infer.dev_id
     dataloader = GSgnnEdgeDataLoader(infer_data, infer_data.test_idxs, fanout=[],
                                      batch_size=config.eval_batch_size,
                                      device=device, train_task=False,
                                      remove_target_edge_type=False,
                                      decoder_edge_feat=config.decoder_edge_feat)
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
```

## graphstorm/run/gsgnn_ep/gsgnn_ep.py

```diff
@@ -23,15 +23,15 @@
 from graphstorm.config import GSConfig
 from graphstorm.trainer import GSgnnEdgePredictionTrainer
 from graphstorm.dataloading import GSgnnEdgeTrainData, GSgnnEdgeDataLoader
 from graphstorm.eval import GSgnnAccEvaluator
 from graphstorm.eval import GSgnnRegressionEvaluator
 from graphstorm.model.utils import save_embeddings
 from graphstorm.model import do_full_graph_inference
-from graphstorm.utils import rt_profiler, sys_tracker
+from graphstorm.utils import rt_profiler, sys_tracker, setup_device
 
 def get_evaluator(config):
     """ Get evaluator class
     """
     if config.task_type == "edge_classification":
         return GSgnnAccEvaluator(config.eval_frequency,
                                  config.eval_metric,
@@ -50,44 +50,44 @@
     else:
         raise ValueError("Unknown task type")
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(True)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
     rt_profiler.init(config.profile_path, rank=gs.get_rank())
     sys_tracker.init(config.verbose, rank=gs.get_rank())
+    device = setup_device(config.local_rank)
     # edge predict only handle edge feature in decoder
     train_data = GSgnnEdgeTrainData(config.graph_name,
                                     config.part_config,
                                     train_etypes=config.target_etype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_edge_gnn_model(train_data.g, config, train_task=True)
     trainer = GSgnnEdgePredictionTrainer(model, gs.get_rank(),
                                          topk_model_to_save=config.topk_model_to_save)
     if config.restore_model_path is not None:
         trainer.restore_model(model_path=config.restore_model_path,
                               model_layer_to_load=config.restore_model_layers)
-    trainer.setup_cuda(dev_id=config.local_rank)
+    trainer.setup_device(device=device)
     if not config.no_validation:
         # TODO(zhengda) we need to refactor the evaluator.
         evaluator = get_evaluator(config)
         trainer.setup_evaluator(evaluator)
         assert len(train_data.val_idxs) > 0, "The training data do not have validation set."
         # TODO(zhengda) we need to compute the size of the entire validation set to make sure
         # we have validation data.
     tracker = gs.create_builtin_task_tracker(config, trainer.rank)
     if trainer.rank == 0:
         tracker.log_params(config.__dict__)
     trainer.setup_task_tracker(tracker)
-
-    device = 'cuda:%d' % trainer.dev_id
     dataloader = GSgnnEdgeDataLoader(train_data, train_data.train_idxs, fanout=config.fanout,
                                      batch_size=config.batch_size, device=device, train_task=True,
                                      reverse_edge_types_map=config.reverse_edge_types_map,
                                      remove_target_edge_type=config.remove_target_edge_type,
                                      exclude_training_targets=config.exclude_training_targets,
                                      decoder_edge_feat=config.decoder_edge_feat)
     val_dataloader = None
```

## graphstorm/run/gsgnn_ep/gsgnn_lm_ep.py

```diff
@@ -23,15 +23,15 @@
 from graphstorm.config import GSConfig
 from graphstorm.trainer import GSgnnEdgePredictionTrainer
 from graphstorm.dataloading import GSgnnEdgeTrainData, GSgnnEdgeDataLoader
 from graphstorm.eval import GSgnnAccEvaluator
 from graphstorm.eval import GSgnnRegressionEvaluator
 from graphstorm.model.utils import save_embeddings
 from graphstorm.model import do_full_graph_inference
-from graphstorm.utils import rt_profiler, sys_tracker
+from graphstorm.utils import rt_profiler, sys_tracker, setup_device
 
 def get_evaluator(config):
     """ Get evaluator class
     """
     if config.task_type == "edge_classification":
         return GSgnnAccEvaluator(config.eval_frequency,
                                  config.eval_metric,
@@ -54,39 +54,38 @@
     """ main function
     """
     config = GSConfig(config_args)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
     rt_profiler.init(config.profile_path, rank=gs.get_rank())
     sys_tracker.init(config.verbose, rank=gs.get_rank())
+    device = setup_device(config.local_rank)
     train_data = GSgnnEdgeTrainData(config.graph_name,
                                     config.part_config,
                                     train_etypes=config.target_etype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_edge_model(train_data.g, config, train_task=True)
     trainer = GSgnnEdgePredictionTrainer(model, gs.get_rank(),
                                          topk_model_to_save=config.topk_model_to_save)
     if config.restore_model_path is not None:
         trainer.restore_model(model_path=config.restore_model_path,
                               model_layer_to_load=config.restore_model_layers)
-    trainer.setup_cuda(dev_id=config.local_rank)
+    trainer.setup_device(device=device)
     if not config.no_validation:
         # TODO(zhengda) we need to refactor the evaluator.
         evaluator = get_evaluator(config)
         trainer.setup_evaluator(evaluator)
         assert len(train_data.val_idxs) > 0, "The training data do not have validation set."
         # TODO(zhengda) we need to compute the size of the entire validation set to make sure
         # we have validation data.
     tracker = gs.create_builtin_task_tracker(config, trainer.rank)
     if trainer.rank == 0:
         tracker.log_params(config.__dict__)
     trainer.setup_task_tracker(tracker)
-
-    device = 'cuda:%d' % trainer.dev_id
     dataloader = GSgnnEdgeDataLoader(train_data, train_data.train_idxs, fanout=[],
                                      batch_size=config.batch_size, device=device, train_task=True,
                                      remove_target_edge_type=False,
                                      decoder_edge_feat=config.decoder_edge_feat)
     val_dataloader = None
     test_dataloader = None
     # we don't need fanout for full-graph inference
```

## graphstorm/run/gsgnn_lp/gsgnn_lm_lp.py

```diff
@@ -36,36 +36,38 @@
 from graphstorm.dataloading import BUILTIN_LP_LOCALUNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_LOCALJOINT_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER
 from graphstorm.eval import GSgnnMrrLPEvaluator
 from graphstorm.model.utils import save_embeddings
 from graphstorm.model import do_full_graph_inference
-from graphstorm.utils import rt_profiler, sys_tracker
+from graphstorm.utils import rt_profiler, sys_tracker, setup_device
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(True)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
     rt_profiler.init(config.profile_path, rank=gs.get_rank())
     sys_tracker.init(config.verbose, rank=gs.get_rank())
+    device = setup_device(config.local_rank)
     train_data = GSgnnEdgeTrainData(config.graph_name,
                                     config.part_config,
                                     train_etypes=config.train_etype,
                                     eval_etypes=config.eval_etype,
                                     node_feat_field=config.node_feat_name)
     model = gs.create_builtin_lp_model(train_data.g, config, train_task=True)
     trainer = GSgnnLinkPredictionTrainer(model, gs.get_rank(),
                                          topk_model_to_save=config.topk_model_to_save)
     if config.restore_model_path is not None:
         trainer.restore_model(model_path=config.restore_model_path,
                               model_layer_to_load=config.restore_model_layers)
-    trainer.setup_cuda(dev_id=config.local_rank)
+    trainer.setup_device(device=device)
     if not config.no_validation:
         # TODO(zhengda) we need to refactor the evaluator.
         trainer.setup_evaluator(
             GSgnnMrrLPEvaluator(config.eval_frequency,
                                 train_data,
                                 config.num_negative_edges_eval,
                                 config.lp_decoder_type,
@@ -91,33 +93,36 @@
         dataloader_cls = GSgnnLPLocalJointNegDataLoader
     elif config.train_negative_sampler == BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER:
         dataloader_cls = GSgnnAllEtypeLinkPredictionDataLoader
     elif config.train_negative_sampler == BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER:
         dataloader_cls = GSgnnAllEtypeLPJointNegDataLoader
     else:
         raise ValueError('Unknown negative sampler')
-    device = 'cuda:%d' % trainer.dev_id
     dataloader = dataloader_cls(train_data, train_data.train_idxs, [],
                                 config.batch_size, config.num_negative_edges, device,
                                 train_task=True,
                                 lp_edge_weight_for_loss=config.lp_edge_weight_for_loss)
 
     # TODO(zhengda) let's use full-graph inference for now.
     if config.eval_negative_sampler == BUILTIN_LP_UNIFORM_NEG_SAMPLER:
         test_dataloader_cls = GSgnnLinkPredictionTestDataLoader
     elif config.eval_negative_sampler == BUILTIN_LP_JOINT_NEG_SAMPLER:
         test_dataloader_cls = GSgnnLinkPredictionJointTestDataLoader
     else:
         raise ValueError('Unknown test negative sampler.'
             'Supported test negative samplers include '
             f'[{BUILTIN_LP_UNIFORM_NEG_SAMPLER}, {BUILTIN_LP_JOINT_NEG_SAMPLER}]')
-    val_dataloader = test_dataloader_cls(train_data, train_data.val_idxs,
-        config.eval_batch_size, config.num_negative_edges_eval)
-    test_dataloader = test_dataloader_cls(train_data, train_data.test_idxs,
-        config.eval_batch_size, config.num_negative_edges_eval)
+    val_dataloader = None
+    test_dataloader = None
+    if len(train_data.val_idxs) > 0:
+        val_dataloader = test_dataloader_cls(train_data, train_data.val_idxs,
+            config.eval_batch_size, config.num_negative_edges_eval)
+    if len(train_data.test_idxs) > 0:
+        test_dataloader = test_dataloader_cls(train_data, train_data.test_idxs,
+            config.eval_batch_size, config.num_negative_edges_eval)
 
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
     # For example pre-compute all BERT embeddings
     model.prepare_input_encoder(train_data)
     if config.save_model_path is not None:
         save_model_path = config.save_model_path
```

## graphstorm/run/gsgnn_lp/gsgnn_lp.py

```diff
@@ -33,40 +33,50 @@
 from graphstorm.dataloading import GSgnnLinkPredictionJointTestDataLoader
 from graphstorm.dataloading import BUILTIN_LP_UNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_JOINT_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_LOCALUNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_LOCALJOINT_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER
+from graphstorm.dataloading import (BUILTIN_FAST_LP_UNIFORM_NEG_SAMPLER,
+                                    BUILTIN_FAST_LP_JOINT_NEG_SAMPLER,
+                                    BUILTIN_FAST_LP_LOCALUNIFORM_NEG_SAMPLER,
+                                    BUILTIN_FAST_LP_LOCALJOINT_NEG_SAMPLER)
+from graphstorm.dataloading import (FastGSgnnLinkPredictionDataLoader,
+                                    FastGSgnnLPJointNegDataLoader,
+                                    FastGSgnnLPLocalUniformNegDataLoader,
+                                    FastGSgnnLPLocalJointNegDataLoader)
 from graphstorm.eval import GSgnnMrrLPEvaluator
 from graphstorm.model.utils import save_embeddings
 from graphstorm.model import do_full_graph_inference
-from graphstorm.utils import rt_profiler, sys_tracker
+from graphstorm.utils import rt_profiler, sys_tracker, setup_device
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(True)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
     rt_profiler.init(config.profile_path, rank=gs.get_rank())
     sys_tracker.init(config.verbose, rank=gs.get_rank())
+    device = setup_device(config.local_rank)
     node_feat_field = config.node_feat_name
     train_data = GSgnnEdgeTrainData(config.graph_name,
                                     config.part_config,
                                     train_etypes=config.train_etype,
                                     eval_etypes=config.eval_etype,
                                     node_feat_field=node_feat_field)
     model = gs.create_builtin_lp_gnn_model(train_data.g, config, train_task=True)
     trainer = GSgnnLinkPredictionTrainer(model, gs.get_rank(),
                                          topk_model_to_save=config.topk_model_to_save)
     if config.restore_model_path is not None:
         trainer.restore_model(model_path=config.restore_model_path,
                               model_layer_to_load=config.restore_model_layers)
-    trainer.setup_cuda(dev_id=config.local_rank)
+    trainer.setup_device(device=device)
     if not config.no_validation:
         # TODO(zhengda) we need to refactor the evaluator.
         trainer.setup_evaluator(
             GSgnnMrrLPEvaluator(config.eval_frequency,
                                 train_data,
                                 config.num_negative_edges_eval,
                                 config.lp_decoder_type,
@@ -90,17 +100,24 @@
         dataloader_cls = GSgnnLPLocalUniformNegDataLoader
     elif config.train_negative_sampler == BUILTIN_LP_LOCALJOINT_NEG_SAMPLER:
         dataloader_cls = GSgnnLPLocalJointNegDataLoader
     elif config.train_negative_sampler == BUILTIN_LP_ALL_ETYPE_UNIFORM_NEG_SAMPLER:
         dataloader_cls = GSgnnAllEtypeLinkPredictionDataLoader
     elif config.train_negative_sampler == BUILTIN_LP_ALL_ETYPE_JOINT_NEG_SAMPLER:
         dataloader_cls = GSgnnAllEtypeLPJointNegDataLoader
+    elif config.train_negative_sampler == BUILTIN_FAST_LP_UNIFORM_NEG_SAMPLER:
+        dataloader_cls = FastGSgnnLinkPredictionDataLoader
+    elif config.train_negative_sampler == BUILTIN_FAST_LP_JOINT_NEG_SAMPLER:
+        dataloader_cls = FastGSgnnLPJointNegDataLoader
+    elif config.train_negative_sampler == BUILTIN_FAST_LP_LOCALUNIFORM_NEG_SAMPLER:
+        dataloader_cls = FastGSgnnLPLocalUniformNegDataLoader
+    elif config.train_negative_sampler == BUILTIN_FAST_LP_LOCALJOINT_NEG_SAMPLER:
+        dataloader_cls = FastGSgnnLPLocalJointNegDataLoader
     else:
         raise ValueError('Unknown negative sampler')
-    device = 'cuda:%d' % trainer.dev_id
     dataloader = dataloader_cls(train_data, train_data.train_idxs, config.fanout,
                                 config.batch_size, config.num_negative_edges, device,
                                 train_task=True,
                                 reverse_edge_types_map=config.reverse_edge_types_map,
                                 exclude_training_targets=config.exclude_training_targets,
                                 lp_edge_weight_for_loss=config.lp_edge_weight_for_loss)
 
@@ -109,18 +126,22 @@
         test_dataloader_cls = GSgnnLinkPredictionTestDataLoader
     elif config.eval_negative_sampler == BUILTIN_LP_JOINT_NEG_SAMPLER:
         test_dataloader_cls = GSgnnLinkPredictionJointTestDataLoader
     else:
         raise ValueError('Unknown test negative sampler.'
             'Supported test negative samplers include '
             f'[{BUILTIN_LP_UNIFORM_NEG_SAMPLER}, {BUILTIN_LP_JOINT_NEG_SAMPLER}]')
-    val_dataloader = test_dataloader_cls(train_data, train_data.val_idxs,
-        config.eval_batch_size, config.num_negative_edges_eval, config.eval_fanout)
-    test_dataloader = test_dataloader_cls(train_data, train_data.test_idxs,
-        config.eval_batch_size, config.num_negative_edges_eval, config.eval_fanout)
+    val_dataloader = None
+    test_dataloader = None
+    if len(train_data.val_idxs) > 0:
+        val_dataloader = test_dataloader_cls(train_data, train_data.val_idxs,
+            config.eval_batch_size, config.num_negative_edges_eval, config.eval_fanout)
+    if len(train_data.test_idxs) > 0:
+        test_dataloader = test_dataloader_cls(train_data, train_data.test_idxs,
+            config.eval_batch_size, config.num_negative_edges_eval, config.eval_fanout)
 
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
     # For example pre-compute all BERT embeddings
     model.prepare_input_encoder(train_data)
     if config.save_model_path is not None:
         save_model_path = config.save_model_path
```

## graphstorm/run/gsgnn_lp/lp_infer_gnn.py

```diff
@@ -22,30 +22,33 @@
 from graphstorm.inference import GSgnnLinkPredictionInfer
 from graphstorm.eval import GSgnnMrrLPEvaluator
 from graphstorm.dataloading import GSgnnEdgeInferData
 from graphstorm.dataloading import GSgnnLinkPredictionTestDataLoader
 from graphstorm.dataloading import GSgnnLinkPredictionJointTestDataLoader
 from graphstorm.dataloading import BUILTIN_LP_UNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_JOINT_NEG_SAMPLER
+from graphstorm.utils import setup_device
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(False)
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
+    device = setup_device(config.local_rank)
 
     infer_data = GSgnnEdgeInferData(config.graph_name,
                                     config.part_config,
                                     eval_etypes=config.eval_etype,
                                     node_feat_field=config.node_feat_name)
     model = gs.create_builtin_lp_gnn_model(infer_data.g, config, train_task=False)
     model.restore_model(config.restore_model_path)
     # TODO(zhengda) we should use a different way to get rank.
     infer = GSgnnLinkPredictionInfer(model, gs.get_rank())
-    infer.setup_cuda(dev_id=config.local_rank)
+    infer.setup_device(device=device)
     if not config.no_validation:
         infer.setup_evaluator(
             GSgnnMrrLPEvaluator(config.eval_frequency,
                                 infer_data,
                                 config.num_negative_edges_eval,
                                 config.lp_decoder_type))
         assert len(infer_data.test_idxs) > 0, "There is not test data for evaluation."
@@ -65,15 +68,18 @@
                                      batch_size=config.eval_batch_size,
                                      num_negative_edges=config.num_negative_edges_eval,
                                      fanout=config.eval_fanout)
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
     # For example pre-compute all BERT embeddings
     model.prepare_input_encoder(infer_data)
-    infer.infer(infer_data, dataloader, save_embed_path=config.save_embed_path,
+    infer.infer(infer_data, dataloader,
+                save_embed_path=config.save_embed_path,
+                edge_mask_for_gnn_embeddings=None if config.no_validation else \
+                    'train_mask', # if no validation,any edge can be used in message passing.
                 node_id_mapping_file=config.node_id_mapping_file)
 
 def generate_parser():
     """ Generate an argument parser
     """
     parser = get_argument_parser()
     return parser
```

## graphstorm/run/gsgnn_lp/lp_infer_lm.py

```diff
@@ -23,30 +23,33 @@
 from graphstorm.inference import GSgnnLinkPredictionInfer
 from graphstorm.eval import GSgnnMrrLPEvaluator
 from graphstorm.dataloading import GSgnnEdgeInferData
 from graphstorm.dataloading import GSgnnLinkPredictionTestDataLoader
 from graphstorm.dataloading import GSgnnLinkPredictionJointTestDataLoader
 from graphstorm.dataloading import BUILTIN_LP_UNIFORM_NEG_SAMPLER
 from graphstorm.dataloading import BUILTIN_LP_JOINT_NEG_SAMPLER
+from graphstorm.utils import setup_device
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(False)
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
+    device = setup_device(config.local_rank)
 
     infer_data = GSgnnEdgeInferData(config.graph_name,
                                     config.part_config,
                                     eval_etypes=config.eval_etype,
                                     node_feat_field=config.node_feat_name)
     model = gs.create_builtin_lp_model(infer_data.g, config, train_task=False)
     model.restore_model(config.restore_model_path)
     # TODO(zhengda) we should use a different way to get rank.
     infer = GSgnnLinkPredictionInfer(model, gs.get_rank())
-    infer.setup_cuda(dev_id=config.local_rank)
+    infer.setup_device(device=device)
     if not config.no_validation:
         infer.setup_evaluator(
             GSgnnMrrLPEvaluator(config.eval_frequency,
                                 infer_data,
                                 config.num_negative_edges_eval,
                                 config.lp_decoder_type))
         assert len(infer_data.test_idxs) > 0, "There is not test data for evaluation."
@@ -67,14 +70,15 @@
                                      num_negative_edges=config.num_negative_edges_eval)
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
     # For example pre-compute all BERT embeddings
     model.prepare_input_encoder(infer_data)
     infer.infer(infer_data, dataloader,
                 save_embed_path=config.save_embed_path,
+                edge_mask_for_gnn_embeddings=None, # LM infer does not use GNN
                 node_id_mapping_file=config.node_id_mapping_file)
 
 def generate_parser():
     """ Generate an argument parser
     """
     parser = get_argument_parser()
     return parser
```

## graphstorm/run/gsgnn_np/gsgnn_np.py

```diff
@@ -18,20 +18,21 @@
 
 import os
 import torch as th
 import graphstorm as gs
 from graphstorm.config import get_argument_parser
 from graphstorm.config import GSConfig
 from graphstorm.trainer import GSgnnNodePredictionTrainer
+from graphstorm.trainer import GLEMNodePredictionTrainer
 from graphstorm.dataloading import GSgnnNodeTrainData, GSgnnNodeDataLoader
 from graphstorm.eval import GSgnnAccEvaluator
 from graphstorm.eval import GSgnnRegressionEvaluator
 from graphstorm.model.utils import save_embeddings
 from graphstorm.model import do_full_graph_inference
-from graphstorm.utils import rt_profiler, sys_tracker
+from graphstorm.utils import rt_profiler, sys_tracker, setup_device
 
 def get_evaluator(config):
     """ Get evaluator class
     """
     if config.task_type == "node_classification":
         return GSgnnAccEvaluator(config.eval_frequency,
                                  config.eval_metric,
@@ -50,41 +51,46 @@
     else:
         raise ValueError("Unknown task type")
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(True)
 
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
     rt_profiler.init(config.profile_path, rank=gs.get_rank())
     sys_tracker.init(config.verbose, rank=gs.get_rank())
+    device = setup_device(config.local_rank)
     train_data = GSgnnNodeTrainData(config.graph_name,
                                     config.part_config,
                                     train_ntypes=config.target_ntype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_node_gnn_model(train_data.g, config, train_task=True)
-    trainer = GSgnnNodePredictionTrainer(model, gs.get_rank(),
-                                         topk_model_to_save=config.topk_model_to_save)
+    if config.training_method["name"] == "glem":
+        trainer_class = GLEMNodePredictionTrainer
+    elif config.training_method["name"] == "default":
+        trainer_class = GSgnnNodePredictionTrainer
+    trainer = trainer_class(model, gs.get_rank(),
+                                        topk_model_to_save=config.topk_model_to_save)
     if config.restore_model_path is not None:
         trainer.restore_model(model_path=config.restore_model_path,
                               model_layer_to_load=config.restore_model_layers)
-    trainer.setup_cuda(dev_id=config.local_rank)
+    trainer.setup_device(device=device)
     if not config.no_validation:
         evaluator = get_evaluator(config)
         trainer.setup_evaluator(evaluator)
         assert len(train_data.val_idxs) > 0, "The training data do not have validation set."
         # TODO(zhengda) we need to compute the size of the entire validation set to make sure
         # we have validation data.
     tracker = gs.create_builtin_task_tracker(config, trainer.rank)
     if trainer.rank == 0:
         tracker.log_params(config.__dict__)
     trainer.setup_task_tracker(tracker)
-    device = 'cuda:%d' % trainer.dev_id
     dataloader = GSgnnNodeDataLoader(train_data, train_data.train_idxs, fanout=config.fanout,
                                      batch_size=config.batch_size, device=device, train_task=True)
     val_dataloader = None
     test_dataloader = None
     # we don't need fanout for full-graph inference
     fanout = config.eval_fanout if config.use_mini_batch_infer else []
     if len(train_data.val_idxs) > 0:
```

## graphstorm/run/gsgnn_np/np_infer_gnn.py

```diff
@@ -18,14 +18,15 @@
 
 import graphstorm as gs
 from graphstorm.config import get_argument_parser
 from graphstorm.config import GSConfig
 from graphstorm.inference import GSgnnNodePredictionInfer
 from graphstorm.eval import GSgnnAccEvaluator, GSgnnRegressionEvaluator
 from graphstorm.dataloading import GSgnnNodeInferData, GSgnnNodeDataLoader
+from graphstorm.utils import setup_device
 
 def get_evaluator(config): # pylint: disable=unused-argument
     """ Get evaluator class
     """
     if config.task_type == "node_regression":
         return GSgnnRegressionEvaluator(config.eval_frequency,
                                         config.eval_metric)
@@ -36,35 +37,45 @@
     else:
         raise AttributeError(config.task_type + ' is not supported.')
 
 def main(config_args):
     """ main function
     """
     config = GSConfig(config_args)
+    config.verify_arguments(False)
     gs.initialize(ip_config=config.ip_config, backend=config.backend)
+    device = setup_device(config.local_rank)
 
     infer_data = GSgnnNodeInferData(config.graph_name,
                                     config.part_config,
                                     eval_ntypes=config.target_ntype,
                                     node_feat_field=config.node_feat_name,
                                     label_field=config.label_field)
     model = gs.create_builtin_node_gnn_model(infer_data.g, config, train_task=False)
     model.restore_model(config.restore_model_path)
     # TODO(zhengda) we should use a different way to get rank.
     infer = GSgnnNodePredictionInfer(model, gs.get_rank())
-    infer.setup_cuda(dev_id=config.local_rank)
+    infer.setup_device(device=device)
     if not config.no_validation:
         evaluator = get_evaluator(config)
         infer.setup_evaluator(evaluator)
-        assert len(infer_data.test_idxs) > 0, "There is not test data for evaluation."
+        assert len(infer_data.test_idxs) > 0, \
+            "There is not test data for evaluation. " \
+            "You can use --no-validation true to avoid do testing"
+        target_idxs = infer_data.test_idxs
+    else:
+        assert len(infer_data.infer_idxs) > 0, \
+            f"To do inference on {config.target_ntype} without doing evaluation, " \
+            "you should not define test_mask as its node feature. " \
+            "GraphStorm will do inference on the whole node set. "
+        target_idxs = infer_data.infer_idxs
     tracker = gs.create_builtin_task_tracker(config, infer.rank)
     infer.setup_task_tracker(tracker)
-    device = 'cuda:%d' % infer.dev_id
     fanout = config.eval_fanout if config.use_mini_batch_infer else []
-    dataloader = GSgnnNodeDataLoader(infer_data, infer_data.test_idxs, fanout=fanout,
+    dataloader = GSgnnNodeDataLoader(infer_data, target_idxs, fanout=fanout,
                                      batch_size=config.eval_batch_size, device=device,
                                      train_task=False)
     # Preparing input layer for training or inference.
     # The input layer can pre-compute node features in the preparing step if needed.
     # For example pre-compute all BERT embeddings
     model.prepare_input_encoder(infer_data)
     infer.infer(dataloader, save_embed_path=config.save_embed_path,
```

## graphstorm/sagemaker/sagemaker_infer.py

```diff
@@ -88,16 +88,16 @@
     elif task_type == BUILTIN_TASK_EDGE_REGRESSION:
         cmd = "graphstorm.run.gs_edge_regression"
     elif task_type == BUILTIN_TASK_LINK_PREDICTION:
         cmd = "graphstorm.run.gs_link_prediction"
     else:
         raise RuntimeError(f"Unsupported task type {task_type}")
 
-    launch_cmd = ["python3", "-m", cmd,
-        "--num-trainers", f"{num_gpus}",
+    launch_cmd = ["python3", "-u",  "-m", cmd,
+        "--num-trainers", f"{num_gpus if int(num_gpus) > 0 else 1}",
         "--num-servers", "1",
         "--num-samplers", "0",
         "--part-config", f"{graph_config}",
         "--ip-config", f"{ip_list}",
         "--extra-envs", f"LD_LIBRARY_PATH={os.environ['LD_LIBRARY_PATH']} ",
         "--ssh-port", "22", "--inference"]
     launch_cmd += [custom_script] if custom_script is not None else []
@@ -149,16 +149,18 @@
         sm_dist_env: json str
             SageMaker distributed env.
         region: str
             AWS Region.
     """
     num_gpus = args.num_gpus
     data_path = args.data_path
-    model_path = '/opt/ml/model'
-    output_path = '/opt/ml/checkpoints'
+    model_path = '/opt/ml/gsgnn_model'
+    output_path = '/tmp/infer_output'
+    os.makedirs(model_path, exist_ok=True)
+    os.makedirs(output_path, exist_ok=True)
 
     # start the ssh server
     subprocess.run(["service", "ssh", "start"], check=True)
 
     print(f"Know args {args}")
     print(f"Unknow args {unknownargs}")
```

## graphstorm/sagemaker/sagemaker_train.py

```diff
@@ -83,16 +83,16 @@
     elif task_type == BUILTIN_TASK_EDGE_REGRESSION:
         cmd = "graphstorm.run.gs_edge_regression"
     elif task_type == BUILTIN_TASK_LINK_PREDICTION:
         cmd = "graphstorm.run.gs_link_prediction"
     else:
         raise RuntimeError(f"Unsupported task type {task_type}")
 
-    launch_cmd = ["python3", "-m", cmd,
-        "--num-trainers", f"{num_gpus}",
+    launch_cmd = ["python3", "-u", "-m", cmd,
+        "--num-trainers", f"{num_gpus if int(num_gpus) > 0 else 1}",
         "--num-servers", "1",
         "--num-samplers", "0",
         "--part-config", f"{graph_config}",
         "--ip-config", f"{ip_list}",
         "--extra-envs", f"LD_LIBRARY_PATH={os.environ['LD_LIBRARY_PATH']} ",
         "--ssh-port", "22"]
     launch_cmd += [custom_script] if custom_script is not None else []
@@ -141,15 +141,16 @@
         sm_dist_env: json str
             SageMaker distributed env.
         region: str
             AWS Region.
     """
     num_gpus = args.num_gpus
     data_path = args.data_path
-    output_path = "/opt/ml/model/"
+    output_path = "/tmp/gsgnn_model/"
+    os.makedirs(output_path, exist_ok=True)
 
     # start the ssh server
     subprocess.run(["service", "ssh", "start"], check=True)
 
     print(f"Know args {args}")
     print(f"Unknow args {unknownargs}")
```

## graphstorm/sagemaker/utils.py

```diff
@@ -11,23 +11,48 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     sagemaker script utilities
 """
-
+import subprocess
+import logging
 import os
 import time
 import shutil
-
 from urllib.parse import urlparse
 
-from sagemaker.s3 import S3Downloader # pylint: disable=no-name-in-module
-from sagemaker.s3 import S3Uploader   # pylint: disable=no-name-in-module
+import boto3
+from botocore.errorfactory import ClientError
+from sagemaker.s3 import S3Downloader
+from sagemaker.s3 import S3Uploader
+
+
+def run(launch_cmd, state_q, env=None):
+    """ Running cmd using shell
+
+    Parameters
+    ----------
+    launch_cmd: str
+        cmd to launch
+    state_q: queue.Queue()
+        A queue used to return execution result (success or failure)
+    env: dict
+        System environment. If None, subprocess will use the inherited one.
+    """
+    try:
+        subprocess.check_call(launch_cmd, shell=False, env=env)
+        state_q.put(0)
+    except subprocess.CalledProcessError as err:
+        logging.error("Called process error %s", err)
+        state_q.put(err.returncode)
+    except Exception as err: # pylint: disable=broad-except
+        logging.error("Called process error %s", err)
+        state_q.put(-1)
 
 def barrier_master(client_list, world_size):
     """ Master barrier, called by host_rank == 0
 
     Parameters
     ----------
     client_list: list
@@ -84,15 +109,15 @@
         Indicate whether the task has finished.
     """
     while task_end.is_set() is False:
         time.sleep(60)
         for rank in range(1, world_size):
             client_list[rank].send(b"Dummy")
 
-    print("Exit")
+    logging.info("keepalive thread exiting...")
 
 def terminate_workers(client_list, world_size, task_end):
     """ termiate all worker deamons.
 
     Parameters
     ----------
     client_list: list
@@ -102,15 +127,16 @@
     task_end: threading.Event
         Indicate whether the task has finished.
     """
     task_end.set()
     for rank in range(1, world_size):
         client_list[rank].send(b"Done")
         msg = client_list[rank].recv(8)
-        print(f"Client {rank} exit {msg.decode()}")
+        logging.info("Client %d exit %s",
+            rank, msg.decode())
 
     # close connections with clients
     for rank in range(1, world_size):
         client_list[rank].close()
 
 def wait_for_exit(master_sock):
     """ Worker processes wait for exit
@@ -119,15 +145,15 @@
     ----------
     master_sock: socket
         Socket connecting master
     """
     msg = master_sock.recv(8)
     while msg.decode() != "Done":
         msg = master_sock.recv(8)
-        print(msg.decode())
+        logging.debug(msg.decode())
     master_sock.send(b"Exit")
 
 def download_yaml_config(yaml_s3, local_path, sagemaker_session):
     """ download yaml config file
 
     Parameters
     ----------
@@ -144,15 +170,16 @@
     ------
     yaml_path: str
         Path to downloaded file
     """
     # Download training yaml file
     s3_url = urlparse(yaml_s3)
     yaml_file_name = s3_url.path.split('/')[-1]
-    assert yaml_file_name.endswith('yaml'), f"{yaml_s3} must be a yaml file."
+    assert yaml_file_name.endswith('yaml') or yaml_file_name.endswith('yml'), \
+        f"{yaml_s3} must be a yaml file."
     yaml_path = os.path.join(local_path, yaml_file_name)
     ### Download Partitioned graph data
 
     os.makedirs(local_path, exist_ok=True)
     try:
         S3Downloader.download(yaml_s3, local_path,
             sagemaker_session=sagemaker_session)
@@ -202,24 +229,51 @@
     Return
     ------
     graph_config_path: str
         Path to downloaded graph config file
     """
     # Download partitioned graph data.
     # Each training instance only download 1 partition.
-    graph_config = f"{graph_name}.json"
     graph_part = f"part{part_id}"
 
     graph_path = os.path.join(local_path, graph_name)
     graph_part_path = os.path.join(graph_path, graph_part)
     os.makedirs(graph_path, exist_ok=True)
     os.makedirs(graph_part_path, exist_ok=True)
-    try:
-        S3Downloader.download(os.path.join(graph_data_s3, graph_config),
+
+    graph_data_s3 = graph_data_s3[:-1] if graph_data_s3.endswith('/') else graph_data_s3
+
+    # We split on '/' to get the bucket, as it's always the third split element in an S3 URI
+    s3_input_bucket = graph_data_s3.split("/")[2]
+    # Similarly, by having maxsplit=3 we get the S3 key value as the fourth element
+    s3_input_key = graph_data_s3.split("/", maxsplit=3)[3]
+
+    s3_client = boto3.client('s3')
+    graph_config = None
+    for config_name  in [f"{graph_name}.json", "metadata.json"]:
+        try:
+            s3_client.head_object(Bucket=s3_input_bucket, Key=f"{s3_input_key}/{config_name}")
+            # This will only be accessed if the above doesn't trigger an exception
+            graph_config = config_name
+        except ClientError as err:
+            if err.response['ResponseMetadata']['HTTPStatusCode'] == 404:
+                # The key does not exist.
+                logging.debug("Metadata key %s does not exist",
+                            f"{s3_input_key}/{graph_config}")
+            elif err.response['Error']['Code'] == 403:
+                # Unauthorized, including invalid bucket
+                logging.error("Authorization error, check the path again: %s",
+                            f"{s3_input_key}/{graph_config}")
+            else:
+                # Something else has gone wrong.
+                raise err
+
+    S3Downloader.download(os.path.join(graph_data_s3, graph_config),
             graph_path, sagemaker_session=sagemaker_session)
+    try:
         S3Downloader.download(os.path.join(graph_data_s3, graph_part),
             graph_part_path, sagemaker_session=sagemaker_session)
     except Exception: # pylint: disable=broad-except
         print(f"Can not download graph_data from {graph_data_s3}.")
         raise RuntimeError(f"Can not download graph_data from {graph_data_s3}.")
 
     node_id_mapping = "node_mapping.pt"
```

## graphstorm/tracker/sagemaker_tracker.py

```diff
@@ -50,15 +50,18 @@
         step: int
             The corresponding step/iteration in the training loop.
         force_report: bool
             If true, report the metric
         """
         if force_report or self._do_report(step):
             if metric_value is not None:
-                print(f"Step {step} | {metric_name}: {metric_value:.4f}")
+                if isinstance(metric_value, str):
+                    print(f"Step {step} | {metric_name}: {metric_value}")
+                else:
+                    print(f"Step {step} | {metric_name}: {metric_value:.4f}")
 
     def log_train_metric(self, metric_name, metric_value, step, force_report=False):
         """ Log train metric
 
             Parameters
             ----------
             metric_name: str
```

## graphstorm/trainer/__init__.py

```diff
@@ -15,7 +15,8 @@
 
     Graphstorm trainer
 """
 from .lp_trainer import GSgnnLinkPredictionTrainer
 from .np_trainer import GSgnnNodePredictionTrainer
 from .ep_trainer import GSgnnEdgePredictionTrainer
 from .gsgnn_trainer import GSgnnTrainer
+from .glem_np_trainer import GLEMNodePredictionTrainer
```

## graphstorm/trainer/ep_trainer.py

```diff
@@ -12,15 +12,15 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     GraphStorm trainer for edge prediction
 """
 import time
-
+import resource
 import dgl
 import torch as th
 from torch.nn.parallel import DistributedDataParallel
 
 from ..model.edge_gnn import edge_mini_batch_gnn_predict, edge_mini_batch_predict
 from ..model.edge_gnn import GSgnnEdgeModelInterface
 from ..model.gnn import do_full_graph_inference, GSgnnModelBase, GSgnnModel
@@ -86,47 +86,44 @@
                     "The evaluator is provided but validation set is not provided."
         if not use_mini_batch_infer:
             assert isinstance(self._model, GSgnnModel), \
                     "Only GSgnnModel supports full-graph inference."
 
         # with freeze_input_layer_epochs is 0, computation graph will not be changed.
         static_graph = freeze_input_layer_epochs == 0
-        model = DistributedDataParallel(self._model, device_ids=[self.dev_id],
-                                        output_device=self.dev_id,
+        on_cpu = self.device == th.device('cpu')
+        model = DistributedDataParallel(self._model, device_ids=None if on_cpu else [self.device],
+                                        output_device=None if on_cpu else self.device,
                                         find_unused_parameters=True,
                                         static_graph=static_graph)
         device = model.device
         data = train_loader.data
 
         # Preparing input layer for training or inference.
         # The input layer can pre-compute node features in the preparing step if needed.
         # For example pre-compute all BERT embeddings
         if freeze_input_layer_epochs > 0:
             self._model.freeze_input_encoder(data)
         # TODO(xiangsx) Support freezing gnn encoder and decoder
 
         # training loop
-        dur = []
-        num_input_nodes = 0
-        forward_time = 0
-        back_time = 0
         total_steps = 0
         early_stop = False # used when early stop is True
         sys_tracker.check('start training')
         for epoch in range(num_epochs):
             model.train()
-            t0 = time.time()
+            epoch_start = time.time()
             if freeze_input_layer_epochs <= epoch:
                 self._model.unfreeze_input_encoder()
             # TODO(xiangsx) Support unfreezing gnn encoder and decoder
             rt_profiler.start_record()
+            batch_tic = time.time()
             for i, (input_nodes, batch_graph, blocks) in enumerate(train_loader):
                 rt_profiler.record('train_sample')
                 total_steps += 1
-                batch_tic = time.time()
 
                 if not isinstance(input_nodes, dict):
                     assert len(batch_graph.ntypes) == 1
                     input_nodes = {batch_graph.ntypes[0]: input_nodes}
                 input_feats = data.get_node_feats(input_nodes, device)
                 rt_profiler.record('train_node_feats')
 
@@ -135,41 +132,34 @@
                 assert len(batch_graph.etypes) == 1
                 target_etype = batch_graph.canonical_etypes[0]
                 # TODO(zhengda) the data loader should return labels directly.
                 seeds = batch_graph.edges[target_etype[1]].data[dgl.EID]
                 lbl = data.get_labels({target_etype: seeds}, device)
                 blocks = [block.to(device) for block in blocks]
                 batch_graph = batch_graph.to(device)
-                for _, nodes in input_nodes.items():
-                    num_input_nodes += nodes.shape[0]
                 rt_profiler.record('train_graph2GPU')
 
-                t2 = time.time()
                 # TODO(zhengda) we don't support edge features for now.
                 loss = model(blocks, batch_graph, input_feats, None, lbl, input_nodes)
                 rt_profiler.record('train_forward')
 
-                t3 = time.time()
                 self.optimizer.zero_grad()
                 loss.backward()
                 rt_profiler.record('train_backward')
                 self.optimizer.step()
                 rt_profiler.record('train_step')
-                forward_time += (t3 - t2)
-                back_time += (time.time() - t3)
 
                 self.log_metric("Train loss", loss.item(), total_steps)
 
                 if i % 20 == 0 and self.rank == 0:
                     rt_profiler.print_stats()
                     # Print task specific info.
                     print(
                         "Part {} | Epoch {:05d} | Batch {:03d} | Train Loss: {:.4f} | Time: {:.4f}".
                         format(self.rank, epoch, i, loss.item(), time.time() - batch_tic))
-                    num_input_nodes = forward_time = back_time = 0
 
                 val_score = None
                 if self.evaluator is not None and \
                     self.evaluator.do_eval(total_steps, epoch_end=False):
                     val_score = self.eval(model.module, val_loader, test_loader,
                                           use_mini_batch_infer, total_steps, return_proba=False)
 
@@ -187,25 +177,25 @@
                         # 1. There is no evaluation, we will keep the
                         #    latest K models.
                         # 2. There is evaluaiton, we need to follow the
                         #    guidance of validation score.
                         self.save_topk_models(model, epoch, i, val_score, save_model_path)
 
                 rt_profiler.record('train_eval')
+                batch_tic = time.time()
                 # early_stop, exit current interation.
                 if early_stop is True:
                     break
 
             # ------- end of an epoch -------
 
             th.distributed.barrier()
-            epoch_time = time.time() - t0
+            epoch_time = time.time() - epoch_start
             if self.rank == 0:
                 print("Epoch {} take {}".format(epoch, epoch_time))
-            dur.append(epoch_time)
 
             val_score = None
             if self.evaluator is not None and self.evaluator.do_eval(total_steps, epoch_end=True):
                 val_score = self.eval(model.module, val_loader, test_loader, use_mini_batch_infer,
                                       total_steps, return_proba=False)
 
                 if self.evaluator.do_early_stop(val_score):
@@ -220,19 +210,26 @@
             th.distributed.barrier()
 
             # early_stop, exit training
             if early_stop is True:
                 break
 
         rt_profiler.save_profile()
-        print("Peak Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) / 1024 /1024))
+        if th.cuda.is_available():
+            print("Peak GPU Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) /
+                                                         1024 / 1024))
+        else:
+            print("Peak RAM Mem alloc: {:.4f} MB".format(
+                  resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024))
         if self.rank == 0 and self.evaluator is not None:
             output = {'best_test_score': self.evaluator.best_test_score,
                        'best_val_score': self.evaluator.best_val_score,
-                       'peak_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_GPU_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_RAM_mem_alloc_MB': \
+                           resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024,
                        'best validation iteration': \
                            self.evaluator.best_iter_num[self.evaluator.metric[0]],
                        'best model path': \
                            self.get_best_model_path() if save_model_path is not None else \
                                "No model is saved, please set save_model_path"}
             self.log_params(output)
 
@@ -266,26 +263,37 @@
         test_start = time.time()
         sys_tracker.check('start prediction')
         model.eval()
         if use_mini_batch_infer:
             val_pred, val_label = edge_mini_batch_gnn_predict(model, val_loader, return_proba,
                                                               return_label=True)
             sys_tracker.check("after_val_score")
-            test_pred, test_label = edge_mini_batch_gnn_predict(model, test_loader, return_proba,
-                                                                return_label=True)
+            if test_loader is not None:
+                test_pred, test_label = \
+                    edge_mini_batch_gnn_predict(model, test_loader, return_proba,
+                                                return_label=True)
+            else: # there is no test set
+                test_pred = None
+                test_label = None
             sys_tracker.check("after_test_score")
         else:
             emb = do_full_graph_inference(model, val_loader.data, fanout=val_loader.fanout,
                                           task_tracker=self.task_tracker)
 
             val_pred, val_label = edge_mini_batch_predict(model, emb, val_loader, return_proba,
                                                           return_label=True)
             sys_tracker.check("after_val_score")
-            test_pred, test_label = edge_mini_batch_predict(model, emb, test_loader, return_proba,
-                                                            return_label=True)
+            if test_loader is not None:
+                test_pred, test_label = \
+                    edge_mini_batch_predict(model, emb, test_loader, return_proba,
+                                            return_label=True)
+            else:
+                # there is no test set
+                test_pred = None
+                test_label = None
             sys_tracker.check("after_test_score")
 
         model.train()
         sys_tracker.check('predict')
         val_score, test_score = self.evaluator.evaluate(val_pred, test_pred,
                                                         val_label, test_label, total_steps)
         sys_tracker.check('evaluate')
```

## graphstorm/trainer/gsgnn_trainer.py

```diff
@@ -46,40 +46,36 @@
         if not isinstance(optimizer, GSOptimizer):
             if rank == 0:
                 print("Warining: the optimizer is not GSOptimizer. "
                         + "Convert it to GSOptimizer.")
             optimizer = GSOptimizer([optimizer])
         self._optimizer = optimizer
         self._rank = rank
-        self._dev_id = -1
+        self._device = -1
         self._evaluator = None
         self._task_tracker = None
         self._best_model_path = None
 
         assert topk_model_to_save >= 0
         self._topklist = TopKList(topk_model_to_save)    # A list to store the top k best
                                                         # perf epoch+iteration for
                                                         # saving/removing models.
 
-    def setup_cuda(self, dev_id):
-        """ Set up the CUDA device of this trainer.
+    def setup_device(self, device):
+        """ Set up the device of this trainer.
 
         The CUDA device is set up based on the local rank.
 
         Parameters
         ----------
-        dev_id : int
-            The device ID for model training.
+        device :
+            The device for model training.
         """
-        # setup cuda env
-        use_cuda = th.cuda.is_available()
-        assert use_cuda, "Only support GPU training"
-        th.cuda.set_device(dev_id)
-        self._dev_id = dev_id
-        self._model = self._model.to(self.dev_id)
+        self._device = th.device(device)
+        self._model = self._model.to(self.device)
         self._optimizer.move_to_device(self._model.device)
 
     def setup_task_tracker(self, task_tracker):
         """ Set the task tracker.
 
         Parameters
         ----------
@@ -304,20 +300,19 @@
             The current iteration
         num_input_nodes: int
             number of input nodes
         compute_time: tuple of ints
             A tuple of (forward time and backward time)
         '''
         gnn_forward_time, back_time = compute_time
-        device = 'cuda:%d' % self.dev_id
 
-        print("Epoch {:05d} | Batch {:03d} | GPU Mem reserved: {:.4f} MB | Peak Mem: {:.4f} MB".
+        print("Epoch {:05d} | Batch {:03d} | GPU Mem reserved: {:.4f} MB | GPU Peak Mem: {:.4f} MB".
                 format(epoch, i,
-                    th.cuda.memory_reserved(device) / 1024 / 1024,
-                    th.cuda.max_memory_allocated(device) / 1024 /1024))
+                    th.cuda.memory_reserved(self.device) / 1024 / 1024,
+                    th.cuda.max_memory_allocated(self.device) / 1024 /1024))
         print('Epoch {:05d} | Batch {:03d} | RAM memory {} used | Avg input nodes per iter {}'.
                 format(epoch, i, psutil.virtual_memory(), num_input_nodes))
         print('Epoch {:05d} | Batch {:03d} | forward {:05f} | Backward {:05f}'.format(
             epoch, i, gnn_forward_time, back_time))
 
     def restore_model(self, model_path, model_layer_to_load=None):
         """ Restore a GNN model and the optimizer.
@@ -354,17 +349,17 @@
     @property
     def task_tracker(self):
         """ The task tracker associated with the trainer.
         """
         return self._task_tracker
 
     @property
-    def dev_id(self):
+    def device(self):
         """ The device associated with the trainer.
         """
-        return self._dev_id
+        return self._device
 
     @property
     def rank(self):
         """ The rank of the trainer.
         """
         return self._rank
```

## graphstorm/trainer/lp_trainer.py

```diff
@@ -12,14 +12,15 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     GraphStorm trainer for link prediction
 """
 import time
+import resource
 import torch as th
 from torch.nn.parallel import DistributedDataParallel
 
 from ..model.lp_gnn import GSgnnLinkPredictionModelInterface
 from ..model.lp_gnn import lp_mini_batch_predict
 from ..model.gnn import do_full_graph_inference, GSgnnModelBase, GSgnnModel
 from .gsgnn_trainer import GSgnnTrainer
@@ -87,84 +88,74 @@
             Default: 0, no freeze.
         """
         if not use_mini_batch_infer:
             assert isinstance(self._model, GSgnnModel), \
                     "Only GSgnnModel supports full-graph inference."
         # with freeze_input_layer_epochs is 0, computation graph will not be changed.
         static_graph = freeze_input_layer_epochs == 0
-        model = DistributedDataParallel(self._model, device_ids=[self.dev_id],
-                                        output_device=self.dev_id,
+        on_cpu = self.device == th.device('cpu')
+        model = DistributedDataParallel(self._model, device_ids=None if on_cpu else [self.device],
+                                        output_device=None if on_cpu else self.device,
                                         find_unused_parameters=True,
                                         static_graph=static_graph)
         device = model.device
         data = train_loader.data
 
         # Preparing input layer for training or inference.
         # The input layer can pre-compute node features in the preparing step if needed.
         # For example pre-compute all BERT embeddings
         if freeze_input_layer_epochs > 0:
             self._model.freeze_input_encoder(data)
         # TODO(xiangsx) Support freezing gnn encoder and decoder
 
         # training loop
-        dur = []
-        num_input_nodes = 0
         total_steps = 0
         early_stop = False # used when early stop is True
-        forward_time = 0
-        back_time = 0
         sys_tracker.check('start training')
         for epoch in range(num_epochs):
             model.train()
-            t0 = time.time()
+            epoch_start = time.time()
 
             if freeze_input_layer_epochs <= epoch:
                 self._model.unfreeze_input_encoder()
             # TODO(xiangsx) Support unfreezing gnn encoder and decoder
 
             rt_profiler.start_record()
+            batch_tic = time.time()
             for i, (input_nodes, pos_graph, neg_graph, blocks) in enumerate(train_loader):
                 rt_profiler.record('train_sample')
                 total_steps += 1
-                batch_tic = time.time()
 
                 if not isinstance(input_nodes, dict):
                     assert len(pos_graph.ntypes) == 1
                     input_nodes = {pos_graph.ntypes[0]: input_nodes}
                 input_feats = data.get_node_feats(input_nodes, device)
                 rt_profiler.record('train_node_feats')
 
                 pos_graph = pos_graph.to(device)
                 neg_graph = neg_graph.to(device)
                 blocks = [blk.to(device) for blk in blocks]
-                for _, nodes in input_nodes.items():
-                    num_input_nodes += nodes.shape[0]
                 rt_profiler.record('train_graph2GPU')
 
-                t2 = time.time()
                 # TODO(zhengda) we don't support edge features for now.
                 loss = model(blocks, pos_graph, neg_graph,
                              input_feats, None, input_nodes)
                 rt_profiler.record('train_forward')
 
-                t3 = time.time()
                 self.optimizer.zero_grad()
                 loss.backward()
                 rt_profiler.record('train_backward')
                 self.optimizer.step()
                 rt_profiler.record('train_step')
-                forward_time += (t3 - t2)
-                back_time += (time.time() - t3)
 
                 self.log_metric("Train loss", loss.item(), total_steps)
                 if i % 20 == 0 and self.rank == 0:
                     rt_profiler.print_stats()
                     print("Epoch {:05d} | Batch {:03d} | Train Loss: {:.4f} | Time: {:.4f}".
                             format(epoch, i, loss.item(), time.time() - batch_tic))
-                    num_input_nodes = forward_time = back_time = 0
 
                 val_score = None
                 if self.evaluator is not None and \
                     self.evaluator.do_eval(total_steps, epoch_end=False):
                     val_score = self.eval(model.module, data,
                                           val_loader, test_loader, total_steps,
                                           edge_mask_for_gnn_embeddings)
@@ -181,26 +172,26 @@
                         # We will save the best model when
                         # 1. There is no evaluation, we will keep the
                         #    latest K models.
                         # 2. There is evaluaiton, we need to follow the
                         #    guidance of validation score.
                         self.save_topk_models(model, epoch, i, val_score, save_model_path)
 
+                batch_tic = time.time()
                 rt_profiler.record('train_eval')
                 # early_stop, exit current interation.
                 if early_stop is True:
                     break
 
             # ------- end of an epoch -------
 
             th.distributed.barrier()
-            epoch_time = time.time() - t0
+            epoch_time = time.time() - epoch_start
             if self.rank == 0:
                 print("Epoch {} take {}".format(epoch, epoch_time))
-            dur.append(epoch_time)
 
             val_score = None
             if self.evaluator is not None and self.evaluator.do_eval(total_steps, epoch_end=True):
                 val_score = self.eval(model.module, data,
                                       val_loader, test_loader, total_steps,
                                       edge_mask_for_gnn_embeddings)
 
@@ -208,27 +199,35 @@
                     early_stop = True
 
             # After each epoch, check to save the top k models. If has validation score, will save
             # the best top k. But if no validation, will either save the last k model or all models
             # depends on the setting of top k. To show this is after epoch save, set the iteration
             # to be None, so that we can have a determistic model folder name for testing and debug.
             self.save_topk_models(model, epoch, None, val_score, save_model_path)
+            rt_profiler.print_stats()
 
             th.distributed.barrier()
 
             # early_stop, exit training
             if early_stop is True:
                 break
 
         rt_profiler.save_profile()
-        print("Peak Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) / 1024 /1024))
+        if th.cuda.is_available():
+            print("Peak GPU Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) /
+                                                         1024 / 1024))
+        else:
+            print("Peak RAM Mem alloc: {:.4f} MB".format(
+                  resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024))
         if self.rank == 0 and self.evaluator is not None:
             output = {'best_test_mrr': self.evaluator.best_test_score,
                        'best_val_mrr':self.evaluator.best_val_score,
-                       'peak_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_GPU_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_RAM_mem_alloc_MB': \
+                           resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024,
                        'best validation iteration': \
                            self.evaluator.best_iter_num[self.evaluator.metric[0]],
                        'best model path': \
                            self.get_best_model_path() if save_model_path is not None else None}
             self.log_params(output)
 
             if save_perf_results_path is not None:
@@ -257,24 +256,26 @@
         Returns
         -------
         float: validation score
         """
         test_start = time.time()
         sys_tracker.check('before prediction')
         model.eval()
+
         emb = do_full_graph_inference(model, data, fanout=val_loader.fanout,
                                       edge_mask=edge_mask_for_gnn_embeddings,
                                       task_tracker=self.task_tracker)
         sys_tracker.check('compute embeddings')
-        device = th.device(f"cuda:{self.dev_id}") \
-            if self.dev_id >= 0 else th.device("cpu")
-        val_scores = lp_mini_batch_predict(model, emb, val_loader, device) \
+        val_scores = lp_mini_batch_predict(model, emb, val_loader, self.device) \
             if val_loader is not None else None
         sys_tracker.check('after_val_score')
-        test_scores = lp_mini_batch_predict(model, emb, test_loader, device)
+        if test_loader is not None:
+            test_scores = lp_mini_batch_predict(model, emb, test_loader, self.device)
+        else:
+            test_scores = None
         sys_tracker.check('after_test_score')
         val_score, test_score = self.evaluator.evaluate(
             val_scores, test_scores, total_steps)
         sys_tracker.check('evaluate validation/test')
         model.train()
 
         if self.rank == 0:
```

## graphstorm/trainer/np_trainer.py

```diff
@@ -12,14 +12,15 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     GraphStorm trainer for node prediction.
 """
 import time
+import resource
 import torch as th
 from torch.nn.parallel import DistributedDataParallel
 
 from ..model.node_gnn import node_mini_batch_gnn_predict, node_mini_batch_predict
 from ..model.node_gnn import GSgnnNodeModelInterface
 from ..model.gnn import do_full_graph_inference, GSgnnModelBase, GSgnnModel
 from .gsgnn_trainer import GSgnnTrainer
@@ -84,84 +85,74 @@
                     "The evaluator is provided but validation set is not provided."
         if not use_mini_batch_infer:
             assert isinstance(self._model, GSgnnModel), \
                     "Only GSgnnModel supports full-graph inference."
 
         # with freeze_input_layer_epochs is 0, computation graph will not be changed.
         static_graph = freeze_input_layer_epochs == 0
-        model = DistributedDataParallel(self._model, device_ids=[self.dev_id],
-                                        output_device=self.dev_id,
+        on_cpu = self.device == th.device('cpu')
+        model = DistributedDataParallel(self._model, device_ids=None if on_cpu else [self.device],
+                                        output_device=None if on_cpu else self.device,
                                         find_unused_parameters=True,
                                         static_graph=static_graph)
         device = model.device
         data = train_loader.data
 
         # Preparing input layer for training or inference.
         # The input layer can pre-compute node features in the preparing step if needed.
         # For example pre-compute all BERT embeddings
         if freeze_input_layer_epochs > 0:
             self._model.freeze_input_encoder(data)
         # TODO(xiangsx) Support freezing gnn encoder and decoder
 
         # training loop
-        dur = []
         total_steps = 0
-        num_input_nodes = 0
-        forward_time = 0
-        back_time = 0
         early_stop = False # used when early stop is True
         sys_tracker.check('start training')
         g = data.g
         for epoch in range(num_epochs):
             model.train()
-            t0 = time.time()
+            epoch_start = time.time()
             if freeze_input_layer_epochs <= epoch:
                 self._model.unfreeze_input_encoder()
             # TODO(xiangsx) Support unfreezing gnn encoder and decoder
 
             # TODO(zhengda) the dataloader should return node features and labels directly.
             rt_profiler.start_record()
+            batch_tic = time.time()
             for i, (input_nodes, seeds, blocks) in enumerate(train_loader):
                 rt_profiler.record('train_sample')
                 total_steps += 1
-                batch_tic = time.time()
 
                 if not isinstance(input_nodes, dict):
                     assert len(g.ntypes) == 1
                     input_nodes = {g.ntypes[0]: input_nodes}
                 input_feats = data.get_node_feats(input_nodes, device)
                 lbl = data.get_labels(seeds, device)
                 rt_profiler.record('train_node_feats')
 
                 blocks = [block.to(device) for block in blocks]
-                for _, feats in input_feats.items():
-                    num_input_nodes += feats.shape[0]
                 rt_profiler.record('train_graph2GPU')
 
-                t2 = time.time()
                 # TODO(zhengda) we don't support edge features for now.
                 loss = model(blocks, input_feats, None, lbl, input_nodes)
                 rt_profiler.record('train_forward')
 
-                t3 = time.time()
                 self.optimizer.zero_grad()
                 loss.backward()
                 rt_profiler.record('train_backward')
                 self.optimizer.step()
                 rt_profiler.record('train_step')
-                forward_time += (t3 - t2)
-                back_time += (time.time() - t3)
 
                 self.log_metric("Train loss", loss.item(), total_steps)
 
                 if i % 20 == 0 and self.rank == 0:
                     rt_profiler.print_stats()
                     print("Part {} | Epoch {:05d} | Batch {:03d} | Loss: {:.4f} | Time: {:.4f}".
                             format(self.rank, epoch, i,  loss.item(), time.time() - batch_tic))
-                    num_input_nodes = forward_time = back_time = 0
 
                 val_score = None
                 if self.evaluator is not None and \
                     self.evaluator.do_eval(total_steps, epoch_end=False) and \
                     val_loader is not None:
                     val_score = self.eval(model.module, val_loader, test_loader,
                                           use_mini_batch_infer, total_steps, return_proba=False)
@@ -180,24 +171,24 @@
                         # 1. There is no evaluation, we will keep the
                         #    latest K models.
                         # 2. There is evaluaiton, we need to follow the
                         #    guidance of validation score.
                         self.save_topk_models(model, epoch, i, val_score, save_model_path)
 
                 rt_profiler.record('train_eval')
+                batch_tic = time.time()
                 # early_stop, exit current interation.
                 if early_stop is True:
                     break
 
             # end of an epoch
             th.distributed.barrier()
-            epoch_time = time.time() - t0
+            epoch_time = time.time() - epoch_start
             if self.rank == 0:
                 print("Epoch {} take {}".format(epoch, epoch_time))
-            dur.append(epoch_time)
 
             val_score = None
             if self.evaluator is not None and self.evaluator.do_eval(total_steps, epoch_end=True):
                 val_score = self.eval(model.module, val_loader, test_loader,
                                       use_mini_batch_infer, total_steps, return_proba=False)
                 if self.evaluator.do_early_stop(val_score):
                     early_stop = True
@@ -209,19 +200,26 @@
             self.save_topk_models(model, epoch, None, val_score, save_model_path)
 
             # early_stop, exit training
             if early_stop is True:
                 break
 
         rt_profiler.save_profile()
-        print("Peak Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) / 1024 /1024))
+        if th.cuda.is_available():
+            print("Peak GPU Mem alloc: {:.4f} MB".format(th.cuda.max_memory_allocated(device) /
+                                                         1024 / 1024))
+        else:
+            print("Peak RAM Mem alloc: {:.4f} MB".format(
+                  resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024))
         if self.rank == 0 and self.evaluator is not None:
             output = {'best_test_score': self.evaluator.best_test_score,
                        'best_val_score': self.evaluator.best_val_score,
-                       'peak_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_GPU_mem_alloc_MB': th.cuda.max_memory_allocated(device) / 1024 / 1024,
+                       'peak_RAM_mem_alloc_MB': \
+                           resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1024,
                        'best validation iteration': \
                            self.evaluator.best_iter_num[self.evaluator.metric[0]],
                        'best model path': \
                            self.get_best_model_path() if save_model_path is not None else None}
             self.log_params(output)
 
             if save_perf_results_path is not None:
@@ -251,26 +249,37 @@
         """
         teval = time.time()
         sys_tracker.check('before prediction')
         if use_mini_batch_infer:
             val_pred, _, val_label = node_mini_batch_gnn_predict(model, val_loader, return_proba,
                                                                  return_label=True)
             sys_tracker.check('after_val_score')
-            test_pred, _, test_label = node_mini_batch_gnn_predict(model, test_loader, return_proba,
-                                                                   return_label=True)
+            if test_loader is not None:
+                test_pred, _, test_label = \
+                    node_mini_batch_gnn_predict(model, test_loader, return_proba,
+                                                return_label=True)
+            else: # there is no test set
+                test_pred = None
+                test_label = None
             sys_tracker.check('after_test_score')
         else:
             emb = do_full_graph_inference(model, val_loader.data, fanout=val_loader.fanout,
                                           task_tracker=self.task_tracker)
             sys_tracker.check('after_full_infer')
             val_pred, val_label = node_mini_batch_predict(model, emb, val_loader, return_proba,
                                                           return_label=True)
             sys_tracker.check('after_val_score')
-            test_pred, test_label = node_mini_batch_predict(model, emb, test_loader, return_proba,
-                                                            return_label=True)
+            if test_loader is not None:
+                test_pred, test_label = \
+                    node_mini_batch_predict(model, emb, test_loader, return_proba,
+                                            return_label=True)
+            else:
+                # there is no test set
+                test_pred = None
+                test_label = None
             sys_tracker.check('after_test_score')
         sys_tracker.check('predict')
         val_score, test_score = self.evaluator.evaluate(val_pred, test_pred,
                                                         val_label, test_label, total_steps)
         sys_tracker.check('evaluate')
         if self.rank == 0:
             self.log_print_metrics(val_score=val_score,
```

## Comparing `graphstorm-0.1.1rc2.dist-info/LICENSE` & `graphstorm-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `graphstorm-0.1.1rc2.dist-info/RECORD` & `graphstorm-0.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,94 +1,100 @@
-graphstorm/__init__.py,sha256=LmxIDQFQBXax4G2sBse6Ev_aiGjL7wCKGDqWfpM9W6Q,1033
-graphstorm/gsf.py,sha256=--v17VvbyAPEbnmanluNllru2iig_VXQBTd-cJlB2N8,21084
-graphstorm/utils.py,sha256=91qTte_GUK9TQSHtPlndEQsiVk7hmKIZ7zWEt8X7Cn8,13143
+graphstorm/__init__.py,sha256=kbhQjetc95AB0CFEWqNpJgV5nPixmt3vtp04PZWGopc,1030
+graphstorm/gsf.py,sha256=Itr0YNWwJrnfRB2BV-A5Bqal-J7mQ-KLjqu_b79S1Kw,21690
+graphstorm/utils.py,sha256=IaSpg1i8BziLkuluo1gKJnpBSLK4EI3iytUI3tIru3M,13370
 graphstorm/config/__init__.py,sha256=yoDCNKMjfIIwusEbAjBy063onP4v24AUzQf_bVZPglc,1320
-graphstorm/config/argument.py,sha256=aK2d0pPHlQa2H-BkuGdwpbJL77ZBHQRL2TpBHprsBck,75206
+graphstorm/config/argument.py,sha256=zU-zbRQlWh3AndVGltWHHkaBns3EVLyvhKlJmNT1buo,81412
 graphstorm/config/config.py,sha256=VroNYn5hVYasii8VwCZBYUpRYwj4qhl6OyFPulAQ95Y,2164
 graphstorm/config/utils.py,sha256=4ZBpWSJYZdEDWPwY7RAcZtK3bOXf8G7aNNIqLr6DKXc,989
 graphstorm/data/__init__.py,sha256=Syass-XNCLT2R3Fjx4j_m4_Y0XKZWKMu_Oi-nmjOW5k,941
 graphstorm/data/constants.py,sha256=3F9_6fOGw41rSFL4MHS64EYFfTBPwoEMpiKTLGUyHeE,997
 graphstorm/data/dataset.py,sha256=5RxhtgAn_aXBsmswWAn4vr6KCzmgvvKczz7its_ykVY,3265
 graphstorm/data/mag_lsc.py,sha256=snjXqPmlXY72o3P5Z7rGeelKZaZ1yortxs4FBfPZ6Hc,8270
 graphstorm/data/movielens.py,sha256=YSBgRkGLJlyUdxENzM2aNBYT2_nS0CB1miGLm5FHiTU,14665
 graphstorm/data/ogbn_datasets.py,sha256=CIEacUy33bSVGPvnawdzkZI_8uuUZ1oPVcDrIxdAH6w,11231
 graphstorm/data/ogbn_mag.py,sha256=cKPzNeDh4rwAGa4_X7uoVDi8lPSZeq7ZheNH3sxHXX0,9541
 graphstorm/data/text_dataset.py,sha256=qoqLVVHJFRckgVDpp4NlxpFHrxwE7Kr5zQPbg1Ycg5U,4907
 graphstorm/data/utils.py,sha256=Sd6ShU9qWAUVGBx8DrBvjoVozJLSt-Kpd1YHuQ-hi9Q,10819
-graphstorm/dataloading/__init__.py,sha256=MPuMeOknfYG28UIdWt8NvuN8ATbFWfi8ijOpTcyfGdY,1831
-graphstorm/dataloading/dataloading.py,sha256=8eYZ6XIXoDFEKhXt_JMDdYZqaA0MeLSL65WuJmnllAU,28498
-graphstorm/dataloading/dataset.py,sha256=iLH8nMvxkfdZ6APBA-Ug7S51M5aAuNstOBamGHffj7Y,25845
-graphstorm/dataloading/sampler.py,sha256=y37LdCAYIcpXOjMq55NyoBw_VE2mVAqnMPYijLpLUqQ,9483
-graphstorm/dataloading/utils.py,sha256=p31TUqMfyWuQdd8sAMWm5t2yyiR6J_VX4B0e4G9tMLQ,3145
+graphstorm/dataloading/__init__.py,sha256=CKvBcS8AGZ_5VaGqriPsxdM_N1Yh-7qe2mgncHUt86s,2333
+graphstorm/dataloading/dataloading.py,sha256=ansrZr7V05webf2oYoeNdM-EKhKJ1hW6uS_WbKXMq00,32504
+graphstorm/dataloading/dataset.py,sha256=FWWkLACry8g8CAP6XpesBoGrluzn6sgkjKG1QS05z3k,28233
+graphstorm/dataloading/sampler.py,sha256=vPEHoUwB6Mi6r6gY180f-Gm3TvpXkFtlQ7Rv9p7FqAE,15791
+graphstorm/dataloading/utils.py,sha256=eXkG-e63VCYh_QuS3CaO38gw1C91nvaqfQVuKZvsfJI,3097
 graphstorm/eval/__init__.py,sha256=mdNua_QDb7zhfBC7z8W8zpukTGizTdNOedC1idujjbA,1261
-graphstorm/eval/eval_func.py,sha256=iKQChJNVniW2N1bA1n1fP-D1DKPRXeBAGWUpSDlU2YE,13568
-graphstorm/eval/evaluator.py,sha256=_v4HkdOJz-TYZ_AarTrQXgCioT6IRYIVvqJrzSEysgA,31913
+graphstorm/eval/eval_func.py,sha256=52oOXGayDALtHSO1KDVxtBTxs0JLJm1iTL3Pc7tpG_0,14472
+graphstorm/eval/evaluator.py,sha256=duGM0npsivGm2uxPEXsPjsoOjFXr_fgG9CLtoC8SZrI,32353
 graphstorm/eval/utils.py,sha256=mnyjNUHvaZmaCZIo6pD9SEcCmGkr2AghyEuvNQWJkN4,9574
 graphstorm/gconstruct/__init__.py,sha256=kloTg9YbXUPAsKE8R7NrvRXyQDLT3dfONt5uRWqAs68,655
-graphstorm/gconstruct/construct_graph.py,sha256=xA6cROYYBPf9p6AZ8ryI_yRmSqAUIm9T8HVzeGfLldQ,30122
-graphstorm/gconstruct/file_io.py,sha256=NpLXWALF82v3NvntIxIjnDoqKd-tRhNC7CZZBJWo_Gg,12338
-graphstorm/gconstruct/id_map.py,sha256=AZnMTGsu7e4_xzuSC1KdBRd5jcx_5gwT2VSCYQ0Z7mo,6619
-graphstorm/gconstruct/transform.py,sha256=YRDz1FyAQ2ZEs8vjiVr38TIkSfoy-5BB7rdjHQ2pUCI,38750
-graphstorm/gconstruct/utils.py,sha256=tAb6ZuAf6m-dpoIh6vO4ekOlpu6Bk2yKh0dpdfNZn64,17952
+graphstorm/gconstruct/construct_graph.py,sha256=AalGGXOAAkiEJ8DXEtwcQP5W13UCQssu_RPzsA7rRAI,32393
+graphstorm/gconstruct/file_io.py,sha256=P6kvjRdUqtswB5DhhlV7tNNmzQZN5xTY9UdX6rgQYew,11781
+graphstorm/gconstruct/id_map.py,sha256=orBB7KV_Q14hwKe48Qr2ElXhghoK3OzUxXYzP7rJEhs,7626
+graphstorm/gconstruct/transform.py,sha256=TIo5mwc_ZM_PPjN-d4KiwzxCjmjfKuXPdOT2Y2qqwu4,43616
+graphstorm/gconstruct/utils.py,sha256=gGvFlwNNl7mtLPJZ5lRaWFEJ_c90cND8y7ZI762GupY,24737
 graphstorm/inference/__init__.py,sha256=xNGVU5x9HgQ9e5VPGAExkvu541ZFivBFym-i1vIPr9g,769
-graphstorm/inference/ep_infer.py,sha256=VYRM-3T98NsdU7sPgV3acI1P07hwhCK_c20RNLhbnK8,5682
-graphstorm/inference/graphstorm_infer.py,sha256=vnaWuaEm9xw3-1QIrwZYOEEW5C4zA7WbdrvEe9wIz-M,3697
-graphstorm/inference/lp_infer.py,sha256=IzE0Vdjd9muGr3jGv45Hm-FC6N3xxQi2NpGBdkpygj0,4155
-graphstorm/inference/np_infer.py,sha256=8cF0PWixBlo64uMSZOGKAhlS6sN4p6m7ChLon2giZLY,6446
+graphstorm/inference/ep_infer.py,sha256=0tvK3t6T-SdA8kJCW_v2EMTDdAM8Ekh_KodSfBsgTYg,5816
+graphstorm/inference/graphstorm_infer.py,sha256=PmH2y67lu6QmepYXLoZJKuQ82NlNgmeMTnZp-MoVQcg,3533
+graphstorm/inference/lp_infer.py,sha256=GZil1VUd8urCMCBOmnDZdR-MwKwk3o6wcVUCisuAFis,4074
+graphstorm/inference/np_infer.py,sha256=LhqcnloCSWGS5bju1CVM4xmpfo7JESjx3EMxAVOU2no,6586
 graphstorm/model/__init__.py,sha256=Z2s0saeIKYK1tqAhDwIrQkLRCPagzyIs-zK36kIcXCA,1834
 graphstorm/model/edge_decoder.py,sha256=bwEH43XG4cwP2tu8_JcBaCfR1XRlVdCTad-e70kSl90,34792
-graphstorm/model/edge_gnn.py,sha256=vwadEjfTnG4eEE-J6p_uZ379qyEYpMRd9TMWXVkL4VI,9963
-graphstorm/model/embed.py,sha256=ajPV_55HynKWUyQIhF0x97bFhcxXKse1hDy5nCfLDKY,13433
+graphstorm/model/edge_gnn.py,sha256=mf8o7Zgp329WbBHE4ILya3sf6h_td4pcGcKmhFxfuDE,10215
+graphstorm/model/embed.py,sha256=KDsJaZUXz9fiEP_-pVlRe0s2-4U4_99Mb6YLSxkoMyc,14220
 graphstorm/model/gnn.py,sha256=NJ0s95mR2JSefaFSvDfbDjTs7x5v1V2AMIh9if80G5A,26383
-graphstorm/model/gnn_encoder_base.py,sha256=OHiBXO5jZ_iPtaVAGs79asamPvm7v3QZo_Ay6FP-Kwo,5783
+graphstorm/model/gnn_encoder_base.py,sha256=Kc9tfsaJ2fwo7CeXbmys1Zw0yCpSNUuqwbiL1lDKq_A,5982
 graphstorm/model/gs_layer.py,sha256=QSBR9YrGsXjsA2bSlo0jg8EQ8NVmjpDGa3gP2bqvCZc,2573
 graphstorm/model/lm_embed.py,sha256=nqHzo3I_A6bH4YpVXlA_3BYFMS0d_ZdiE_dPK0LhDuw,17036
 graphstorm/model/loss_func.py,sha256=WtGAQTGpzcq6Z-IITRaG2miciIxmiqLocF2OhALzTgc,4830
 graphstorm/model/lp_gnn.py,sha256=NtlPGGvyISLf9pfa-17W-0dmeJoQgQ9-VlLck9dZihM,5718
+graphstorm/model/ngnn_mlp.py,sha256=O1QUCyLDkX67YoeCgy-XGcQsy35NzxZ0tyQUmCmAI8Q,2385
 graphstorm/model/node_decoder.py,sha256=uFEToqQ8BZG9EspyGfZPRpCX_35MKSlnekDYN_J0Dcs,4502
-graphstorm/model/node_gnn.py,sha256=XrkGNnj06B2jlTKAl_1oHBIFQp5cPUQJbNas8bmS-tk,9019
-graphstorm/model/rgat_encoder.py,sha256=aM5eB0PPkMeGkvngV8gwWdow7F96W0hVlh8kN3Oh9xM,6096
-graphstorm/model/rgcn_encoder.py,sha256=a3JKM627iTbWEPZEVVO3p53ZrUV_nV24tkjLS6YJMl4,7156
-graphstorm/model/utils.py,sha256=Euv5-GCOnQBuQ51gUa18RwM_2FM2Kmehd8ydpWlmsz0,32293
+graphstorm/model/node_glem.py,sha256=uagimb4FRtNzgqtIeYSt7YxZ1tv7ekdfTCQb9P9i__8,13943
+graphstorm/model/node_gnn.py,sha256=G5uyR8071bsOjxH-fgsJg7pMAnybncGSbuq1--JDzYg,9425
+graphstorm/model/rgat_encoder.py,sha256=9DNjMULliSG_FLGtQTe4MRvHozQgJbHwMjaqfI0WG2M,6901
+graphstorm/model/rgcn_encoder.py,sha256=Dc1OkknH7iFNZwxVZuFUdlO14jE1n6cMsUa6ynq70dI,7944
+graphstorm/model/utils.py,sha256=STWv3C-LwjEFudCyEReRZNpBA_VKJVB7syRoFMpLdSQ,32304
 graphstorm/model/lm_model/__init__.py,sha256=YQWOkUIUoQHwwJae1-CY8vWcOSWI0eXAGFP5Bn7OCnc,841
 graphstorm/model/lm_model/hf_bert.py,sha256=feYjVuBTkM1Aqe3RMDRjiJGZh_vy0tRDMyJ5OJBlMME,11149
 graphstorm/model/lm_model/lm_model.py,sha256=7xVwmYNYAyiGEfTF-ziqQYzo_SoBxqbExqrYhRkEhc8,3955
 graphstorm/model/lm_model/utils.py,sha256=jxkTwOBt57eMYw5ENcO6tJnF-lCql2wRUDPQaMClT_s,2294
 graphstorm/run/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 graphstorm/run/gs_edge_classification.py,sha256=3KLqQUz1p8-U06euUsncgXC8x_1TqEPdW8esPPfEMgk,1648
 graphstorm/run/gs_edge_regression.py,sha256=05-YO02nwQsicdPKTof6SOiklfjVLB0d0dQ1Lbzu8RY,1640
 graphstorm/run/gs_link_prediction.py,sha256=nG-VylP34d3UHgRoUiHQj-PZoAT3EIuuE-D23Gex9Fc,1875
 graphstorm/run/gs_node_classification.py,sha256=mnmd1vb1A1FMRzee4n1hR-QLxVA6pLtyv88YuePrsKM,1523
 graphstorm/run/gs_node_regression.py,sha256=TTKdAFDjzHI1LLeIZ4f6SHG7OcZuv393VUPUvxxciy0,1515
-graphstorm/run/launch.py,sha256=O6DRpKRNgfzQkru-Ze7GBIthH8XAXX4cZ2T41CyMiNQ,30523
+graphstorm/run/launch.py,sha256=IHOSzrd2KAhIF1az2kT7hBb7YhOjz2ZuKFPDDSJBejM,31201
 graphstorm/run/gsgnn_ep/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-graphstorm/run/gsgnn_ep/ep_infer_gnn.py,sha256=atzZV4Qs0nSOfetwNkV0knn09d98myh80tF5PmblgBQ,4113
-graphstorm/run/gsgnn_ep/ep_infer_lm.py,sha256=fqoANYa99S0xPpSadRq__1vhp0pTO8ripDkvFCHN4Zk,3950
-graphstorm/run/gsgnn_ep/gsgnn_ep.py,sha256=1y7_8e5BmJJMqjc3oL0z4pFfiLcUm6uXXukW5zCdOf0,8075
-graphstorm/run/gsgnn_ep/gsgnn_lm_ep.py,sha256=-gjFzTrOFrEoo7UA40K7rkxQAUnqebDIySsBA4htxVU,7126
+graphstorm/run/gsgnn_ep/ep_infer_gnn.py,sha256=D7XoCQ-eMlz9GYpgqW2DVWDsEa4bgYrnnGJjHo6X8os,4631
+graphstorm/run/gsgnn_ep/ep_infer_lm.py,sha256=3Xfc6UjSAUyK-qqHRmGTxfj9Qnbgb_UEhhStZ6CB1xI,3990
+graphstorm/run/gsgnn_ep/gsgnn_ep.py,sha256=A4ct9dFaWFTi0LnKWRSU0ZyBPeg_TFPjZ6E3DPNfttI,8118
+graphstorm/run/gsgnn_ep/gsgnn_lm_ep.py,sha256=NZXA4T8jEoFWp1EZ9hFiC5kz1sap7xFKyWosZtk9TNM,7135
 graphstorm/run/gsgnn_lp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-graphstorm/run/gsgnn_lp/gsgnn_lm_lp.py,sha256=r7cjfpyiOg0s14FNTdkrkrjoO2VC2uMrDlkDCP5kta0,8422
-graphstorm/run/gsgnn_lp/gsgnn_lp.py,sha256=GI--HUipqkCVW22YrZeAk7nB_0WhFB2D0XG8WTGo5j4,8770
-graphstorm/run/gsgnn_lp/lp_infer_gnn.py,sha256=DvfCP4e82AI527nnsNOabgFZ08Zxat_1PAaMn66qgrI,3853
-graphstorm/run/gsgnn_lp/lp_infer_lm.py,sha256=MOVj7Qba9bzk8s73fuNJDkjgPGPMFlLj0N-ho3sHBow,3833
+graphstorm/run/gsgnn_lp/gsgnn_lm_lp.py,sha256=0DAJIIxYZiJNPGnCIhxzXOzBEU55U1Jsmh6PhsRGKjg,8610
+graphstorm/run/gsgnn_lp/gsgnn_lp.py,sha256=M5aA6F5l7n5hdZa35THkxRqTqQMkdEh_dwnQRF7Qdb4,10098
+graphstorm/run/gsgnn_lp/lp_infer_gnn.py,sha256=lFP3AYmXdxxRwcxhQUxSzHAQxxd2q1rP3ySGvXdxSOM,4157
+graphstorm/run/gsgnn_lp/lp_infer_lm.py,sha256=4ANRwXs7jSzcmIdckhhIIZP3o8UQkkCmB9Gdq69zdTk,4025
 graphstorm/run/gsgnn_np/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-graphstorm/run/gsgnn_np/gsgnn_np.py,sha256=zdByj4zMazlD62wU4hbrZk_FS-PyJNx419nLJtOCJnI,7002
-graphstorm/run/gsgnn_np/np_infer_gnn.py,sha256=auMoaTB9a2PNhB3y7XDtjvkI8tdBr_XX9A32rtgpKQ4,3781
+graphstorm/run/gsgnn_np/gsgnn_np.py,sha256=iZG1Ums8lth0Jqjt01mfM6EV6Ax5WZMbTh5dUHG2Mi4,7293
+graphstorm/run/gsgnn_np/np_infer_gnn.py,sha256=JnziE4m_lIJnx3Pz_KDSfwQ-DppwpcLtU5weUbmMb-E,4299
 graphstorm/sagemaker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-graphstorm/sagemaker/sagemaker_infer.py,sha256=wF1ChuXFyJsPZV1tYMGuubGUQbimyak9yftgN7fLrdg,10664
-graphstorm/sagemaker/sagemaker_train.py,sha256=etCvqxDhO1C76eK-gHY4lIxLSZ0pdxOJWeO-E0ThS1I,9046
-graphstorm/sagemaker/utils.py,sha256=S-dIpae2vrbajOhCM7HwotXU11lxIXduJ81BCM6y9GI,10422
+graphstorm/sagemaker/partition_algorithm.py,sha256=cibePOSVwSRkgTgMnF0-WL4dNogkFlnOMYdJ7-g66cM,9144
+graphstorm/sagemaker/s3_utils.py,sha256=xmV0xcutJte38uwa6CoVlFYsx2x8kUnkpQBqZ4SMT-E,1939
+graphstorm/sagemaker/sagemaker_infer.py,sha256=TjOdaC3FkgIa3ZvKoSOmEGDLM2QDL1_bQflb7nUriQg,10790
+graphstorm/sagemaker/sagemaker_partition.py,sha256=iyvbPlbMdF9c_6dvH5xa8_k0Qda78FAWVtAux3KqV0E,14911
+graphstorm/sagemaker/sagemaker_train.py,sha256=gjgWkup-pTtYCZ2U3qKnagEC-fZuyVGhtEZaAOSAVbg,9127
+graphstorm/sagemaker/utils.py,sha256=IMyt7sISNOIrOXtKYz3-kTWYu3y1r5Q8H9HN8NEvPK8,12568
 graphstorm/tracker/__init__.py,sha256=k-0FMxtaTdZCCOGDhfl0nDfxKQR-NCRjw2qA5GlI-zc,1306
 graphstorm/tracker/graphstorm_tracker.py,sha256=IG1uxnPZ_zGSFSjTZ59Q7jmhB4QOlr1myCPu6MQOSNk,4370
-graphstorm/tracker/sagemaker_tracker.py,sha256=0D8fVye0uhO0uk5RAUyYKLSm2ELBsZLXlts0PWfM4gY,10002
-graphstorm/trainer/__init__.py,sha256=AN0HzpYd6X5Hzzta-tL2cAHKZa7Gp1_mcSWoZzj0710,817
-graphstorm/trainer/ep_trainer.py,sha256=BMXI9Sxsx-c3Tc3DhDIL1p2M4kLnNOSiy839rUsaLc8,13648
-graphstorm/trainer/gsgnn_trainer.py,sha256=54Vro-AGOXb4Z113jID7NsJcKblhE1xoQL3xKUlzWHM,13436
-graphstorm/trainer/lp_trainer.py,sha256=mu9CrE_GAIwH7BXscH5OupWpM56D8iMK8TpRtuiHuUA,12971
-graphstorm/trainer/np_trainer.py,sha256=s0_RahtuUu6Ls_imi1TOx-VDXugHuBgHfLcMWsQ9of8,13000
-graphstorm-0.1.1rc2.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
-graphstorm-0.1.1rc2.dist-info/METADATA,sha256=AMASzIGZ06s2wHsWmhY9RVsxr6gzEuaJXlZEkiZ8yI0,208
-graphstorm-0.1.1rc2.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
-graphstorm-0.1.1rc2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-graphstorm-0.1.1rc2.dist-info/top_level.txt,sha256=a-DZLjGSac-h49SLtJLk0pWec2S7qs9S_CoFa8y8JXg,11
-graphstorm-0.1.1rc2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-graphstorm-0.1.1rc2.dist-info/RECORD,,
+graphstorm/tracker/sagemaker_tracker.py,sha256=3iYwTGeEUobwuFtKPfY6MatdQVrae6DsxorzOIawX2E,10152
+graphstorm/trainer/__init__.py,sha256=9WAcs_PAPbtgYzOqOcXM4XBRCvDBTJyZxR-NAFzb-pM,872
+graphstorm/trainer/ep_trainer.py,sha256=AntrZ06SIAManDlKAvpz0Y9C5HQoEi2L22LQfCSC94U,14072
+graphstorm/trainer/glem_np_trainer.py,sha256=tUOZhT9ljG8M1zZ3gegZyqsfr913d1RNxXdRPIBwI9w,10396
+graphstorm/trainer/gsgnn_trainer.py,sha256=8QOUchcy1PGK2tsMtgzBB-1aSTRuMxuzXqNN0smhdWA,13255
+graphstorm/trainer/lp_trainer.py,sha256=8SbY51LWCDVzuZHTTnLlmTrJsSHFzCKMEIjQJQwa1Tw,13092
+graphstorm/trainer/np_trainer.py,sha256=fy2rZX4duDpKfIih8oshex-04yHBPICGI6IgBG-ByRI,13422
+graphstorm-0.1.2.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
+graphstorm-0.1.2.dist-info/METADATA,sha256=rWuudPTwo6A3hXLvmCQXniVD1EiDkOiLXDtpZ6FoyoQ,384
+graphstorm-0.1.2.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
+graphstorm-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+graphstorm-0.1.2.dist-info/top_level.txt,sha256=a-DZLjGSac-h49SLtJLk0pWec2S7qs9S_CoFa8y8JXg,11
+graphstorm-0.1.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+graphstorm-0.1.2.dist-info/RECORD,,
```

