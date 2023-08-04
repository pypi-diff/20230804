# Comparing `tmp/alpaca_farm-0.1.8.tar.gz` & `tmp/alpaca_farm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.8.tar", last modified: Sun Jul  9 01:33:12 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.9.tar", last modified: Fri Aug  4 10:37:44 2023, max compression
```

## Comparing `alpaca_farm-0.1.8.tar` & `alpaca_farm-0.1.9.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.178722 alpaca_farm-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:33:12.178722 alpaca_farm-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-09 01:33:00.000000 alpaca_farm-0.1.8/src/alpaca_farm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/models/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_flash_llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_flash_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.452797 alpaca_farm-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-08-04 10:37:21.000000 alpaca_farm-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 10:37:21.000000 alpaca_farm-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-08-04 10:37:44.452797 alpaca_farm-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-08-04 10:37:21.000000 alpaca_farm-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:37:44.452797 alpaca_farm-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.440797 alpaca_farm-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.440797 alpaca_farm-0.1.9/src/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-04 10:37:33.000000 alpaca_farm-0.1.9/src/alpaca_farm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.444797 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.440797 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/src/alpaca_farm/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/quark_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/quark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/src/alpaca_farm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.444797 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-08-04 10:37:44.000000 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-04 10:37:44.000000 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:37:44.000000 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 10:37:44.000000 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 10:37:44.000000 alpaca_farm-0.1.9/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:37:44.448797 alpaca_farm-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/tests/test_auto_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/tests/test_flash_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/tests/test_flash_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/tests/test_torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-04 10:37:22.000000 alpaca_farm-0.1.9/tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.8/LICENSE` & `alpaca_farm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/PKG-INFO` & `alpaca_farm-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `alpaca_farm-0.1.8/README.md` & `alpaca_farm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/setup.py` & `alpaca_farm-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.1.8'
+from .eval import PairwiseAutoAnnotator, alpaca_leaderboard
```

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.9/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/flash_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .eval import PairwiseAutoAnnotator, alpaca_leaderboard
```

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/eval.py` & `alpaca_farm-0.1.9/src/alpaca_farm/auto_annotations/eval.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 from pathlib import Path
 from typing import Any, Optional, Sequence, Union
 
 import alpaca_eval.annotators as eval_annotators
 import alpaca_eval.utils as eval_utils
 import datasets
 import pandas as pd
+
+import alpaca_eval.annotators as eval_annotators
+import alpaca_eval.processors as eval_processors
 from alpaca_eval import metrics
 
 from .. import constants
 
 __all__ = ["alpaca_leaderboard", "PairwiseAutoAnnotator"]
 
 CURRENT_DIR = Path(__file__).parent
 ANNOTATORS_CONFIG_DIR = CURRENT_DIR / "annotators"
+DUMMY_EXAMPLE_NOINPUT = dict(instruction="Solve: 1+1=", output_1="2", output_2="3")
+DUMMY_EXAMPLE_INPUT = dict(instruction="Solve:", output_1="2", input="1+1=", output_2="3")
 
 
 PRECOMPUTED_LEADERBOARD = {
     "annotator_pool_v0/configs.yaml": {
         # Internal codename: rlhf_llama_7b_regen_v7_3ep_v12_ckpt_20
         "RLHF PPO": {
             "n_draws": 9.0,
@@ -173,33 +178,75 @@
 
     @property
     def SingleAnnotator(self):
         return SinglePairwiseAutoAnnotator
 
 
 class SinglePairwiseAutoAnnotator(eval_annotators.SinglePairwiseAnnotator):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        for i, processor in enumerate(self.processors):
+            # you need to use a batch padder that separates inputs and no inputs
+            if isinstance(processor, eval_processors.PaddingForBatchesProcessor):
+                self.processors[i] = PaddingForBatchesProcessorInputNoinput(
+                    batch_size=self.batch_size,
+                    padding_example_input=DUMMY_EXAMPLE_INPUT,
+                    padding_example_noinput=DUMMY_EXAMPLE_NOINPUT,
+                )
+
     def _get_prompt_template(self, prompt_template: dict[str, str]):
         # prompt_template will now be a dictionary of prompt templates of len 2 (one with and one without input)
         _get_prompt_template = super()._get_prompt_template
         return {k: _get_prompt_template(prompt) for k, prompt in prompt_template.items()}
 
-    def make_prompts(self, df_to_annotate, prompt_template=None):
+    def _make_prompts(self, df_to_annotate, prompt_template=None):
         if prompt_template is None:
             prompt_template = self.prompt_template
 
         arr_is_inputs = (df_to_annotate["input"] != "") & (df_to_annotate["input"].notnull())
         df_with_inputs = df_to_annotate[arr_is_inputs]
         df_without_inputs = df_to_annotate[~arr_is_inputs]
 
-        prompts, df = super().make_prompts(
+        prompts, df = super()._make_prompts(
             df_without_inputs,
             prompt_template=prompt_template["without_inputs"],
         )
         if arr_is_inputs.any():
-            prompts_i, df_i = super().make_prompts(
+            prompts_i, df_i = super()._make_prompts(
                 df_with_inputs,
                 prompt_template=prompt_template["with_inputs"],
             )
             prompts += prompts_i
             df = pd.concat([df, df_i], axis=0, ignore_index=True)
 
         return prompts, df
+
+
+class PaddingForBatchesProcessorInputNoinput(eval_processors.BaseProcessor):
+    def __init__(self, batch_size, padding_example_input: dict, padding_example_noinput: dict, **kwargs):
+        self.padded_noinput = eval_processors.PaddingForBatchesProcessor(
+            batch_size=batch_size, padding_example=padding_example_noinput, **kwargs
+        )
+        self.padded_input = eval_processors.PaddingForBatchesProcessor(
+            batch_size=batch_size, padding_example=padding_example_input, **kwargs
+        )
+        super().__init__(**kwargs)
+
+    def preprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
+        arr_is_inputs = (df_to_annotate["input"] != "") & (df_to_annotate["input"].notnull())
+        if arr_is_inputs.any():
+            # need to padd separately with and without inputs
+            padded_df_without_inputs = self.padded_noinput.preprocess(df_to_annotate[~arr_is_inputs].copy())
+            padded_df_with_inputs = self.padded_input.preprocess(df_to_annotate[arr_is_inputs].copy())
+
+            df_out = pd.concat([padded_df_without_inputs, padded_df_with_inputs], axis=0, ignore_index=True)
+        else:
+            df_out = self.padded_noinput.preprocess(df_to_annotate)
+
+        df_out["is_padding"] = df_out["is_padding"].astype(bool)
+
+        return df_out
+
+    def postprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
+        # independent of inputs
+        return self.padded_noinput.postprocess(df_to_annotate)
```

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/common.py` & `alpaca_farm-0.1.9/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.9/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.9/src/alpaca_farm/data_postprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.9/src/alpaca_farm/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.9/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.9/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.9/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.9/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.9/src/alpaca_farm/inference/decode.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.9/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.9/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.9/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.9/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/openai_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.9/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.9/src/alpaca_farm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = '0.1.9'
```

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_trainer.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/quark_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/quark_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.9/src/alpaca_farm/rl/rl_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.9/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/types.py` & `alpaca_farm-0.1.9/src/alpaca_farm/types.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.9/src/alpaca_farm/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.9/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-farm
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `alpaca_farm-0.1.8/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.9/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,11 +68,12 @@
 src/alpaca_farm/rl/__init__.py
 src/alpaca_farm/rl/kl_controller.py
 src/alpaca_farm/rl/ppo_trainer.py
 src/alpaca_farm/rl/ppo_utils.py
 src/alpaca_farm/rl/quark_trainer.py
 src/alpaca_farm/rl/quark_utils.py
 src/alpaca_farm/rl/rl_trainer.py
+tests/test_auto_eval.py
 tests/test_flash_llama.py
 tests/test_flash_opt.py
 tests/test_torch_ops.py
 tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.8/tests/test_flash_llama.py` & `alpaca_farm-0.1.9/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/tests/test_flash_opt.py` & `alpaca_farm-0.1.9/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/tests/test_torch_ops.py` & `alpaca_farm-0.1.9/tests/test_torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.8/tests/test_utils.py` & `alpaca_farm-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

