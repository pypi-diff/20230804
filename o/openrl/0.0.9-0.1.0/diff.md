# Comparing `tmp/openrl-0.0.9.tar.gz` & `tmp/openrl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.9.tar", last modified: Mon May  8 11:19:00 2023, max compression
+gzip compressed data, was "openrl-0.1.0.tar", last modified: Fri Aug  4 07:18:47 2023, max compression
```

## Comparing `openrl-0.0.9.tar` & `openrl-0.1.0.tar`

### file list

```diff
@@ -1,175 +1,295 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.192651 openrl-0.0.9/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.0.9/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.9/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)    13540 2023-05-08 11:19:00.192202 openrl-0.0.9/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)    12391 2023-05-08 11:10:58.000000 openrl-0.0.9/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.143714 openrl-0.0.9/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      425 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.146210 openrl-0.0.9/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2916 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    16410 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.147665 openrl-0.0.9/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54804 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.149771 openrl-0.0.9/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.151417 openrl-0.0.9/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.152020 openrl-0.0.9/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    31231 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.154729 openrl-0.0.9/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9929 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      841 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.155191 openrl-0.0.9/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)       79 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.156324 openrl-0.0.9/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1621 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/common/build_envs.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3305 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.156937 openrl-0.0.9/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1425 2023-04-28 09:05:04.000000 openrl-0.0.9/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.160596 openrl-0.0.9/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11650 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.161044 openrl-0.0.9/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4405 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.161788 openrl-0.0.9/openrl/envs/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/nlp/daily_dialog_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      347 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/nlp_env.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.163348 openrl-0.0.9/openrl/envs/nlp/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/custom_text_generation_pools.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/distribution.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/evaluation_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.163853 openrl-0.0.9/openrl/envs/nlp/utils/metrics/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/metrics/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/metrics/meteor.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/observation.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/sampler.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/nlp/utils/text_generation_pool.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.165249 openrl-0.0.9/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      348 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30978 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8061 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.167122 openrl-0.0.9/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6518 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.169258 openrl-0.0.9/openrl/envs/vec_env/vec_info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1058 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/base_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/nlp_vec_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1221 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/envs/vec_env/vec_info/simple_vec_info.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.170356 openrl-0.0.9/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9266 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2227 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/reward_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.172264 openrl-0.0.9/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1612 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2454 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.174284 openrl-0.0.9/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.175409 openrl-0.0.9/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       57 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3456 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.176931 openrl-0.0.9/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6445 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/policy_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3991 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/modules/networks/policy_value_network_gpt.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.180223 openrl-0.0.9/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7389 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2270 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3551 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10432 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/mlp.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.181617 openrl-0.0.9/openrl/modules/networks/utils/nlp/
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11814 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/base_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/causal_policy.py
--rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-04-28 09:05:05.000000 openrl-0.0.9/openrl/modules/networks/utils/nlp/hf_generation_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3344 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7053 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5206 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.183328 openrl-0.0.9/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.185098 openrl-0.0.9/openrl/rewards/
--rw-r--r--   0 4paradigm   (501) staff       (20)      919 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/rewards/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      570 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/rewards/base_reward.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-04-28 09:44:16.000000 openrl-0.0.9/openrl/rewards/nlp_reward.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.185717 openrl-0.0.9/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/runners/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.187769 openrl-0.0.9/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      188 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1263 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4024 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/runners/common/chat_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2849 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/runners/common/ppo_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4596 2023-05-08 11:10:58.000000 openrl-0.0.9/openrl/runners/common/rl_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.188247 openrl-0.0.9/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.188575 openrl-0.0.9/openrl/supports/opendata/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.189206 openrl-0.0.9/openrl/supports/opendata/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opendata/utils/opendata_utils.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.190217 openrl-0.0.9/openrl/supports/opengpu/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/supports/opengpu/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-05-04 10:32:54.000000 openrl-0.0.9/openrl/supports/opengpu/gpu_info.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7114 2023-05-06 12:04:43.000000 openrl-0.0.9/openrl/supports/opengpu/manager.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191038 openrl-0.0.9/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5744 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1482 2023-04-28 07:15:42.000000 openrl-0.0.9/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.145386 openrl-0.0.9/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)    13540 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     4588 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      278 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-05-08 11:19:00.000000 openrl-0.0.9/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-05-08 11:19:00.192706 openrl-0.0.9/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     3149 2023-05-06 12:04:43.000000 openrl-0.0.9/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191221 openrl-0.0.9/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191581 openrl-0.0.9/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-05-08 11:19:00.191945 openrl-0.0.9/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.0.9/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.552238 openrl-0.1.0/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-28 07:15:42.000000 openrl-0.1.0/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17236 2023-08-04 07:18:47.551976 openrl-0.1.0/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)    15936 2023-08-04 07:14:34.000000 openrl-0.1.0/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.502486 openrl-0.1.0/examples/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-31 08:18:26.000000 openrl-0.1.0/examples/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.502858 openrl-0.1.0/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      440 2023-08-04 05:59:14.000000 openrl-0.1.0/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.506094 openrl-0.1.0/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3004 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8900 2023-07-26 07:53:23.000000 openrl-0.1.0/openrl/algorithms/behavior_cloning.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9878 2023-07-30 11:39:30.000000 openrl-0.1.0/openrl/algorithms/ddpg.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6998 2023-07-30 12:05:59.000000 openrl-0.1.0/openrl/algorithms/dqn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1945 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/algorithms/gail.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1238 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/algorithms/mat.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    15795 2023-07-26 07:53:23.000000 openrl-0.1.0/openrl/algorithms/ppo.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11948 2023-07-30 11:21:22.000000 openrl-0.1.0/openrl/algorithms/sac.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8504 2023-07-30 11:57:29.000000 openrl-0.1.0/openrl/algorithms/vdn.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.507075 openrl-0.1.0/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      807 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2009 2023-07-28 13:25:40.000000 openrl-0.1.0/openrl/buffers/offpolicy_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14892 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/buffers/offpolicy_replay_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54484 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.508155 openrl-0.1.0/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1938 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3240 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.508639 openrl-0.1.0/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2551 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1579 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.509334 openrl-0.1.0/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    34138 2023-08-03 13:56:29.000000 openrl-0.1.0/openrl/configs/config.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3577 2023-08-03 13:56:28.000000 openrl-0.1.0/openrl/configs/utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.509671 openrl-0.1.0/openrl/datasets/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/datasets/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4537 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/datasets/expert_dataset.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.510752 openrl-0.1.0/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      238 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1294 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/drivers/offline_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8805 2023-07-30 12:05:04.000000 openrl-0.1.0/openrl/drivers/offpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9176 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5837 2023-07-28 07:22:45.000000 openrl-0.1.0/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.511004 openrl-0.1.0/openrl/envs/
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.511241 openrl-0.1.0/openrl/envs/PettingZoo/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1763 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/PettingZoo/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      591 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.511943 openrl-0.1.0/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      739 2023-07-05 11:01:20.000000 openrl-0.1.0/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2439 2023-08-03 13:56:28.000000 openrl-0.1.0/openrl/envs/common/build_envs.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5610 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.512831 openrl-0.1.0/openrl/envs/connect_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1764 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/connect_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3785 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/connect_env/base_connect_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      430 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/connect_env/connect3_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      430 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/connect_env/connect4_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2254 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/connect_env/utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.513183 openrl-0.1.0/openrl/envs/gridworld/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1333 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/gridworld/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3425 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/gridworld/gridworld_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.513318 openrl-0.1.0/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1492 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.514610 openrl-0.1.0/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      628 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      615 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11659 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      343 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.514925 openrl-0.1.0/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      145 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4433 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.515550 openrl-0.1.0/openrl/envs/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7514 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/nlp/daily_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3272 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/nlp/fake_dialog_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      462 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/nlp/nlp_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.516647 openrl-0.1.0/openrl/envs/nlp/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2765 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/nlp/utils/custom_text_generation_pools.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4515 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/distribution.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1823 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/evaluation_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.516953 openrl-0.1.0/openrl/envs/nlp/utils/metrics/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/metrics/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7088 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/nlp/utils/metrics/meteor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7201 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/observation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1363 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/nlp/utils/sampler.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-07-14 12:12:55.000000 openrl-0.1.0/openrl/envs/nlp/utils/text_generation_pool.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.517251 openrl-0.1.0/openrl/envs/offline/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1596 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/offline/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3053 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/offline/offline_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.517623 openrl-0.1.0/openrl/envs/super_mario/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1477 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/super_mario/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2494 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/super_mario/super_mario_convert.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.518720 openrl-0.1.0/openrl/envs/toy_envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2370 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/toy_envs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8028 2023-07-27 11:24:00.000000 openrl-0.1.0/openrl/envs/toy_envs/bit_flipping_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8864 2023-07-30 11:52:07.000000 openrl-0.1.0/openrl/envs/toy_envs/identity_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6306 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/toy_envs/multi_input_envs.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.519857 openrl-0.1.0/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1377 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    33689 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11888 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    12047 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.520723 openrl-0.1.0/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7611 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7902 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2933 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.521714 openrl-0.1.0/openrl/envs/vec_env/vec_info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1270 2023-08-04 07:09:50.000000 openrl-0.1.0/openrl/envs/vec_env/vec_info/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      585 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/vec_info/base_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1927 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/vec_info/episode_rewards_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2323 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/vec_info/nlp_vec_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1237 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/vec_info/simple_vec_info.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.523107 openrl-0.1.0/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9652 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10459 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/gen_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2274 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/reward_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1544 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      883 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/vec_env/wrappers/zero_reward_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.524882 openrl-0.1.0/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      553 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5196 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/wrappers/atari_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3665 2023-08-02 08:46:16.000000 openrl-0.1.0/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6649 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3325 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/envs/wrappers/flatten.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1486 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/wrappers/image_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1796 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/wrappers/mat_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3561 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/wrappers/monitor.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2269 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.527103 openrl-0.1.0/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/base_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4330 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/bc_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.528887 openrl-0.1.0/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      399 2023-07-26 07:34:36.000000 openrl-0.1.0/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1364 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/common/bc_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3162 2023-07-28 13:58:47.000000 openrl-0.1.0/openrl/modules/common/ddpg_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3462 2023-07-30 12:06:55.000000 openrl-0.1.0/openrl/modules/common/dqn_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1662 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/common/gail_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1337 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/common/mat_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3713 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3349 2023-07-27 11:08:54.000000 openrl-0.1.0/openrl/modules/common/sac_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3539 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/common/vdn_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5743 2023-07-30 11:40:00.000000 openrl-0.1.0/openrl/modules/ddpg_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4333 2023-07-30 11:49:45.000000 openrl-0.1.0/openrl/modules/dqn_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2002 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/gail_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1210 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.531094 openrl-0.1.0/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    16147 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/MAT_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1191 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1944 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/base_value_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11066 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/ddpg_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7064 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/gail_discriminator.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8050 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6032 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/policy_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4006 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/policy_value_network_gpt.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3960 2023-07-27 09:57:50.000000 openrl-0.1.0/openrl/modules/networks/q_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5080 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/sac_network.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.533561 openrl-0.1.0/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7359 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9343 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2850 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      805 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3536 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10540 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5904 2023-07-28 15:51:43.000000 openrl-0.1.0/openrl/modules/networks/utils/mlp.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.534173 openrl-0.1.0/openrl/modules/networks/utils/nlp/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/nlp/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11772 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/nlp/base_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10986 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/utils/nlp/causal_policy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)   188639 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/utils/nlp/hf_generation_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3973 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3515 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2074 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/running_mean_std.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3314 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      317 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      217 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/utils/vdn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4627 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7336 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/modules/networks/vdn_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7258 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5004 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/rl_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7405 2023-07-30 11:40:31.000000 openrl-0.1.0/openrl/modules/sac_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.535652 openrl-0.1.0/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      631 2023-07-26 07:53:23.000000 openrl-0.1.0/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3599 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/modules/utils/valuenorm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4331 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/modules/vdn_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.536587 openrl-0.1.0/openrl/rewards/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1095 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/rewards/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      641 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/rewards/base_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1667 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/rewards/gail_reward.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3467 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/rewards/nlp_reward.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.536779 openrl-0.1.0/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.539521 openrl-0.1.0/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      674 2023-07-26 07:34:36.000000 openrl-0.1.0/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1684 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2308 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/runners/common/bc_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4024 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/runners/common/chat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4099 2023-07-28 13:58:03.000000 openrl-0.1.0/openrl/runners/common/ddpg_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4143 2023-07-30 12:10:42.000000 openrl-0.1.0/openrl/runners/common/dqn_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2044 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/runners/common/gail_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1616 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/runners/common/mat_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4914 2023-07-27 10:02:16.000000 openrl-0.1.0/openrl/runners/common/ppo_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7172 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/runners/common/rl_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4441 2023-07-27 11:12:48.000000 openrl-0.1.0/openrl/runners/common/sac_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4088 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/runners/common/vdn_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.539847 openrl-0.1.0/openrl/selfplay/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/selfplay/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.540720 openrl-0.1.0/openrl/selfplay/callbacks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-08-01 07:02:46.000000 openrl-0.1.0/openrl/selfplay/callbacks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      751 2023-08-01 09:20:25.000000 openrl-0.1.0/openrl/selfplay/callbacks/base_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2488 2023-08-04 06:55:00.000000 openrl-0.1.0/openrl/selfplay/callbacks/selfplay_api.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5563 2023-08-03 13:56:29.000000 openrl-0.1.0/openrl/selfplay/callbacks/selfplay_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/selfplay/multiplayer_env.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.542401 openrl-0.1.0/openrl/selfplay/opponents/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-08-02 09:49:08.000000 openrl-0.1.0/openrl/selfplay/opponents/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2011 2023-08-03 13:56:29.000000 openrl-0.1.0/openrl/selfplay/opponents/base_opponent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1962 2023-08-03 13:56:29.000000 openrl-0.1.0/openrl/selfplay/opponents/network_opponent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2493 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/opponents/opponent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2544 2023-08-03 13:56:29.000000 openrl-0.1.0/openrl/selfplay/opponents/opponent_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4035 2023-08-03 14:21:50.000000 openrl-0.1.0/openrl/selfplay/opponents/utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.543448 openrl-0.1.0/openrl/selfplay/sample_strategy/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1177 2023-08-04 07:02:08.000000 openrl-0.1.0/openrl/selfplay/sample_strategy/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      850 2023-08-04 06:42:33.000000 openrl-0.1.0/openrl/selfplay/sample_strategy/base_sample_strategy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      859 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/sample_strategy/last_opponent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      884 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/sample_strategy/random_opponent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.544401 openrl-0.1.0/openrl/selfplay/selfplay_api/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-08-01 10:49:12.000000 openrl-0.1.0/openrl/selfplay/selfplay_api/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2056 2023-08-04 06:31:05.000000 openrl-0.1.0/openrl/selfplay/selfplay_api/base_api.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2874 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/selfplay_api/selfplay_api.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2517 2023-08-04 06:53:46.000000 openrl-0.1.0/openrl/selfplay/selfplay_api/selfplay_client.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.545143 openrl-0.1.0/openrl/selfplay/strategies/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1508 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/strategies/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      885 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/selfplay/strategies/base_strategy.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    15330 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/selfplay/strategies/strategies.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.546220 openrl-0.1.0/openrl/selfplay/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/selfplay/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5003 2023-08-03 13:50:46.000000 openrl-0.1.0/openrl/selfplay/wrappers/base_multiplayer_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1076 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/wrappers/human_opponent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3129 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/wrappers/opponent_pool_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1194 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/selfplay/wrappers/random_opponent_wrapper.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.546656 openrl-0.1.0/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.546918 openrl-0.1.0/openrl/supports/opendata/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/supports/opendata/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.547402 openrl-0.1.0/openrl/supports/opendata/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/supports/opendata/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2132 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/supports/opendata/utils/opendata_utils.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.548358 openrl-0.1.0/openrl/supports/opengpu/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/supports/opengpu/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4184 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/supports/opengpu/gpu_info.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7114 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/supports/opengpu/manager.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.549889 openrl-0.1.0/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-28 07:15:42.000000 openrl-0.1.0/openrl/utils/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.551435 openrl-0.1.0/openrl/utils/callbacks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      740 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9559 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/callbacks.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2613 2023-08-04 07:09:51.000000 openrl-0.1.0/openrl/utils/callbacks/callbacks_factory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3774 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/checkpoint_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10942 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/eval_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2022 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/processbar_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5995 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/callbacks/stop_callback.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7132 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/evaluation.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1587 2023-08-03 13:56:30.000000 openrl-0.1.0/openrl/utils/file_tool.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6175 2023-08-03 11:12:17.000000 openrl-0.1.0/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1377 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/type_aliases.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1423 2023-07-21 13:01:50.000000 openrl-0.1.0/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.503701 openrl-0.1.0/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17236 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8562 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      422 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       16 2023-08-04 07:18:47.000000 openrl-0.1.0/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-08-04 07:18:47.552282 openrl-0.1.0/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3475 2023-08-04 03:49:26.000000 openrl-0.1.0/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.501749 openrl-0.1.0/tests/
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.551581 openrl-0.1.0/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      972 2023-04-28 07:15:42.000000 openrl-0.1.0/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-04 07:18:47.551728 openrl-0.1.0/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-28 07:15:42.000000 openrl-0.1.0/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.9/LICENSE` & `openrl-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/PKG-INFO` & `openrl-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,261 +1,297 @@
-Metadata-Version: 2.1
-Name: openrl
-Version: 0.0.9
-Summary: unified reinforcement learning framework
-Home-page: https://github.com/OpenRL-Lab/openrl
-Author: openrl contributors
-Author-email: huangsy1314@163.com
-Project-URL: Code, https://github.com/OpenRL-Lab/openrl
-Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
-Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: mpe
-Provides-Extra: nlp
-License-File: LICENSE
-License-File: LICENSE.txt
-
 <div align="center">
-    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
+    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
-[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/en/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.9 is updated on May 6, 2023 
+[![Embark](https://img.shields.io/badge/discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT)
+[![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg)
+
+OpenRL-v0.0.16 is updated on July 30, 2023
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
-## 欢迎来到OpenRL
+## Welcome to OpenRL
+
+[Documentation](https://openrl-docs.readthedocs.io/en/latest/) | [中文介绍](README_zh.md) |  [中文文档](https://openrl-docs.readthedocs.io/zh/latest/)
+
+<div align="center">
+    Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights Welcome.   <br><br>
+</div>
+
+OpenRL is an open-source general reinforcement learning research framework that supports training for various tasks 
+such as single-agent, multi-agent, offline RL, self-play, and natural language. 
+Developed based on PyTorch, the goal of OpenRL is to provide a simple-to-use, flexible, efficient and sustainable platform for the reinforcement learning research community.
+
+Currently, the features supported by OpenRL include:
+
+- A simple-to-use universal interface that supports training for both single-agent and multi-agent
+
+- Support for offline RL training with expert dataset
+
+- Support self-play training
+
+- Reinforcement learning training support for natural language tasks (such as dialogue)
+
+- Importing models and datasets from [Hugging Face](https://huggingface.co/)
+
+- Support for models such as LSTM, GRU, Transformer etc.
+
+- Multiple training acceleration methods including automatic mixed precision training and data collecting wth half precision policy network
+
+- User-defined training models, reward models, training data and environment support
+
+- Support for [gymnasium](https://gymnasium.farama.org/) environments
+
+- Support for [Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html), which can be used to implement various functions such as logging, saving, and early stopping
+
+- Dictionary observation space support
+
+- Popular visualization tools such as [wandb](https://wandb.ai/),  [tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html) are supported
+
+- Serial or parallel environment training while ensuring consistent results in both modes
 
-[English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
+- Chinese and English documentation
 
-OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
-目前，OpenRL支持的特性包括：
+- Provides unit testing and code coverage testing
 
-- 简单易用且支持单智能体、多智能体训练的通用接口
-- 支持自然语言任务（如对话任务）的强化学习训练
-- 支持从[Hugging Face](https://huggingface.co/)上导入模型和数据
-- 支持LSTM，GRU，Transformer等模型
-- 支持多种训练加速，例如：自动混合精度训练，半精度策略网络收集数据等
-- 支持用户自定义训练模型、奖励模型、训练数据以及环境
-- 支持[gymnasium](https://gymnasium.farama.org/)环境
-- 支持字典观测空间
-- 支持[wandb](https://wandb.ai/)，[tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html)等主流训练可视化工具
-- 支持环境的串行和并行训练，同时保证两种模式下的训练效果一致
-- 中英文文档
-- 提供单元测试和代码覆盖测试
-- 符合Black Code Style和类型检查
-
-该框架经过了[OpenRL-Lab](https://github.com/OpenRL-Lab)的多次迭代并应用于学术研究，目前已经成为了一个成熟的强化学习框架。
-OpenRL-Lab将持续维护和更新OpenRL，欢迎大家加入我们的[开源社区](./CONTRIBUTING.md)，一起为强化学习的发展做出贡献。
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
-
-## 目录
-
-- [欢迎来到OpenRL](#欢迎来到openrl)
-- [目录](#目录)
-- [安装](#安装)
-- [使用Docker](#使用docker)
-- [快速上手](#快速上手)
-- [Gallery](#Gallery)
-- [使用OpenRL的项目](#使用OpenRL的项目)
-- [反馈和贡献](#反馈和贡献)
-- [维护人员](#维护人员)
-- [支持者](#支持者)
-  - [&#8627; Contributors](#-contributors)  
+- Compliant with Black Code Style guidelines and type checking
+
+Algorithms currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Proximal Policy Optimization (PPO)](https://arxiv.org/abs/1707.06347)
+- [Dual-clip PPO](https://arxiv.org/abs/1912.09729)
+- [Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955)
+- [Joint-ratio Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515)
+- [Generative Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476)
+- [Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf)
+- Self-Play
+- [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602)
+- [Multi-Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953)
+- [Value-Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296)
+- [Soft Actor Critic (SAC)](https://arxiv.org/abs/1812.05905)
+- [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/abs/1509.02971)
+
+Environments currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Gymnasium](https://gymnasium.farama.org/)
+- [MuJoCo](https://github.com/deepmind/mujoco)
+- [PettingZoo](https://pettingzoo.farama.org/)
+- [MPE](https://github.com/openai/multiagent-particle-envs)
+- [Chat Bot](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
+- [Atari](https://gymnasium.farama.org/environments/atari/)
+- [StarCraft II](https://github.com/oxwhirl/smac)
+- [Omniverse Isaac Gym](https://github.com/NVIDIA-Omniverse/OmniIsaacGymEnvs)
+- [GridWorld](./examples/gridworld/)
+- [Super Mario Bros](https://github.com/Kautenja/gym-super-mario-bros)
+- [Gym Retro](https://github.com/openai/retro)
+
+This framework has undergone multiple iterations by the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in academic research. 
+It has now become a mature reinforcement learning framework.
+
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone to join our [open-source community](./CONTRIBUTING.md) 
+to contribute towards the development of reinforcement learning.
+
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
+
+## Outline
+
+- [Welcome to OpenRL](#welcome-to-openrl)
+- [Outline](#outline)
+- [Installation](#installation)
+- [Use Docker](#use-docker)
+- [Quick Start](#quick-start)
+- [Gallery](#gallery)
+- [Projects Using OpenRL](#projects-using-openrl)
+- [Feedback and Contribution](#feedback-and-contribution)
+- [Maintainers](#maintainers)
+- [Supporters](#supporters)
+  - [&#8627; Contributors](#-contributors) 
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
-## 安装
+## Installation
+
+Users can directly install OpenRL via pip:
 
-用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
 
-如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
+If users are using Anaconda or Miniconda, they can also install OpenRL via conda:
+
 ```bash
 conda install -c openrl openrl
 ```
 
-想要修改源码的用户也可以从源码安装OpenRL:
+Users who want to modify the source code can also install OpenRL from the source code:
+
 ```bash
 git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
-安装完成后，用户可以直接通过命令行查看OpenRL的版本：
+After installation, users can check the version of OpenRL through command line:
+
 ```bash
 openrl --version
 ```
 
-**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-
-## 使用Docker
+**Tips**: No installation required, try OpenRL online through Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
 
-OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
-如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+## Use Docker
 
+OpenRL currently provides Docker images with and without GPU support. 
+If the user's computer does not have an NVIDIA GPU, they can obtain an image without the GPU plugin using the following command:
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
-如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+If the user wants to accelerate training with a GPU, they can obtain it using the following command:
 ```bash
 sudo docker pull openrllab/openrl
 ```
 
-镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+After successfully pulling the image, users can run OpenRL's Docker image using the following commands:
 ```bash
-# 不带显卡加速
+# Without GPU acceleration
 sudo docker run -it openrllab/openrl-cpu
-# 带显卡加速
+# With GPU acceleration 
 sudo docker run -it --gpus all --net host openrllab/openrl
 ```
 
-进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
-```bash
-# 查看Docker镜像中OpenRL的版本
-openrl --version
-# 运行测例
-openrl --mode train --env CartPole-v1
+Once inside the Docker container, users can check OpenRL's version and then run test cases using these commands: 
+```bash 
+# Check OpenRL version in Docker container  
+openrl --version  
+# Run test case  
+openrl --mode train --env CartPole-v1  
 ```
 
+## Quick Start
 
-## 快速上手
-
-OpenRL为强化学习入门用户提供了简单易用的接口，
-下面是一个使用PPO算法训练`CartPole`环境的例子：
+OpenRL provides a simple and easy-to-use interface for beginners in reinforcement learning. 
+Below is an example of using the PPO algorithm to train the `CartPole` environment:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-env = make("CartPole-v1", env_num=9) # 创建环境，并设置环境并行数为9
-net = Net(env) # 创建神经网络
-agent = Agent(net) # 初始化智能体
-agent.train(total_time_steps=20000) # 开始训练，并设置环境运行总步数为20000
+env = make("CartPole-v1", env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network.
+agent = Agent(net) # Initialize the agent.
+agent.train(total_time_steps=20000) # Start training and set the total number of steps to 20,000 for the running environment.
 ```
-使用OpenRL训练智能体只需要简单的四步：**创建环境**=>**初始化模型**=>**初始化智能体**=>**开始训练**！
+Training an agent using OpenRL only requires four simple steps: 
+**Create Environment** => **Initialize Model** => **Initialize Agent** => **Start Training**!
 
-对于训练好的智能体，用户也可以方便地进行智能体的测试:
+For a well-trained agent, users can also easily test the agent:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-agent = Agent(Net(make("CartPole-v1", env_num=9))) # 初始化训练器
+agent = Agent(Net(make("CartPole-v1", env_num=9))) # Initialize trainer.
 agent.train(total_time_steps=20000)
-# 创建用于测试的环境，并设置环境并行数为9，设置渲染模式为group_human
+# Create an environment for test, set the parallelism of the environment to 9, and set the rendering mode to group_human.
 env = make("CartPole-v1", env_num=9, render_mode="group_human")
-agent.set_env(env) # 训练好的智能体设置需要交互的环境
-obs, info = env.reset() # 环境进行初始化，得到初始的观测值和环境信息
+agent.set_env(env) # The agent requires an interactive environment.
+obs, info = env.reset() # Initialize the environment to obtain initial observations and environmental information.
 while True:
-    action, _ = agent.act(obs) # 智能体根据环境观测输入预测下一个动作
-    # 环境根据动作执行一步，得到下一个观测值、奖励、是否结束、环境信息
+    action, _ = agent.act(obs) # The agent predicts the next action based on environmental observations.
+    # The environment takes one step according to the action, obtains the next observation, reward, whether it ends and environmental information.
     obs, r, done, info = env.step(action)
     if any(done): break
-env.close() # 关闭测试环境
+env.close() # Close test environment
 ```
-在普通笔记本电脑上执行以上代码，只需要几秒钟，便可以完成该智能体的训练和可视化测试：
+Executing the above code on a regular laptop only takes **a few seconds**
+to complete the training. Below shows the visualization of the agent:
 
 <div align="center">
-  <img src="./docs/images/train_ppo_cartpole.gif"></a>
+  <img src="docs/images/train_ppo_cartpole.gif"></a>
 </div>
 
 
-**Tips:** 用户还可以在终端中通过执行一行命令快速训练`CartPole`环境:
+**Tips:** Users can also quickly train the `CartPole` environment by executing a command line in the terminal.
 ```bash
 openrl --mode train --env CartPole-v1
 ```
 
-对于多智能体、自然语言等任务的训练，OpenRL也提供了同样简单易用的接口。
+For training tasks such as multi-agent and natural language processing, OpenRL also provides a similarly simple and easy-to-use interface.
 
-关于如何进行多智能体训练、训练超参数设置、训练配置文件加载、wandb使用、保存gif动画等信息，请参考：
-- [多智能体训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/multi_agent_RL.html)
+For information on how to perform multi-agent training, set hyperparameters for training, load training configurations, use wandb, save GIF animations, etc., please refer to:
+- [Multi-Agent Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html)
 
-关于自然语言任务训练、Hugging Face上模型(数据)加载、自定义训练模型(奖励模型)等信息，请参考：
-- [对话任务训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
+For information on natural language task training, loading models/datasets on Hugging Face, customizing training models/reward models, etc., please refer to:
+- [Dialogue Task Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
 
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
 
 ## Gallery
 
-为了方便用户熟悉该框架，
-我们在[Gallery](./Gallery.md)中提供了更多使用OpenRL的示例和demo。
-也欢迎用户将自己的训练示例和demo贡献到Gallery中。
-
-## 使用OpenRL的研究项目
-
-我们在 [OpenRL Project](./Project.md) 中列举了使用OpenRL的研究项目。 
-如果你在研究项目中使用了OpenRL，也欢迎加入该列表。
-
-## 反馈和贡献
-- 有问题和发现bugs可以到 [Issues](https://github.com/OpenRL-Lab/openrl/issues) 处进行查询或提问
-- 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
+In order to facilitate users' familiarity with the framework, we provide more examples and demos of using OpenRL in [Gallery](./Gallery.md). 
+Users are also welcome to contribute their own training examples and demos to the Gallery.
 
-<div align="center">
-    <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
-</div>
+## Projects Using OpenRL
 
-- 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
-- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
-- 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
-- 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
+We have listed research projects that use OpenRL in the [OpenRL Project](./Project.md). 
+If you are using OpenRL in your research project, you are also welcome to join this list.
 
-OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
+## Feedback and Contribution
+- If you have any questions or find bugs, you can check or ask in the [Issues](https://github.com/OpenRL-Lab/openrl/issues).
+- Join the QQ group: [OpenRL Official Communication Group](docs/images/qq.png)
+<div align="center">
+<a href="docs/images/qq.png"><img width="250px" height="auto" src="docs/images/qq.png"></a>
+</div>
 
-- 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
-- [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development with us.
+- Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss OpenRL usage and development with us.
+- Send an E-mail to: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
+- Join the [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions).
+
+The OpenRL framework is still under continuous development and documentation. 
+We welcome you to join us in making this project better:
+- How to contribute code: Read the [Contributors' Guide](./CONTRIBUTING.md)
+- [OpenRL Roadmap](https://github.com/OpenRL-Lab/openrl/issues/2)
 
-## 维护人员
+## Maintainers
 
-目前，OpenRL由以下维护人员维护：
+At present, OpenRL is maintained by the following maintainers:
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
+- Yiwen Sun([@YiwenAI](https://github.com/YiwenAI))
 
-欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
+Welcome more contributors to join our maintenance team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) 
+to apply for joining the OpenRL team).
 
-## 支持者
+## Supporters
 
 ### &#8627; Contributors
 
 <a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
 </a>
 
@@ -265,15 +301,15 @@
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们:
+If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
```

#### html2text {}

```diff
@@ -1,181 +1,203 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.9 Summary: unified
-reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
-openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
-URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
-https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
-multi-agent reinforcement-learning-algorithms pytorch machine-learning
-baselines toolbox python data-science gym gymnasium Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: test
-Provides-Extra: dev Provides-Extra: mpe Provides-Extra: nlp License-File:
-LICENSE License-File: LICENSE.txt
-                        [./docs/images/openrl_text.png]
+                         [docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
-codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
+//codecov.io/gh/OpenRL-Lab/openrl_release) [![Documentation Status](https://
 readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
+docs.readthedocs.io/en/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
 docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
 github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
 OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
 forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
 github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
-The main branch is the latest version of OpenRL, which is under active
-development. If you just want to have a try with OpenRL, you can switch to the
-stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
-)
-OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
-OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
-ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
-ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
-æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
-[Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
-æ¯æLSTMï¼GRUï¼Transformerç­æ¨¡å -
-æ¯æå¤ç§è®­ç»å éï¼ä¾å¦ï¼èªå¨æ··åç²¾åº¦è®­ç»ï¼åç²¾åº¦ç­ç¥ç½ç»æ¶éæ°æ®ç­
-- æ¯æç¨æ·èªå®ä¹è®­ç»æ¨¡åãå¥å±æ¨¡åãè®­ç»æ°æ®ä»¥åç¯å¢ -
-æ¯æ[gymnasium](https://gymnasium.farama.org/)ç¯å¢ -
-æ¯æå­å¸è§æµç©ºé´ - æ¯æ[wandb](https://wandb.ai/)ï¼[tensorboardX]
-(https://tensorboardx.readthedocs.io/en/latest/
-index.html)ç­ä¸»æµè®­ç»å¯è§åå·¥å· -
-æ¯æç¯å¢çä¸²è¡åå¹¶è¡è®­ç»ï¼åæ¶ä¿è¯ä¸¤ç§æ¨¡å¼ä¸çè®­ç»ææä¸è´
-- ä¸­è±æææ¡£ - æä¾ååæµè¯åä»£ç è¦çæµè¯ - ç¬¦åBlack Code
-Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
-Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
-OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
-[å¼æºç¤¾åº](./
-CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
-(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
-[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
-(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
-[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
-(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
-[Acknowledgments](#acknowledgments) ## å®è£
-ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
-å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
-```bash conda install -c openrl openrl ```
-æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
-https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
-å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ```
-**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+OpenRL-Lab/openrl/blob/master/LICENSE) [![Embark](https://img.shields.io/badge/
+discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT) [!
+[slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&)]
+(https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
+Eeh0IxQ~DIaGqYXoW2IUQg) OpenRL-v0.0.16 is updated on July 30, 2023 The main
+branch is the latest version of OpenRL, which is under active development. If
+you just want to have a try with OpenRL, you can switch to the stable branch.
+## Welcome to OpenRL [Documentation](https://openrl-docs.readthedocs.io/en/
+latest/) | [ä¸­æä»ç»](README_zh.md) | [ä¸­æææ¡£](https://openrl-
+docs.readthedocs.io/zh/latest/)
+Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights
+                                   Welcome.
+
+OpenRL is an open-source general reinforcement learning research framework that
+supports training for various tasks such as single-agent, multi-agent, offline
+RL, self-play, and natural language. Developed based on PyTorch, the goal of
+OpenRL is to provide a simple-to-use, flexible, efficient and sustainable
+platform for the reinforcement learning research community. Currently, the
+features supported by OpenRL include: - A simple-to-use universal interface
+that supports training for both single-agent and multi-agent - Support for
+offline RL training with expert dataset - Support self-play training -
+Reinforcement learning training support for natural language tasks (such as
+dialogue) - Importing models and datasets from [Hugging Face](https://
+huggingface.co/) - Support for models such as LSTM, GRU, Transformer etc. -
+Multiple training acceleration methods including automatic mixed precision
+training and data collecting wth half precision policy network - User-defined
+training models, reward models, training data and environment support - Support
+for [gymnasium](https://gymnasium.farama.org/) environments - Support for
+[Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html),
+which can be used to implement various functions such as logging, saving, and
+early stopping - Dictionary observation space support - Popular visualization
+tools such as [wandb](https://wandb.ai/), [tensorboardX](https://
+tensorboardx.readthedocs.io/en/latest/index.html) are supported - Serial or
+parallel environment training while ensuring consistent results in both modes -
+Chinese and English documentation - Provides unit testing and code coverage
+testing - Compliant with Black Code Style guidelines and type checking
+Algorithms currently supported by OpenRL (for more details, please refer to
+[Gallery](./Gallery.md)): - [Proximal Policy Optimization (PPO)](https://
+arxiv.org/abs/1707.06347) - [Dual-clip PPO](https://arxiv.org/abs/1912.09729) -
+[Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955) - [Joint-ratio
+Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515) - [Generative
+Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476) -
+[Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf) -
+Self-Play - [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602) - [Multi-
+Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953) - [Value-
+Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296) - [Soft Actor
+Critic (SAC)](https://arxiv.org/abs/1812.05905) - [Deep Deterministic Policy
+Gradient (DDPG)](https://arxiv.org/abs/1509.02971) Environments currently
+supported by OpenRL (for more details, please refer to [Gallery](./
+Gallery.md)): - [Gymnasium](https://gymnasium.farama.org/) - [MuJoCo](https://
+github.com/deepmind/mujoco) - [PettingZoo](https://pettingzoo.farama.org/) -
+[MPE](https://github.com/openai/multiagent-particle-envs) - [Chat Bot](https://
+openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html) - [Atari]
+(https://gymnasium.farama.org/environments/atari/) - [StarCraft II](https://
+github.com/oxwhirl/smac) - [Omniverse Isaac Gym](https://github.com/NVIDIA-
+Omniverse/OmniIsaacGymEnvs) - [GridWorld](./examples/gridworld/) - [Super Mario
+Bros](https://github.com/Kautenja/gym-super-mario-bros) - [Gym Retro](https://
+github.com/openai/retro) This framework has undergone multiple iterations by
+the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in
+academic research. It has now become a mature reinforcement learning framework.
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone
+to join our [open-source community](./CONTRIBUTING.md) to contribute towards
+the development of reinforcement learning. For more information about OpenRL,
+please refer to the [documentation](https://openrl-docs.readthedocs.io/en/
+latest/). ## Outline - [Welcome to OpenRL](#welcome-to-openrl) - [Outline]
+(#outline) - [Installation](#installation) - [Use Docker](#use-docker) - [Quick
+Start](#quick-start) - [Gallery](#gallery) - [Projects Using OpenRL](#projects-
+using-openrl) - [Feedback and Contribution](#feedback-and-contribution) -
+[Maintainers](#maintainers) - [Supporters](#supporters) - [↳ Contributors](#-
+contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers](#-forkers) - [Citing
+OpenRL](#citing-openrl) - [License](#license) - [Acknowledgments]
+(#acknowledgments) ## Installation Users can directly install OpenRL via pip:
+```bash pip install openrl ``` If users are using Anaconda or Miniconda, they
+can also install OpenRL via conda: ```bash conda install -c openrl openrl ```
+Users who want to modify the source code can also install OpenRL from the
+source code: ```bash git clone https://github.com/OpenRL-Lab/openrl.git && cd
+openrl pip install -e . ``` After installation, users can check the version of
+OpenRL through command line: ```bash openrl --version ``` **Tips**: No
+installation required, try OpenRL online through Colab: [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-## ä½¿ç¨Docker
-OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
-å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
-```bash sudo docker pull openrllab/openrl-cpu ```
-å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
-```bash sudo docker pull openrllab/openrl ```
-éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
-```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
-å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
-è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
-```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
-openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
-OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
-ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
-train_ppo.py from openrl.envs.common import make from openrl.modules.common
-import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
-make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
-net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
-agent.train(total_time_steps=20000) #
-å¼å§è®­ç»ï¼å¹¶è®¾ç½®ç¯å¢è¿è¡æ»æ­¥æ°ä¸º20000 ```
-ä½¿ç¨OpenRLè®­ç»æºè½ä½åªéè¦ç®åçåæ­¥ï¼**åå»ºç¯å¢**=>**åå§åæ¨¡å**=>**åå§åæºè½ä½**=>**å¼å§è®­ç»**ï¼
-å¯¹äºè®­ç»å¥½çæºè½ä½ï¼ç¨æ·ä¹å¯ä»¥æ¹ä¾¿å°è¿è¡æºè½ä½çæµè¯:
-```python # train_ppo.py from openrl.envs.common import make from
-openrl.modules.common import PPONet as Net from openrl.runners.common import
-PPOAgent as Agent agent = Agent(Net(make("CartPole-v1", env_num=9))) #
-åå§åè®­ç»å¨ agent.train(total_time_steps=20000) #
-åå»ºç¨äºæµè¯çç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9ï¼è®¾ç½®æ¸²ææ¨¡å¼ä¸ºgroup_human
-env = make("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env
-(env) # è®­ç»å¥½çæºè½ä½è®¾ç½®éè¦äº¤äºçç¯å¢ obs, info = env.reset
-() # ç¯å¢è¿è¡åå§åï¼å¾å°åå§çè§æµå¼åç¯å¢ä¿¡æ¯ while
-True: action, _ = agent.act(obs) #
-æºè½ä½æ ¹æ®ç¯å¢è§æµè¾å¥é¢æµä¸ä¸ä¸ªå¨ä½ #
-ç¯å¢æ ¹æ®å¨ä½æ§è¡ä¸æ­¥ï¼å¾å°ä¸ä¸ä¸ªè§æµå¼ãå¥å±ãæ¯å¦ç»æãç¯å¢ä¿¡æ¯
-obs, r, done, info = env.step(action) if any(done): break env.close() #
-å³é­æµè¯ç¯å¢ ```
-å¨æ®éç¬è®°æ¬çµèä¸æ§è¡ä»¥ä¸ä»£ç ï¼åªéè¦å ç§éï¼ä¾¿å¯ä»¥å®æè¯¥æºè½ä½çè®­ç»åå¯è§åæµè¯ï¼
-                    [./docs/images/train_ppo_cartpole.gif]
-**Tips:**
-ç¨æ·è¿å¯ä»¥å¨ç»ç«¯ä¸­éè¿æ§è¡ä¸è¡å½ä»¤å¿«éè®­ç»`CartPole`ç¯å¢:
-```bash openrl --mode train --env CartPole-v1 ```
-å¯¹äºå¤æºè½ä½ãèªç¶è¯­è¨ç­ä»»å¡çè®­ç»ï¼OpenRLä¹æä¾äºåæ ·ç®åæç¨çæ¥å£ã
-å³äºå¦ä½è¿è¡å¤æºè½ä½è®­ç»ãè®­ç»è¶åæ°è®¾ç½®ãè®­ç»éç½®æä»¶å è½½ãwandbä½¿ç¨ãä¿å­gifå¨ç»ç­ä¿¡æ¯ï¼è¯·åèï¼
-- [å¤æºè½ä½è®­ç»ä¾å­](https://openrl-docs.readthedocs.io/zh/latest/
-quick_start/multi_agent_RL.html) å³äºèªç¶è¯­è¨ä»»å¡è®­ç»ãHugging
-Faceä¸æ¨¡å(æ°æ®)å è½½ãèªå®ä¹è®­ç»æ¨¡å
-(å¥å±æ¨¡å)ç­ä¿¡æ¯ï¼è¯·åèï¼ - [å¯¹è¯ä»»å¡è®­ç»ä¾å­](https://
-openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## Gallery
-ä¸ºäºæ¹ä¾¿ç¨æ·çæè¯¥æ¡æ¶ï¼ æä»¬å¨[Gallery](./
-Gallery.md)ä¸­æä¾äºæ´å¤ä½¿ç¨OpenRLçç¤ºä¾ådemoã
-ä¹æ¬¢è¿ç¨æ·å°èªå·±çè®­ç»ç¤ºä¾ådemoè´¡ç®å°Galleryä¸­ã ##
-ä½¿ç¨OpenRLçç ç©¶é¡¹ç® æä»¬å¨ [OpenRL Project](./Project.md)
-ä¸­åä¸¾äºä½¿ç¨OpenRLçç ç©¶é¡¹ç®ã
-å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
-åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
-OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
-[OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
-                            [./docs/images/qq.png]
-- å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
-Eeh0IxQ~DIaGqYXoW2IUQg)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
-(https://discord.gg/tyy96TGbep)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
-[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
-Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
-OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
-- å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
-[OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
-ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
-(https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
-huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
-æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
-[huangshiyu@4paradigm.com]
-(huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
-Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
-Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
-reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
-//reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
-openrl/network/members) ## Citing OpenRL
-å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
+## Use Docker OpenRL currently provides Docker images with and without GPU
+support. If the user's computer does not have an NVIDIA GPU, they can obtain an
+image without the GPU plugin using the following command: ```bash sudo docker
+pull openrllab/openrl-cpu ``` If the user wants to accelerate training with a
+GPU, they can obtain it using the following command: ```bash sudo docker pull
+openrllab/openrl ``` After successfully pulling the image, users can run
+OpenRL's Docker image using the following commands: ```bash # Without GPU
+acceleration sudo docker run -it openrllab/openrl-cpu # With GPU acceleration
+sudo docker run -it --gpus all --net host openrllab/openrl ``` Once inside the
+Docker container, users can check OpenRL's version and then run test cases
+using these commands: ```bash # Check OpenRL version in Docker container openrl
+--version # Run test case openrl --mode train --env CartPole-v1 ``` ## Quick
+Start OpenRL provides a simple and easy-to-use interface for beginners in
+reinforcement learning. Below is an example of using the PPO algorithm to train
+the `CartPole` environment: ```python # train_ppo.py from openrl.envs.common
+import make from openrl.modules.common import PPONet as Net from
+openrl.runners.common import PPOAgent as Agent env = make("CartPole-v1",
+env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network. agent = Agent(net) # Initialize the
+agent. agent.train(total_time_steps=20000) # Start training and set the total
+number of steps to 20,000 for the running environment. ``` Training an agent
+using OpenRL only requires four simple steps: **Create Environment** =>
+**Initialize Model** => **Initialize Agent** => **Start Training**! For a well-
+trained agent, users can also easily test the agent: ```python # train_ppo.py
+from openrl.envs.common import make from openrl.modules.common import PPONet as
+Net from openrl.runners.common import PPOAgent as Agent agent = Agent(Net(make
+("CartPole-v1", env_num=9))) # Initialize trainer. agent.train
+(total_time_steps=20000) # Create an environment for test, set the parallelism
+of the environment to 9, and set the rendering mode to group_human. env = make
+("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env(env) # The
+agent requires an interactive environment. obs, info = env.reset() # Initialize
+the environment to obtain initial observations and environmental information.
+while True: action, _ = agent.act(obs) # The agent predicts the next action
+based on environmental observations. # The environment takes one step according
+to the action, obtains the next observation, reward, whether it ends and
+environmental information. obs, r, done, info = env.step(action) if any(done):
+break env.close() # Close test environment ``` Executing the above code on a
+regular laptop only takes **a few seconds** to complete the training. Below
+shows the visualization of the agent:
+                     [docs/images/train_ppo_cartpole.gif]
+**Tips:** Users can also quickly train the `CartPole` environment by executing
+a command line in the terminal. ```bash openrl --mode train --env CartPole-v1
+``` For training tasks such as multi-agent and natural language processing,
+OpenRL also provides a similarly simple and easy-to-use interface. For
+information on how to perform multi-agent training, set hyperparameters for
+training, load training configurations, use wandb, save GIF animations, etc.,
+please refer to: - [Multi-Agent Training Example](https://openrl-
+docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html) For information
+on natural language task training, loading models/datasets on Hugging Face,
+customizing training models/reward models, etc., please refer to: - [Dialogue
+Task Training Example](https://openrl-docs.readthedocs.io/en/latest/
+quick_start/train_nlp.html) For more information about OpenRL, please refer to
+the [documentation](https://openrl-docs.readthedocs.io/en/latest/). ## Gallery
+In order to facilitate users' familiarity with the framework, we provide more
+examples and demos of using OpenRL in [Gallery](./Gallery.md). Users are also
+welcome to contribute their own training examples and demos to the Gallery. ##
+Projects Using OpenRL We have listed research projects that use OpenRL in the
+[OpenRL Project](./Project.md). If you are using OpenRL in your research
+project, you are also welcome to join this list. ## Feedback and Contribution -
+If you have any questions or find bugs, you can check or ask in the [Issues]
+(https://github.com/OpenRL-Lab/openrl/issues). - Join the QQ group: [OpenRL
+Official Communication Group](docs/images/qq.png)
+                             [docs/images/qq.png]
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-
+1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development
+with us. - Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss
+OpenRL usage and development with us. - Send an E-mail to:
+[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - Join the [GitHub
+Discussion](https://github.com/orgs/OpenRL-Lab/discussions). The OpenRL
+framework is still under continuous development and documentation. We welcome
+you to join us in making this project better: - How to contribute code: Read
+the [Contributors' Guide](./CONTRIBUTING.md) - [OpenRL Roadmap](https://
+github.com/OpenRL-Lab/openrl/issues/2) ## Maintainers At present, OpenRL is
+maintained by the following maintainers: - [Shiyu Huang](https://
+huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13)) -
+Wenze Chen([@Chen001117](https://github.com/Chen001117)) - Yiwen Sun([@YiwenAI]
+(https://github.com/YiwenAI)) Welcome more contributors to join our maintenance
+team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) to
+apply for joining the OpenRL team). ## Supporters ### ↳ Contributors [https://
+contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳ Stargazers [![Stargazers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/stargazers) ### ↳ Forkers [![Forkers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/network/members) ## Citing OpenRL If our
+work has been helpful to you, please feel free to cite us: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
 #OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
 Acknowledgments The development of the OpenRL framework has drawn on the
 strengths of other reinforcement learning frameworks: - Stable-baselines3:
```

### Comparing `openrl-0.0.9/README.md` & `openrl-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,328 @@
+Metadata-Version: 2.1
+Name: openrl
+Version: 0.1.0
+Summary: unified reinforcement learning framework
+Home-page: https://github.com/OpenRL-Lab/openrl
+Author: openrl contributors
+Author-email: huangsy1314@163.com
+Project-URL: Code, https://github.com/OpenRL-Lab/openrl
+Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
+Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: mpe
+Provides-Extra: nlp
+Provides-Extra: selfplay
+Provides-Extra: retro
+Provides-Extra: super_mario
+License-File: LICENSE
+
 <div align="center">
-    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
+    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
-[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/en/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.9 is updated on May 6, 2023 
+[![Embark](https://img.shields.io/badge/discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT)
+[![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg)
+
+OpenRL-v0.0.16 is updated on July 30, 2023
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
-## 欢迎来到OpenRL
+## Welcome to OpenRL
+
+[Documentation](https://openrl-docs.readthedocs.io/en/latest/) | [中文介绍](README_zh.md) |  [中文文档](https://openrl-docs.readthedocs.io/zh/latest/)
+
+<div align="center">
+    Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights Welcome.   <br><br>
+</div>
+
+OpenRL is an open-source general reinforcement learning research framework that supports training for various tasks 
+such as single-agent, multi-agent, offline RL, self-play, and natural language. 
+Developed based on PyTorch, the goal of OpenRL is to provide a simple-to-use, flexible, efficient and sustainable platform for the reinforcement learning research community.
+
+Currently, the features supported by OpenRL include:
+
+- A simple-to-use universal interface that supports training for both single-agent and multi-agent
+
+- Support for offline RL training with expert dataset
+
+- Support self-play training
+
+- Reinforcement learning training support for natural language tasks (such as dialogue)
+
+- Importing models and datasets from [Hugging Face](https://huggingface.co/)
+
+- Support for models such as LSTM, GRU, Transformer etc.
+
+- Multiple training acceleration methods including automatic mixed precision training and data collecting wth half precision policy network
+
+- User-defined training models, reward models, training data and environment support
+
+- Support for [gymnasium](https://gymnasium.farama.org/) environments
+
+- Support for [Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html), which can be used to implement various functions such as logging, saving, and early stopping
+
+- Dictionary observation space support
+
+- Popular visualization tools such as [wandb](https://wandb.ai/),  [tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html) are supported
+
+- Serial or parallel environment training while ensuring consistent results in both modes
 
-[English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
+- Chinese and English documentation
 
-OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
-目前，OpenRL支持的特性包括：
+- Provides unit testing and code coverage testing
 
-- 简单易用且支持单智能体、多智能体训练的通用接口
-- 支持自然语言任务（如对话任务）的强化学习训练
-- 支持从[Hugging Face](https://huggingface.co/)上导入模型和数据
-- 支持LSTM，GRU，Transformer等模型
-- 支持多种训练加速，例如：自动混合精度训练，半精度策略网络收集数据等
-- 支持用户自定义训练模型、奖励模型、训练数据以及环境
-- 支持[gymnasium](https://gymnasium.farama.org/)环境
-- 支持字典观测空间
-- 支持[wandb](https://wandb.ai/)，[tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html)等主流训练可视化工具
-- 支持环境的串行和并行训练，同时保证两种模式下的训练效果一致
-- 中英文文档
-- 提供单元测试和代码覆盖测试
-- 符合Black Code Style和类型检查
-
-该框架经过了[OpenRL-Lab](https://github.com/OpenRL-Lab)的多次迭代并应用于学术研究，目前已经成为了一个成熟的强化学习框架。
-OpenRL-Lab将持续维护和更新OpenRL，欢迎大家加入我们的[开源社区](./CONTRIBUTING.md)，一起为强化学习的发展做出贡献。
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
-
-## 目录
-
-- [欢迎来到OpenRL](#欢迎来到openrl)
-- [目录](#目录)
-- [安装](#安装)
-- [使用Docker](#使用docker)
-- [快速上手](#快速上手)
-- [Gallery](#Gallery)
-- [使用OpenRL的项目](#使用OpenRL的项目)
-- [反馈和贡献](#反馈和贡献)
-- [维护人员](#维护人员)
-- [支持者](#支持者)
-  - [&#8627; Contributors](#-contributors)  
+- Compliant with Black Code Style guidelines and type checking
+
+Algorithms currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Proximal Policy Optimization (PPO)](https://arxiv.org/abs/1707.06347)
+- [Dual-clip PPO](https://arxiv.org/abs/1912.09729)
+- [Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955)
+- [Joint-ratio Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515)
+- [Generative Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476)
+- [Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf)
+- Self-Play
+- [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602)
+- [Multi-Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953)
+- [Value-Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296)
+- [Soft Actor Critic (SAC)](https://arxiv.org/abs/1812.05905)
+- [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/abs/1509.02971)
+
+Environments currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Gymnasium](https://gymnasium.farama.org/)
+- [MuJoCo](https://github.com/deepmind/mujoco)
+- [PettingZoo](https://pettingzoo.farama.org/)
+- [MPE](https://github.com/openai/multiagent-particle-envs)
+- [Chat Bot](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
+- [Atari](https://gymnasium.farama.org/environments/atari/)
+- [StarCraft II](https://github.com/oxwhirl/smac)
+- [Omniverse Isaac Gym](https://github.com/NVIDIA-Omniverse/OmniIsaacGymEnvs)
+- [GridWorld](./examples/gridworld/)
+- [Super Mario Bros](https://github.com/Kautenja/gym-super-mario-bros)
+- [Gym Retro](https://github.com/openai/retro)
+
+This framework has undergone multiple iterations by the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in academic research. 
+It has now become a mature reinforcement learning framework.
+
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone to join our [open-source community](./CONTRIBUTING.md) 
+to contribute towards the development of reinforcement learning.
+
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
+
+## Outline
+
+- [Welcome to OpenRL](#welcome-to-openrl)
+- [Outline](#outline)
+- [Installation](#installation)
+- [Use Docker](#use-docker)
+- [Quick Start](#quick-start)
+- [Gallery](#gallery)
+- [Projects Using OpenRL](#projects-using-openrl)
+- [Feedback and Contribution](#feedback-and-contribution)
+- [Maintainers](#maintainers)
+- [Supporters](#supporters)
+  - [&#8627; Contributors](#-contributors) 
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
-## 安装
+## Installation
+
+Users can directly install OpenRL via pip:
 
-用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
 
-如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
+If users are using Anaconda or Miniconda, they can also install OpenRL via conda:
+
 ```bash
 conda install -c openrl openrl
 ```
 
-想要修改源码的用户也可以从源码安装OpenRL:
+Users who want to modify the source code can also install OpenRL from the source code:
+
 ```bash
 git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
-安装完成后，用户可以直接通过命令行查看OpenRL的版本：
+After installation, users can check the version of OpenRL through command line:
+
 ```bash
 openrl --version
 ```
 
-**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-
-## 使用Docker
+**Tips**: No installation required, try OpenRL online through Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
 
-OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
-如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+## Use Docker
 
+OpenRL currently provides Docker images with and without GPU support. 
+If the user's computer does not have an NVIDIA GPU, they can obtain an image without the GPU plugin using the following command:
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
-如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+If the user wants to accelerate training with a GPU, they can obtain it using the following command:
 ```bash
 sudo docker pull openrllab/openrl
 ```
 
-镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+After successfully pulling the image, users can run OpenRL's Docker image using the following commands:
 ```bash
-# 不带显卡加速
+# Without GPU acceleration
 sudo docker run -it openrllab/openrl-cpu
-# 带显卡加速
+# With GPU acceleration 
 sudo docker run -it --gpus all --net host openrllab/openrl
 ```
 
-进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
-```bash
-# 查看Docker镜像中OpenRL的版本
-openrl --version
-# 运行测例
-openrl --mode train --env CartPole-v1
+Once inside the Docker container, users can check OpenRL's version and then run test cases using these commands: 
+```bash 
+# Check OpenRL version in Docker container  
+openrl --version  
+# Run test case  
+openrl --mode train --env CartPole-v1  
 ```
 
+## Quick Start
 
-## 快速上手
-
-OpenRL为强化学习入门用户提供了简单易用的接口，
-下面是一个使用PPO算法训练`CartPole`环境的例子：
+OpenRL provides a simple and easy-to-use interface for beginners in reinforcement learning. 
+Below is an example of using the PPO algorithm to train the `CartPole` environment:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-env = make("CartPole-v1", env_num=9) # 创建环境，并设置环境并行数为9
-net = Net(env) # 创建神经网络
-agent = Agent(net) # 初始化智能体
-agent.train(total_time_steps=20000) # 开始训练，并设置环境运行总步数为20000
+env = make("CartPole-v1", env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network.
+agent = Agent(net) # Initialize the agent.
+agent.train(total_time_steps=20000) # Start training and set the total number of steps to 20,000 for the running environment.
 ```
-使用OpenRL训练智能体只需要简单的四步：**创建环境**=>**初始化模型**=>**初始化智能体**=>**开始训练**！
+Training an agent using OpenRL only requires four simple steps: 
+**Create Environment** => **Initialize Model** => **Initialize Agent** => **Start Training**!
 
-对于训练好的智能体，用户也可以方便地进行智能体的测试:
+For a well-trained agent, users can also easily test the agent:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-agent = Agent(Net(make("CartPole-v1", env_num=9))) # 初始化训练器
+agent = Agent(Net(make("CartPole-v1", env_num=9))) # Initialize trainer.
 agent.train(total_time_steps=20000)
-# 创建用于测试的环境，并设置环境并行数为9，设置渲染模式为group_human
+# Create an environment for test, set the parallelism of the environment to 9, and set the rendering mode to group_human.
 env = make("CartPole-v1", env_num=9, render_mode="group_human")
-agent.set_env(env) # 训练好的智能体设置需要交互的环境
-obs, info = env.reset() # 环境进行初始化，得到初始的观测值和环境信息
+agent.set_env(env) # The agent requires an interactive environment.
+obs, info = env.reset() # Initialize the environment to obtain initial observations and environmental information.
 while True:
-    action, _ = agent.act(obs) # 智能体根据环境观测输入预测下一个动作
-    # 环境根据动作执行一步，得到下一个观测值、奖励、是否结束、环境信息
+    action, _ = agent.act(obs) # The agent predicts the next action based on environmental observations.
+    # The environment takes one step according to the action, obtains the next observation, reward, whether it ends and environmental information.
     obs, r, done, info = env.step(action)
     if any(done): break
-env.close() # 关闭测试环境
+env.close() # Close test environment
 ```
-在普通笔记本电脑上执行以上代码，只需要几秒钟，便可以完成该智能体的训练和可视化测试：
+Executing the above code on a regular laptop only takes **a few seconds**
+to complete the training. Below shows the visualization of the agent:
 
 <div align="center">
-  <img src="./docs/images/train_ppo_cartpole.gif"></a>
+  <img src="docs/images/train_ppo_cartpole.gif"></a>
 </div>
 
 
-**Tips:** 用户还可以在终端中通过执行一行命令快速训练`CartPole`环境:
+**Tips:** Users can also quickly train the `CartPole` environment by executing a command line in the terminal.
 ```bash
 openrl --mode train --env CartPole-v1
 ```
 
-对于多智能体、自然语言等任务的训练，OpenRL也提供了同样简单易用的接口。
+For training tasks such as multi-agent and natural language processing, OpenRL also provides a similarly simple and easy-to-use interface.
 
-关于如何进行多智能体训练、训练超参数设置、训练配置文件加载、wandb使用、保存gif动画等信息，请参考：
-- [多智能体训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/multi_agent_RL.html)
+For information on how to perform multi-agent training, set hyperparameters for training, load training configurations, use wandb, save GIF animations, etc., please refer to:
+- [Multi-Agent Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html)
 
-关于自然语言任务训练、Hugging Face上模型(数据)加载、自定义训练模型(奖励模型)等信息，请参考：
-- [对话任务训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
+For information on natural language task training, loading models/datasets on Hugging Face, customizing training models/reward models, etc., please refer to:
+- [Dialogue Task Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
 
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
 
 ## Gallery
 
-为了方便用户熟悉该框架，
-我们在[Gallery](./Gallery.md)中提供了更多使用OpenRL的示例和demo。
-也欢迎用户将自己的训练示例和demo贡献到Gallery中。
-
-## 使用OpenRL的研究项目
-
-我们在 [OpenRL Project](./Project.md) 中列举了使用OpenRL的研究项目。 
-如果你在研究项目中使用了OpenRL，也欢迎加入该列表。
-
-## 反馈和贡献
-- 有问题和发现bugs可以到 [Issues](https://github.com/OpenRL-Lab/openrl/issues) 处进行查询或提问
-- 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
+In order to facilitate users' familiarity with the framework, we provide more examples and demos of using OpenRL in [Gallery](./Gallery.md). 
+Users are also welcome to contribute their own training examples and demos to the Gallery.
 
-<div align="center">
-    <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
-</div>
+## Projects Using OpenRL
 
-- 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
-- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
-- 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
-- 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
+We have listed research projects that use OpenRL in the [OpenRL Project](./Project.md). 
+If you are using OpenRL in your research project, you are also welcome to join this list.
 
-OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
+## Feedback and Contribution
+- If you have any questions or find bugs, you can check or ask in the [Issues](https://github.com/OpenRL-Lab/openrl/issues).
+- Join the QQ group: [OpenRL Official Communication Group](docs/images/qq.png)
+<div align="center">
+<a href="docs/images/qq.png"><img width="250px" height="auto" src="docs/images/qq.png"></a>
+</div>
 
-- 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
-- [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development with us.
+- Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss OpenRL usage and development with us.
+- Send an E-mail to: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
+- Join the [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions).
+
+The OpenRL framework is still under continuous development and documentation. 
+We welcome you to join us in making this project better:
+- How to contribute code: Read the [Contributors' Guide](./CONTRIBUTING.md)
+- [OpenRL Roadmap](https://github.com/OpenRL-Lab/openrl/issues/2)
 
-## 维护人员
+## Maintainers
 
-目前，OpenRL由以下维护人员维护：
+At present, OpenRL is maintained by the following maintainers:
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
+- Yiwen Sun([@YiwenAI](https://github.com/YiwenAI))
 
-欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
+Welcome more contributors to join our maintenance team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) 
+to apply for joining the OpenRL team).
 
-## 支持者
+## Supporters
 
 ### &#8627; Contributors
 
 <a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
 </a>
 
@@ -238,15 +332,15 @@
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们:
+If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
```

#### html2text {}

```diff
@@ -1,165 +1,221 @@
-                        [./docs/images/openrl_text.png]
+Metadata-Version: 2.1 Name: openrl Version: 0.1.0 Summary: unified
+reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
+openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
+URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
+https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
+multi-agent reinforcement-learning-algorithms pytorch machine-learning
+baselines toolbox python data-science gym gymnasium Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
+nlp Provides-Extra: selfplay Provides-Extra: retro Provides-Extra: super_mario
+License-File: LICENSE
+                         [docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
-codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
+//codecov.io/gh/OpenRL-Lab/openrl_release) [![Documentation Status](https://
 readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
+docs.readthedocs.io/en/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
 docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
 github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
 OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
 forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
 github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
-The main branch is the latest version of OpenRL, which is under active
-development. If you just want to have a try with OpenRL, you can switch to the
-stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
-)
-OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
-OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
-ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
-ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
-æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
-[Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
-æ¯æLSTMï¼GRUï¼Transformerç­æ¨¡å -
-æ¯æå¤ç§è®­ç»å éï¼ä¾å¦ï¼èªå¨æ··åç²¾åº¦è®­ç»ï¼åç²¾åº¦ç­ç¥ç½ç»æ¶éæ°æ®ç­
-- æ¯æç¨æ·èªå®ä¹è®­ç»æ¨¡åãå¥å±æ¨¡åãè®­ç»æ°æ®ä»¥åç¯å¢ -
-æ¯æ[gymnasium](https://gymnasium.farama.org/)ç¯å¢ -
-æ¯æå­å¸è§æµç©ºé´ - æ¯æ[wandb](https://wandb.ai/)ï¼[tensorboardX]
-(https://tensorboardx.readthedocs.io/en/latest/
-index.html)ç­ä¸»æµè®­ç»å¯è§åå·¥å· -
-æ¯æç¯å¢çä¸²è¡åå¹¶è¡è®­ç»ï¼åæ¶ä¿è¯ä¸¤ç§æ¨¡å¼ä¸çè®­ç»ææä¸è´
-- ä¸­è±æææ¡£ - æä¾ååæµè¯åä»£ç è¦çæµè¯ - ç¬¦åBlack Code
-Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
-Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
-OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
-[å¼æºç¤¾åº](./
-CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
-(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
-[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
-(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
-[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
-(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
-[Acknowledgments](#acknowledgments) ## å®è£
-ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
-å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
-```bash conda install -c openrl openrl ```
-æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
-https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
-å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ```
-**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+OpenRL-Lab/openrl/blob/master/LICENSE) [![Embark](https://img.shields.io/badge/
+discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT) [!
+[slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&)]
+(https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
+Eeh0IxQ~DIaGqYXoW2IUQg) OpenRL-v0.0.16 is updated on July 30, 2023 The main
+branch is the latest version of OpenRL, which is under active development. If
+you just want to have a try with OpenRL, you can switch to the stable branch.
+## Welcome to OpenRL [Documentation](https://openrl-docs.readthedocs.io/en/
+latest/) | [ä¸­æä»ç»](README_zh.md) | [ä¸­æææ¡£](https://openrl-
+docs.readthedocs.io/zh/latest/)
+Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights
+                                   Welcome.
+
+OpenRL is an open-source general reinforcement learning research framework that
+supports training for various tasks such as single-agent, multi-agent, offline
+RL, self-play, and natural language. Developed based on PyTorch, the goal of
+OpenRL is to provide a simple-to-use, flexible, efficient and sustainable
+platform for the reinforcement learning research community. Currently, the
+features supported by OpenRL include: - A simple-to-use universal interface
+that supports training for both single-agent and multi-agent - Support for
+offline RL training with expert dataset - Support self-play training -
+Reinforcement learning training support for natural language tasks (such as
+dialogue) - Importing models and datasets from [Hugging Face](https://
+huggingface.co/) - Support for models such as LSTM, GRU, Transformer etc. -
+Multiple training acceleration methods including automatic mixed precision
+training and data collecting wth half precision policy network - User-defined
+training models, reward models, training data and environment support - Support
+for [gymnasium](https://gymnasium.farama.org/) environments - Support for
+[Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html),
+which can be used to implement various functions such as logging, saving, and
+early stopping - Dictionary observation space support - Popular visualization
+tools such as [wandb](https://wandb.ai/), [tensorboardX](https://
+tensorboardx.readthedocs.io/en/latest/index.html) are supported - Serial or
+parallel environment training while ensuring consistent results in both modes -
+Chinese and English documentation - Provides unit testing and code coverage
+testing - Compliant with Black Code Style guidelines and type checking
+Algorithms currently supported by OpenRL (for more details, please refer to
+[Gallery](./Gallery.md)): - [Proximal Policy Optimization (PPO)](https://
+arxiv.org/abs/1707.06347) - [Dual-clip PPO](https://arxiv.org/abs/1912.09729) -
+[Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955) - [Joint-ratio
+Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515) - [Generative
+Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476) -
+[Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf) -
+Self-Play - [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602) - [Multi-
+Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953) - [Value-
+Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296) - [Soft Actor
+Critic (SAC)](https://arxiv.org/abs/1812.05905) - [Deep Deterministic Policy
+Gradient (DDPG)](https://arxiv.org/abs/1509.02971) Environments currently
+supported by OpenRL (for more details, please refer to [Gallery](./
+Gallery.md)): - [Gymnasium](https://gymnasium.farama.org/) - [MuJoCo](https://
+github.com/deepmind/mujoco) - [PettingZoo](https://pettingzoo.farama.org/) -
+[MPE](https://github.com/openai/multiagent-particle-envs) - [Chat Bot](https://
+openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html) - [Atari]
+(https://gymnasium.farama.org/environments/atari/) - [StarCraft II](https://
+github.com/oxwhirl/smac) - [Omniverse Isaac Gym](https://github.com/NVIDIA-
+Omniverse/OmniIsaacGymEnvs) - [GridWorld](./examples/gridworld/) - [Super Mario
+Bros](https://github.com/Kautenja/gym-super-mario-bros) - [Gym Retro](https://
+github.com/openai/retro) This framework has undergone multiple iterations by
+the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in
+academic research. It has now become a mature reinforcement learning framework.
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone
+to join our [open-source community](./CONTRIBUTING.md) to contribute towards
+the development of reinforcement learning. For more information about OpenRL,
+please refer to the [documentation](https://openrl-docs.readthedocs.io/en/
+latest/). ## Outline - [Welcome to OpenRL](#welcome-to-openrl) - [Outline]
+(#outline) - [Installation](#installation) - [Use Docker](#use-docker) - [Quick
+Start](#quick-start) - [Gallery](#gallery) - [Projects Using OpenRL](#projects-
+using-openrl) - [Feedback and Contribution](#feedback-and-contribution) -
+[Maintainers](#maintainers) - [Supporters](#supporters) - [↳ Contributors](#-
+contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers](#-forkers) - [Citing
+OpenRL](#citing-openrl) - [License](#license) - [Acknowledgments]
+(#acknowledgments) ## Installation Users can directly install OpenRL via pip:
+```bash pip install openrl ``` If users are using Anaconda or Miniconda, they
+can also install OpenRL via conda: ```bash conda install -c openrl openrl ```
+Users who want to modify the source code can also install OpenRL from the
+source code: ```bash git clone https://github.com/OpenRL-Lab/openrl.git && cd
+openrl pip install -e . ``` After installation, users can check the version of
+OpenRL through command line: ```bash openrl --version ``` **Tips**: No
+installation required, try OpenRL online through Colab: [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-## ä½¿ç¨Docker
-OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
-å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
-```bash sudo docker pull openrllab/openrl-cpu ```
-å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
-```bash sudo docker pull openrllab/openrl ```
-éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
-```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
-å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
-è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
-```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
-openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
-OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
-ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
-train_ppo.py from openrl.envs.common import make from openrl.modules.common
-import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
-make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
-net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
-agent.train(total_time_steps=20000) #
-å¼å§è®­ç»ï¼å¹¶è®¾ç½®ç¯å¢è¿è¡æ»æ­¥æ°ä¸º20000 ```
-ä½¿ç¨OpenRLè®­ç»æºè½ä½åªéè¦ç®åçåæ­¥ï¼**åå»ºç¯å¢**=>**åå§åæ¨¡å**=>**åå§åæºè½ä½**=>**å¼å§è®­ç»**ï¼
-å¯¹äºè®­ç»å¥½çæºè½ä½ï¼ç¨æ·ä¹å¯ä»¥æ¹ä¾¿å°è¿è¡æºè½ä½çæµè¯:
-```python # train_ppo.py from openrl.envs.common import make from
-openrl.modules.common import PPONet as Net from openrl.runners.common import
-PPOAgent as Agent agent = Agent(Net(make("CartPole-v1", env_num=9))) #
-åå§åè®­ç»å¨ agent.train(total_time_steps=20000) #
-åå»ºç¨äºæµè¯çç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9ï¼è®¾ç½®æ¸²ææ¨¡å¼ä¸ºgroup_human
-env = make("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env
-(env) # è®­ç»å¥½çæºè½ä½è®¾ç½®éè¦äº¤äºçç¯å¢ obs, info = env.reset
-() # ç¯å¢è¿è¡åå§åï¼å¾å°åå§çè§æµå¼åç¯å¢ä¿¡æ¯ while
-True: action, _ = agent.act(obs) #
-æºè½ä½æ ¹æ®ç¯å¢è§æµè¾å¥é¢æµä¸ä¸ä¸ªå¨ä½ #
-ç¯å¢æ ¹æ®å¨ä½æ§è¡ä¸æ­¥ï¼å¾å°ä¸ä¸ä¸ªè§æµå¼ãå¥å±ãæ¯å¦ç»æãç¯å¢ä¿¡æ¯
-obs, r, done, info = env.step(action) if any(done): break env.close() #
-å³é­æµè¯ç¯å¢ ```
-å¨æ®éç¬è®°æ¬çµèä¸æ§è¡ä»¥ä¸ä»£ç ï¼åªéè¦å ç§éï¼ä¾¿å¯ä»¥å®æè¯¥æºè½ä½çè®­ç»åå¯è§åæµè¯ï¼
-                    [./docs/images/train_ppo_cartpole.gif]
-**Tips:**
-ç¨æ·è¿å¯ä»¥å¨ç»ç«¯ä¸­éè¿æ§è¡ä¸è¡å½ä»¤å¿«éè®­ç»`CartPole`ç¯å¢:
-```bash openrl --mode train --env CartPole-v1 ```
-å¯¹äºå¤æºè½ä½ãèªç¶è¯­è¨ç­ä»»å¡çè®­ç»ï¼OpenRLä¹æä¾äºåæ ·ç®åæç¨çæ¥å£ã
-å³äºå¦ä½è¿è¡å¤æºè½ä½è®­ç»ãè®­ç»è¶åæ°è®¾ç½®ãè®­ç»éç½®æä»¶å è½½ãwandbä½¿ç¨ãä¿å­gifå¨ç»ç­ä¿¡æ¯ï¼è¯·åèï¼
-- [å¤æºè½ä½è®­ç»ä¾å­](https://openrl-docs.readthedocs.io/zh/latest/
-quick_start/multi_agent_RL.html) å³äºèªç¶è¯­è¨ä»»å¡è®­ç»ãHugging
-Faceä¸æ¨¡å(æ°æ®)å è½½ãèªå®ä¹è®­ç»æ¨¡å
-(å¥å±æ¨¡å)ç­ä¿¡æ¯ï¼è¯·åèï¼ - [å¯¹è¯ä»»å¡è®­ç»ä¾å­](https://
-openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## Gallery
-ä¸ºäºæ¹ä¾¿ç¨æ·çæè¯¥æ¡æ¶ï¼ æä»¬å¨[Gallery](./
-Gallery.md)ä¸­æä¾äºæ´å¤ä½¿ç¨OpenRLçç¤ºä¾ådemoã
-ä¹æ¬¢è¿ç¨æ·å°èªå·±çè®­ç»ç¤ºä¾ådemoè´¡ç®å°Galleryä¸­ã ##
-ä½¿ç¨OpenRLçç ç©¶é¡¹ç® æä»¬å¨ [OpenRL Project](./Project.md)
-ä¸­åä¸¾äºä½¿ç¨OpenRLçç ç©¶é¡¹ç®ã
-å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
-åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
-OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
-[OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
-                            [./docs/images/qq.png]
-- å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
-Eeh0IxQ~DIaGqYXoW2IUQg)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
-(https://discord.gg/tyy96TGbep)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
-[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
-Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
-OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
-- å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
-[OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
-ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
-(https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
-huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
-æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
-[huangshiyu@4paradigm.com]
-(huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
-Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
-Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
-reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
-//reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
-openrl/network/members) ## Citing OpenRL
-å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
+## Use Docker OpenRL currently provides Docker images with and without GPU
+support. If the user's computer does not have an NVIDIA GPU, they can obtain an
+image without the GPU plugin using the following command: ```bash sudo docker
+pull openrllab/openrl-cpu ``` If the user wants to accelerate training with a
+GPU, they can obtain it using the following command: ```bash sudo docker pull
+openrllab/openrl ``` After successfully pulling the image, users can run
+OpenRL's Docker image using the following commands: ```bash # Without GPU
+acceleration sudo docker run -it openrllab/openrl-cpu # With GPU acceleration
+sudo docker run -it --gpus all --net host openrllab/openrl ``` Once inside the
+Docker container, users can check OpenRL's version and then run test cases
+using these commands: ```bash # Check OpenRL version in Docker container openrl
+--version # Run test case openrl --mode train --env CartPole-v1 ``` ## Quick
+Start OpenRL provides a simple and easy-to-use interface for beginners in
+reinforcement learning. Below is an example of using the PPO algorithm to train
+the `CartPole` environment: ```python # train_ppo.py from openrl.envs.common
+import make from openrl.modules.common import PPONet as Net from
+openrl.runners.common import PPOAgent as Agent env = make("CartPole-v1",
+env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network. agent = Agent(net) # Initialize the
+agent. agent.train(total_time_steps=20000) # Start training and set the total
+number of steps to 20,000 for the running environment. ``` Training an agent
+using OpenRL only requires four simple steps: **Create Environment** =>
+**Initialize Model** => **Initialize Agent** => **Start Training**! For a well-
+trained agent, users can also easily test the agent: ```python # train_ppo.py
+from openrl.envs.common import make from openrl.modules.common import PPONet as
+Net from openrl.runners.common import PPOAgent as Agent agent = Agent(Net(make
+("CartPole-v1", env_num=9))) # Initialize trainer. agent.train
+(total_time_steps=20000) # Create an environment for test, set the parallelism
+of the environment to 9, and set the rendering mode to group_human. env = make
+("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env(env) # The
+agent requires an interactive environment. obs, info = env.reset() # Initialize
+the environment to obtain initial observations and environmental information.
+while True: action, _ = agent.act(obs) # The agent predicts the next action
+based on environmental observations. # The environment takes one step according
+to the action, obtains the next observation, reward, whether it ends and
+environmental information. obs, r, done, info = env.step(action) if any(done):
+break env.close() # Close test environment ``` Executing the above code on a
+regular laptop only takes **a few seconds** to complete the training. Below
+shows the visualization of the agent:
+                     [docs/images/train_ppo_cartpole.gif]
+**Tips:** Users can also quickly train the `CartPole` environment by executing
+a command line in the terminal. ```bash openrl --mode train --env CartPole-v1
+``` For training tasks such as multi-agent and natural language processing,
+OpenRL also provides a similarly simple and easy-to-use interface. For
+information on how to perform multi-agent training, set hyperparameters for
+training, load training configurations, use wandb, save GIF animations, etc.,
+please refer to: - [Multi-Agent Training Example](https://openrl-
+docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html) For information
+on natural language task training, loading models/datasets on Hugging Face,
+customizing training models/reward models, etc., please refer to: - [Dialogue
+Task Training Example](https://openrl-docs.readthedocs.io/en/latest/
+quick_start/train_nlp.html) For more information about OpenRL, please refer to
+the [documentation](https://openrl-docs.readthedocs.io/en/latest/). ## Gallery
+In order to facilitate users' familiarity with the framework, we provide more
+examples and demos of using OpenRL in [Gallery](./Gallery.md). Users are also
+welcome to contribute their own training examples and demos to the Gallery. ##
+Projects Using OpenRL We have listed research projects that use OpenRL in the
+[OpenRL Project](./Project.md). If you are using OpenRL in your research
+project, you are also welcome to join this list. ## Feedback and Contribution -
+If you have any questions or find bugs, you can check or ask in the [Issues]
+(https://github.com/OpenRL-Lab/openrl/issues). - Join the QQ group: [OpenRL
+Official Communication Group](docs/images/qq.png)
+                             [docs/images/qq.png]
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-
+1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development
+with us. - Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss
+OpenRL usage and development with us. - Send an E-mail to:
+[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - Join the [GitHub
+Discussion](https://github.com/orgs/OpenRL-Lab/discussions). The OpenRL
+framework is still under continuous development and documentation. We welcome
+you to join us in making this project better: - How to contribute code: Read
+the [Contributors' Guide](./CONTRIBUTING.md) - [OpenRL Roadmap](https://
+github.com/OpenRL-Lab/openrl/issues/2) ## Maintainers At present, OpenRL is
+maintained by the following maintainers: - [Shiyu Huang](https://
+huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13)) -
+Wenze Chen([@Chen001117](https://github.com/Chen001117)) - Yiwen Sun([@YiwenAI]
+(https://github.com/YiwenAI)) Welcome more contributors to join our maintenance
+team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) to
+apply for joining the OpenRL team). ## Supporters ### ↳ Contributors [https://
+contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳ Stargazers [![Stargazers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/stargazers) ### ↳ Forkers [![Forkers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/network/members) ## Citing OpenRL If our
+work has been helpful to you, please feel free to cite us: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
 #OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
 Acknowledgments The development of the OpenRL framework has drawn on the
 strengths of other reinforcement learning frameworks: - Stable-baselines3:
```

### Comparing `openrl-0.0.9/openrl/algorithms/__init__.py` & `openrl-0.1.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/algorithms/base_algorithm.py` & `openrl-0.1.0/openrl/algorithms/base_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,17 @@
         self.tpdv = dict(dtype=torch.float32, device=device)
 
         self.algo_module = init_module
 
         self.world_size = self.algo_module.world_size or 1
         self.clip_param = cfg.clip_param
         self.ppo_epoch = cfg.ppo_epoch
+        self.bc_epoch = cfg.bc_epoch
         self.num_mini_batch = cfg.num_mini_batch
+        self.mini_batch_size = cfg.mini_batch_size
         self.data_chunk_length = cfg.data_chunk_length
         self.policy_value_loss_coef = cfg.policy_value_loss_coef
         self.value_loss_coef = cfg.value_loss_coef
         self.entropy_coef = cfg.entropy_coef
         self.max_grad_norm = cfg.max_grad_norm
         self.huber_delta = cfg.huber_delta
```

### Comparing `openrl-0.0.9/openrl/algorithms/ppo.py` & `openrl-0.1.0/openrl/algorithms/ppo.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.nn.parallel import DistributedDataParallel
 
 from openrl.algorithms.base_algorithm import BaseAlgorithm
 from openrl.modules.networks.utils.distributed_utils import reduce_tensor
-from openrl.modules.utils.util import get_gard_norm, huber_loss, mse_loss
+from openrl.modules.utils.util import get_grad_norm, huber_loss, mse_loss
 from openrl.utils.util import check
 
 
 class PPOAlgorithm(BaseAlgorithm):
     def __init__(
         self,
         cfg,
         init_module,
         agent_num: int = 1,
         device: Union[str, torch.device] = "cpu",
     ) -> None:
         self._use_share_model = cfg.use_share_model
         self.use_joint_action_loss = cfg.use_joint_action_loss
         super(PPOAlgorithm, self).__init__(cfg, init_module, agent_num, device)
+        self.train_list = [self.train_ppo]
 
     def ppo_update(self, sample, turn_on=True):
         for optimizer in self.algo_module.optimizers.values():
             optimizer.zero_grad()
 
         (
             critic_obs_batch,
@@ -53,15 +54,15 @@
             actions_batch,
             value_preds_batch,
             return_batch,
             masks_batch,
             active_masks_batch,
             old_action_log_probs_batch,
             adv_targ,
-            available_actions_batch,
+            action_masks_batch,
         ) = sample
 
         old_action_log_probs_batch = check(old_action_log_probs_batch).to(**self.tpdv)
         adv_targ = check(adv_targ).to(**self.tpdv)
         value_preds_batch = check(value_preds_batch).to(**self.tpdv)
         return_batch = check(return_batch).to(**self.tpdv)
         active_masks_batch = check(active_masks_batch).to(**self.tpdv)
@@ -77,15 +78,15 @@
                 ) = self.prepare_loss(
                     critic_obs_batch,
                     obs_batch,
                     rnn_states_batch,
                     rnn_states_critic_batch,
                     actions_batch,
                     masks_batch,
-                    available_actions_batch,
+                    action_masks_batch,
                     old_action_log_probs_batch,
                     adv_targ,
                     value_preds_batch,
                     return_batch,
                     active_masks_batch,
                     turn_on,
                 )
@@ -95,62 +96,45 @@
             loss_list, value_loss, policy_loss, dist_entropy, ratio = self.prepare_loss(
                 critic_obs_batch,
                 obs_batch,
                 rnn_states_batch,
                 rnn_states_critic_batch,
                 actions_batch,
                 masks_batch,
-                available_actions_batch,
+                action_masks_batch,
                 old_action_log_probs_batch,
                 adv_targ,
                 value_preds_batch,
                 return_batch,
                 active_masks_batch,
                 turn_on,
             )
             for loss in loss_list:
                 loss.backward()
 
-        if "transformer" in self.algo_module.models:
-            if self._use_max_grad_norm:
-                grad_norm = nn.utils.clip_grad_norm_(
-                    self.algo_module.models["transformer"].parameters(),
-                    self.max_grad_norm,
-                )
-            else:
-                grad_norm = get_gard_norm(
-                    self.algo_module.models["transformer"].parameters()
-                )
-            critic_grad_norm = grad_norm
-            actor_grad_norm = grad_norm
-
+        # else:
+        if self._use_share_model:
+            actor_para = self.algo_module.models["model"].get_actor_para()
         else:
-            if self._use_share_model:
-                actor_para = self.algo_module.models["model"].get_actor_para()
-            else:
-                actor_para = self.algo_module.models["policy"].parameters()
+            actor_para = self.algo_module.models["policy"].parameters()
 
-            if self._use_max_grad_norm:
-                actor_grad_norm = nn.utils.clip_grad_norm_(
-                    actor_para, self.max_grad_norm
-                )
-            else:
-                actor_grad_norm = get_gard_norm(actor_para)
+        if self._use_max_grad_norm:
+            actor_grad_norm = nn.utils.clip_grad_norm_(actor_para, self.max_grad_norm)
+        else:
+            actor_grad_norm = get_grad_norm(actor_para)
 
-            if self._use_share_model:
-                critic_para = self.algo_module.models["model"].get_critic_para()
-            else:
-                critic_para = self.algo_module.models["critic"].parameters()
+        if self._use_share_model:
+            critic_para = self.algo_module.models["model"].get_critic_para()
+        else:
+            critic_para = self.algo_module.models["critic"].parameters()
 
-            if self._use_max_grad_norm:
-                critic_grad_norm = nn.utils.clip_grad_norm_(
-                    critic_para, self.max_grad_norm
-                )
-            else:
-                critic_grad_norm = get_gard_norm(critic_para)
+        if self._use_max_grad_norm:
+            critic_grad_norm = nn.utils.clip_grad_norm_(critic_para, self.max_grad_norm)
+        else:
+            critic_grad_norm = get_grad_norm(critic_para)
 
         if self.use_amp:
             for optimizer in self.algo_module.optimizers.values():
                 self.algo_module.scaler.unscale_(optimizer)
 
             for optimizer in self.algo_module.optimizers.values():
                 self.algo_module.scaler.step(optimizer)
@@ -215,32 +199,40 @@
 
         return value_loss
 
     def to_single_np(self, input):
         reshape_input = input.reshape(-1, self.agent_num, *input.shape[1:])
         return reshape_input[:, 0, ...]
 
+    def construct_loss_list(self, policy_loss, dist_entropy, value_loss, turn_on):
+        loss_list = []
+        if turn_on:
+            final_p_loss = policy_loss - dist_entropy * self.entropy_coef
+
+            loss_list.append(final_p_loss)
+        final_v_loss = value_loss * self.value_loss_coef
+        loss_list.append(final_v_loss)
+        return loss_list
+
     def prepare_loss(
         self,
         critic_obs_batch,
         obs_batch,
         rnn_states_batch,
         rnn_states_critic_batch,
         actions_batch,
         masks_batch,
-        available_actions_batch,
+        action_masks_batch,
         old_action_log_probs_batch,
         adv_targ,
         value_preds_batch,
         return_batch,
         active_masks_batch,
         turn_on,
     ):
-        loss_list = []
-
         if self.use_joint_action_loss:
             critic_obs_batch = self.to_single_np(critic_obs_batch)
             rnn_states_critic_batch = self.to_single_np(rnn_states_critic_batch)
             critic_masks_batch = self.to_single_np(masks_batch)
             value_preds_batch = self.to_single_np(value_preds_batch)
             return_batch = self.to_single_np(return_batch)
             adv_targ = adv_targ.reshape(-1, self.agent_num, 1)
@@ -257,15 +249,15 @@
         ) = self.algo_module.evaluate_actions(
             critic_obs_batch,
             obs_batch,
             rnn_states_batch,
             rnn_states_critic_batch,
             actions_batch,
             masks_batch,
-            available_actions_batch,
+            action_masks_batch,
             active_masks_batch,
             critic_masks_batch=critic_masks_batch,
         )
 
         if self.use_joint_action_loss:
             action_log_probs_copy = (
                 action_log_probs.reshape(-1, self.agent_num, action_log_probs.shape[-1])
@@ -337,31 +329,40 @@
             value_normalizer,
             values,
             value_preds_batch,
             return_batch,
             active_masks_batch,
         )
 
-        if "transformer" in self.algo_module.models:
-            loss = (
-                policy_loss
-                - dist_entropy * self.entropy_coef
-                + value_loss * self.value_loss_coef
+        loss_list = self.construct_loss_list(
+            policy_loss, dist_entropy, value_loss, turn_on
+        )
+        return loss_list, value_loss, policy_loss, dist_entropy, ratio
+
+    def get_data_generator(self, buffer, advantages):
+        if self._use_recurrent_policy:
+            if self.use_joint_action_loss:
+                data_generator = buffer.recurrent_generator_v3(
+                    advantages, self.num_mini_batch, self.data_chunk_length
+                )
+            else:
+                data_generator = buffer.recurrent_generator(
+                    advantages, self.num_mini_batch, self.data_chunk_length
+                )
+        elif self._use_naive_recurrent:
+            data_generator = buffer.naive_recurrent_generator(
+                advantages, self.num_mini_batch
             )
-            loss_list.append(loss)
         else:
-            if turn_on:
-                final_p_loss = policy_loss - dist_entropy * self.entropy_coef
-
-                loss_list.append(final_p_loss)
-            final_v_loss = value_loss * self.value_loss_coef
-            loss_list.append(final_v_loss)
-        return loss_list, value_loss, policy_loss, dist_entropy, ratio
+            data_generator = buffer.feed_forward_generator(
+                advantages, self.num_mini_batch
+            )
+        return data_generator
 
-    def train(self, buffer, turn_on=True):
+    def train_ppo(self, buffer, turn_on):
         if self._use_popart or self._use_valuenorm:
             if self._use_share_model:
                 value_normalizer = self.algo_module.models["model"].value_normalizer
             elif isinstance(self.algo_module.models["critic"], DistributedDataParallel):
                 value_normalizer = self.algo_module.models[
                     "critic"
                 ].module.value_normalizer
@@ -392,35 +393,15 @@
         train_info["critic_grad_norm"] = 0
         train_info["ratio"] = 0
         if self.world_size > 1:
             train_info["reduced_value_loss"] = 0
             train_info["reduced_policy_loss"] = 0
 
         for _ in range(self.ppo_epoch):
-            if "transformer" in self.algo_module.models:
-                data_generator = buffer.feed_forward_generator_transformer(
-                    advantages, self.num_mini_batch
-                )
-            elif self._use_recurrent_policy:
-                if self.use_joint_action_loss:
-                    data_generator = buffer.recurrent_generator_v3(
-                        advantages, self.num_mini_batch, self.data_chunk_length
-                    )
-                else:
-                    data_generator = buffer.recurrent_generator(
-                        advantages, self.num_mini_batch, self.data_chunk_length
-                    )
-            elif self._use_naive_recurrent:
-                data_generator = buffer.naive_recurrent_generator(
-                    advantages, self.num_mini_batch
-                )
-            else:
-                data_generator = buffer.feed_forward_generator(
-                    advantages, self.num_mini_batch
-                )
+            data_generator = self.get_data_generator(buffer, advantages)
 
             for sample in data_generator:
                 (
                     value_loss,
                     critic_grad_norm,
                     policy_loss,
                     dist_entropy,
@@ -445,12 +426,19 @@
                 train_info["ratio"] += ratio.mean().item()
 
         num_updates = self.ppo_epoch * self.num_mini_batch
 
         for k in train_info.keys():
             train_info[k] /= num_updates
 
+        return train_info
+
+    def train(self, buffer, turn_on=True):
+        train_info = {}
+        for train_func in self.train_list:
+            train_info.update(train_func(buffer, turn_on))
+
         for optimizer in self.algo_module.optimizers.values():
             if hasattr(optimizer, "sync_lookahead"):
                 optimizer.sync_lookahead()
 
         return train_info
```

### Comparing `openrl-0.0.9/openrl/buffers/__init__.py` & `openrl-0.1.0/openrl/selfplay/callbacks/base_callback.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# Copyright 2021 The OpenRL Authors.
+# Copyright 2023 The OpenRL Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,12 +12,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-from .normal_buffer import NormalReplayBuffer
 
-__all__ = [
-    "NormalReplayBuffer",
-]
+from openrl.utils.callbacks.callbacks import BaseCallback
+
+
+class BaseSelfplayCallback(BaseCallback):
+    pass
```

### Comparing `openrl-0.0.9/openrl/buffers/normal_buffer.py` & `openrl-0.1.0/openrl/buffers/normal_buffer.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,43 +30,43 @@
             num_agents,
             obs_space,
             act_space,
             data_client,
             episode_length,
         )
 
-    def init_buffer(self, raw_obs, available_actions=None):
-        self.data.init_buffer(raw_obs, available_actions)
+    def init_buffer(self, raw_obs, action_masks=None):
+        self.data.init_buffer(raw_obs, action_masks)
 
     def insert(
         self,
         raw_obs,
         rnn_states,
         rnn_states_critic,
         actions,
         action_log_probs,
         value_preds,
         rewards,
         masks,
         bad_masks=None,
         active_masks=None,
-        available_actions=None,
+        action_masks=None,
     ):
         self.data.insert(
             raw_obs,
             rnn_states,
             rnn_states_critic,
             actions,
             action_log_probs,
             value_preds,
             rewards,
             masks,
             bad_masks,
             active_masks,
-            available_actions,
+            action_masks,
         )
 
     def after_update(self):
         self.data.after_update()
 
     def compute_returns(self, next_value, value_normalizer=None):
         self.data.compute_returns(next_value, value_normalizer)
```

### Comparing `openrl-0.0.9/openrl/buffers/replay_data.py` & `openrl-0.1.0/openrl/buffers/replay_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,25 +142,25 @@
         self.value_preds = np.zeros(
             (self.episode_length + 1, self.n_rollout_threads, num_agents, 1),
             dtype=np.float32,
         )
         self.returns = np.zeros_like(self.value_preds)
 
         if act_space.__class__.__name__ == "Discrete":
-            self.available_actions = np.ones(
+            self.action_masks = np.ones(
                 (
                     self.episode_length + 1,
                     self.n_rollout_threads,
                     num_agents,
                     act_space.n,
                 ),
                 dtype=np.float32,
             )
         else:
-            self.available_actions = None
+            self.action_masks = None
 
         act_shape = get_shape_from_act_space(act_space)
 
         self.actions = np.zeros(
             (self.episode_length, self.n_rollout_threads, num_agents, act_shape),
             dtype=np.float32,
         )
@@ -186,14 +186,16 @@
     def get_batch_data(
         self,
         data_name: str,
         step: int,
     ):
         assert hasattr(self, data_name)
         data = getattr(self, data_name)
+        if data is None:
+            return None
 
         if isinstance(data, ObsData):
             return data.step_batch(step)
         else:
             return np.concatenate(data[step])
 
     def all_batch_data(self, data_name: str, min=None, max=None):
@@ -231,16 +233,16 @@
         if "masks" in data:
             self.masks[self.step + 1] = data["masks"].copy()
 
         if "bad_masks" in data:
             self.bad_masks[self.step + 1] = data["bad_masks"].copy()
         if "active_masks" in data:
             self.active_masks[self.step + 1] = data["active_masks"].copy()
-        if "available_actions" in data:
-            self.available_actions[self.step + 1] = data["available_actions"].copy()
+        if "action_masks" in data:
+            self.action_masks[self.step + 1] = data["action_masks"].copy()
 
         self.step = (self.step + 1) % self.episode_length
 
     def insert(
         self,
         raw_obs,
         rnn_states,
@@ -248,55 +250,56 @@
         actions,
         action_log_probs,
         value_preds,
         rewards,
         masks,
         bad_masks=None,
         active_masks=None,
-        available_actions=None,
+        action_masks=None,
     ):
         critic_obs = get_critic_obs(raw_obs)
         policy_obs = get_policy_obs(raw_obs)
         if self._mixed_obs:
             for key in self.critic_obs.keys():
                 self.critic_obs[key][self.step + 1] = critic_obs[key].copy()
             for key in self.policy_obs.keys():
                 self.policy_obs[key][self.step + 1] = policy_obs[key].copy()
         else:
             self.critic_obs[self.step + 1] = critic_obs.copy()
             self.policy_obs[self.step + 1] = policy_obs.copy()
-
-        self.rnn_states[self.step + 1] = rnn_states.copy()
-        self.rnn_states_critic[self.step + 1] = rnn_states_critic.copy()
+        if rnn_states is not None:
+            self.rnn_states[self.step + 1] = rnn_states.copy()
+        if rnn_states_critic is not None:
+            self.rnn_states_critic[self.step + 1] = rnn_states_critic.copy()
         self.actions[self.step] = actions.copy()
         self.action_log_probs[self.step] = action_log_probs.copy()
         self.value_preds[self.step] = value_preds.copy()
         self.rewards[self.step] = rewards.copy()
         self.masks[self.step + 1] = masks.copy()
         if bad_masks is not None:
             self.bad_masks[self.step + 1] = bad_masks.copy()
         if active_masks is not None:
             self.active_masks[self.step + 1] = active_masks.copy()
-        if available_actions is not None:
-            self.available_actions[self.step + 1] = available_actions.copy()
+        if action_masks is not None:
+            self.action_masks[self.step + 1] = action_masks.copy()
         self.step = (self.step + 1) % self.episode_length
 
-    def init_buffer(self, raw_obs, available_actions=None):
+    def init_buffer(self, raw_obs, action_masks=None):
         critic_obs = get_critic_obs(raw_obs)
         policy_obs = get_policy_obs(raw_obs)
         if self._mixed_obs:
             for key in self.critic_obs.keys():
                 self.critic_obs[key][0] = critic_obs[key].copy()
             for key in self.policy_obs.keys():
                 self.policy_obs[key][0] = policy_obs[key].copy()
         else:
             self.critic_obs[0] = critic_obs.copy()
             self.policy_obs[0] = policy_obs.copy()
-        if available_actions is not None and self.available_actions is not None:
-            self.available_actions[0] = available_actions
+        if action_masks is not None and self.action_masks is not None:
+            self.action_masks[0] = action_masks
 
     def after_update(self):
         assert self.step == 0, "step:{} episode:{}".format(
             self.step, self.episode_length
         )
         if self._mixed_obs:
             for key in self.critic_obs.keys():
@@ -307,16 +310,16 @@
             self.critic_obs[0] = self.critic_obs[-1].copy()
             self.policy_obs[0] = self.policy_obs[-1].copy()
         self.rnn_states[0] = self.rnn_states[-1].copy()
         self.rnn_states_critic[0] = self.rnn_states_critic[-1].copy()
         self.masks[0] = self.masks[-1].copy()
         self.bad_masks[0] = self.bad_masks[-1].copy()
         self.active_masks[0] = self.active_masks[-1].copy()
-        if self.available_actions is not None:
-            self.available_actions[0] = self.available_actions[-1].copy()
+        if self.action_masks is not None:
+            self.action_masks[0] = self.action_masks[-1].copy()
 
     def compute_returns(self, next_value, value_normalizer=None):
         if self._use_proper_time_limits:
             if self._use_gae:
                 self.value_preds[-1] = next_value
                 gae = 0
                 for step in reversed(range(self.rewards.shape[0])):
@@ -373,15 +376,17 @@
                             step
                         ]
         else:
             if self._use_gae:
                 self.value_preds[-1] = next_value
                 gae = 0
                 for step in reversed(range(self.rewards.shape[0])):
-                    if self._use_popart or self._use_valuenorm:
+                    if (
+                        self._use_popart or self._use_valuenorm
+                    ) and value_normalizer is not None:
                         delta = (
                             self.rewards[step]
                             + self.gamma
                             * value_normalizer.denormalize(self.value_preds[step + 1])
                             * self.masks[step + 1]
                             - value_normalizer.denormalize(self.value_preds[step])
                         )
@@ -419,15 +424,15 @@
         data_chunks = batch_size // data_chunk_length  # [C=r*T*M/L]
         mini_batch_size = data_chunks // num_mini_batch
 
         assert n_rollout_threads * episode_length >= data_chunk_length, (
             "PPO requires the nfumber of processes ({}) * episode length ({}) "
             "to be greater than or equal to the number of "
             "data chunk length ({}).".format(
-                n_rollout_threads, num_agents, episode_length, data_chunk_length
+                n_rollout_threads, episode_length, data_chunk_length
             )
         )
 
         rand = torch.randperm(data_chunks).numpy()
         sampler = [
             rand[i * mini_batch_size : (i + 1) * mini_batch_size]
             for i in range(num_mini_batch)
@@ -451,25 +456,25 @@
         )
         rnn_states_critic = (
             self.rnn_states_critic[:-1]
             .transpose(1, 0, 2, 3, 4)
             .reshape(-1, *self.rnn_states_critic.shape[2:])
         )
 
-        if self.available_actions is not None:
-            available_actions = _cast_v3(self.available_actions[:-1])
+        if self.action_masks is not None:
+            action_masks = _cast_v3(self.action_masks[:-1])
 
         for indices in sampler:
             critic_obs_batch = []
             policy_obs_batch = []
 
             rnn_states_batch = []
             rnn_states_critic_batch = []
             actions_batch = []
-            available_actions_batch = []
+            action_masks_batch = []
             value_preds_batch = []
             return_batch = []
             masks_batch = []
             active_masks_batch = []
             old_action_log_probs_batch = []
             adv_targ = []
 
@@ -477,17 +482,17 @@
                 ind = index * data_chunk_length
                 # size [T+1 N M Dim]-->[T N M Dim]-->[N,M,T,Dim]-->[N*M*T,Dim]-->[L,Dim]
                 # [L, agent_num, Dim]
                 critic_obs_batch.append(critic_obs[ind : ind + data_chunk_length])
                 policy_obs_batch.append(policy_obs[ind : ind + data_chunk_length])
 
                 actions_batch.append(actions[ind : ind + data_chunk_length])
-                if self.available_actions is not None:
-                    available_actions_batch.append(
-                        available_actions[ind : ind + data_chunk_length]
+                if self.action_masks is not None:
+                    action_masks_batch.append(
+                        action_masks[ind : ind + data_chunk_length]
                     )
                 value_preds_batch.append(value_preds[ind : ind + data_chunk_length])
                 return_batch.append(returns[ind : ind + data_chunk_length])
                 masks_batch.append(masks[ind : ind + data_chunk_length])
                 active_masks_batch.append(active_masks[ind : ind + data_chunk_length])
                 old_action_log_probs_batch.append(
                     action_log_probs[ind : ind + data_chunk_length]
@@ -502,16 +507,16 @@
 
             # These are all from_numpys of size (L, N, agent_num, Dim)
 
             critic_obs_batch = np.stack(critic_obs_batch, axis=1)
             policy_obs_batch = np.stack(policy_obs_batch, axis=1)
 
             actions_batch = np.stack(actions_batch, axis=1)
-            if self.available_actions is not None:
-                available_actions_batch = np.stack(available_actions_batch, axis=1)
+            if self.action_masks is not None:
+                action_masks_batch = np.stack(action_masks_batch, axis=1)
             value_preds_batch = np.stack(value_preds_batch, axis=1)
             return_batch = np.stack(return_batch, axis=1)
             masks_batch = np.stack(masks_batch, axis=1)
             active_masks_batch = np.stack(active_masks_batch, axis=1)
             old_action_log_probs_batch = np.stack(old_action_log_probs_batch, axis=1)
             adv_targ = np.stack(adv_targ, axis=1)
 
@@ -523,29 +528,27 @@
                 N * num_agents, *self.rnn_states_critic.shape[3:]
             )
             # Flatten the (L, N, ...) from_numpys to (L * N, ...)
 
             critic_obs_batch = _flatten_v3(L, N, num_agents, critic_obs_batch)
             policy_obs_batch = _flatten_v3(L, N, num_agents, policy_obs_batch)
             actions_batch = _flatten_v3(L, N, num_agents, actions_batch)
-            if self.available_actions is not None:
-                available_actions_batch = _flatten_v3(
-                    L, N, num_agents, available_actions_batch
-                )
+            if self.action_masks is not None:
+                action_masks_batch = _flatten_v3(L, N, num_agents, action_masks_batch)
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = _flatten_v3(L, N, num_agents, value_preds_batch)
             return_batch = _flatten_v3(L, N, num_agents, return_batch)
             masks_batch = _flatten_v3(L, N, num_agents, masks_batch)
             active_masks_batch = _flatten_v3(L, N, num_agents, active_masks_batch)
             old_action_log_probs_batch = _flatten_v3(
                 L, N, num_agents, old_action_log_probs_batch
             )
             adv_targ = _flatten_v3(L, N, num_agents, adv_targ)
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
 
     def feed_forward_generator(
         self,
         advantages,
         num_mini_batch=None,
         mini_batch_size=None,
         critic_obs_process_func=None,
@@ -589,17 +592,17 @@
             critic_obs = self.critic_obs[:-1].reshape(-1, *self.critic_obs.shape[3:])
             policy_obs = self.policy_obs[:-1].reshape(-1, *self.policy_obs.shape[3:])
         rnn_states = self.rnn_states[:-1].reshape(-1, *self.rnn_states.shape[3:])
         rnn_states_critic = self.rnn_states_critic[:-1].reshape(
             -1, *self.rnn_states_critic.shape[3:]
         )
         actions = self.actions.reshape(-1, self.actions.shape[-1])
-        if self.available_actions is not None:
-            available_actions = self.available_actions[:-1].reshape(
-                -1, self.available_actions.shape[-1]
+        if self.action_masks is not None:
+            action_masks = self.action_masks[:-1].reshape(
+                -1, self.action_masks.shape[-1]
             )
         value_preds = self.value_preds[:-1].reshape(-1, 1)
         returns = self.returns[:-1].reshape(-1, 1)
         masks = self.masks[:-1].reshape(-1, 1)
         active_masks = self.active_masks[:-1].reshape(-1, 1)
         action_log_probs = self.action_log_probs.reshape(
             -1, self.action_log_probs.shape[-1]
@@ -618,31 +621,31 @@
                     policy_obs_batch[key] = policy_obs[key][indices]
             else:
                 critic_obs_batch = critic_obs[indices]
                 policy_obs_batch = policy_obs[indices]
             rnn_states_batch = rnn_states[indices]
             rnn_states_critic_batch = rnn_states_critic[indices]
             actions_batch = actions[indices]
-            if self.available_actions is not None:
-                available_actions_batch = available_actions[indices]
+            if self.action_masks is not None:
+                action_masks_batch = action_masks[indices]
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = value_preds[indices]
             return_batch = returns[indices]
             masks_batch = masks[indices]
             active_masks_batch = active_masks[indices]
             old_action_log_probs_batch = action_log_probs[indices]
             if advantages is None:
                 adv_targ = None
             else:
                 adv_targ = advantages[indices]
             if critic_obs_process_func is not None:
                 critic_obs_batch = critic_obs_process_func(critic_obs_batch)
 
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
 
     def feed_forward_critic_obs_generator(
         self,
         advantages,
         num_mini_batch=None,
         mini_batch_size=None,
         critic_obs_process_func=None,
@@ -747,19 +750,19 @@
             -1, *self.rnn_states_critic.shape[2:]
         )
         rnn_states_critic = rnn_states_critic[rows, cols]
         actions = self.actions.reshape(-1, *self.actions.shape[2:])
 
         actions = actions[rows, cols]
 
-        if self.available_actions is not None:
-            available_actions = self.available_actions[:-1].reshape(
-                -1, *self.available_actions.shape[2:]
+        if self.action_masks is not None:
+            action_masks = self.action_masks[:-1].reshape(
+                -1, *self.action_masks.shape[2:]
             )
-            available_actions = available_actions[rows, cols]
+            action_masks = action_masks[rows, cols]
         value_preds = self.value_preds[:-1].reshape(-1, *self.value_preds.shape[2:])
         value_preds = value_preds[rows, cols]
         returns = self.returns[:-1].reshape(-1, *self.returns.shape[2:])
         returns = returns[rows, cols]
         masks = self.masks[:-1].reshape(-1, *self.masks.shape[2:])
         masks = masks[rows, cols]
         active_masks = self.active_masks[:-1].reshape(-1, *self.active_masks.shape[2:])
@@ -776,35 +779,35 @@
             critic_obs_batch = critic_obs[indices].reshape(-1, *critic_obs.shape[2:])
             policy_obs_batch = policy_obs[indices].reshape(-1, *policy_obs.shape[2:])
             rnn_states_batch = rnn_states[indices].reshape(-1, *rnn_states.shape[2:])
             rnn_states_critic_batch = rnn_states_critic[indices].reshape(
                 -1, *rnn_states_critic.shape[2:]
             )
             actions_batch = actions[indices].reshape(-1, *actions.shape[2:])
-            if self.available_actions is not None:
-                available_actions_batch = available_actions[indices].reshape(
-                    -1, *available_actions.shape[2:]
+            if self.action_masks is not None:
+                action_masks_batch = action_masks[indices].reshape(
+                    -1, *action_masks.shape[2:]
                 )
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = value_preds[indices].reshape(-1, *value_preds.shape[2:])
             return_batch = returns[indices].reshape(-1, *returns.shape[2:])
             masks_batch = masks[indices].reshape(-1, *masks.shape[2:])
             active_masks_batch = active_masks[indices].reshape(
                 -1, *active_masks.shape[2:]
             )
             old_action_log_probs_batch = action_log_probs[indices].reshape(
                 -1, *action_log_probs.shape[2:]
             )
             if advantages is None:
                 adv_targ = None
             else:
                 adv_targ = advantages[indices].reshape(-1, *advantages.shape[2:])
 
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
 
     def naive_recurrent_generator(self, advantages, num_mini_batch):
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * num_agents
         assert n_rollout_threads * num_agents >= num_mini_batch, (
             "PPO requires the number of processes ({})* number of agents ({}) "
             "to be greater than or equal to the number of "
@@ -834,17 +837,17 @@
                 -1, batch_size, *self.policy_obs.shape[3:]
             )
         rnn_states = self.rnn_states.reshape(-1, batch_size, *self.rnn_states.shape[3:])
         rnn_states_critic = self.rnn_states_critic.reshape(
             -1, batch_size, *self.rnn_states_critic.shape[3:]
         )
         actions = self.actions.reshape(-1, batch_size, self.actions.shape[-1])
-        if self.available_actions is not None:
-            available_actions = self.available_actions.reshape(
-                -1, batch_size, self.available_actions.shape[-1]
+        if self.action_masks is not None:
+            action_masks = self.action_masks.reshape(
+                -1, batch_size, self.action_masks.shape[-1]
             )
         value_preds = self.value_preds.reshape(-1, batch_size, 1)
         returns = self.returns.reshape(-1, batch_size, 1)
         masks = self.masks.reshape(-1, batch_size, 1)
         active_masks = self.active_masks.reshape(-1, batch_size, 1)
         action_log_probs = self.action_log_probs.reshape(
             -1, batch_size, self.action_log_probs.shape[-1]
@@ -858,15 +861,15 @@
             else:
                 critic_obs_batch = []
                 policy_obs_batch = []
 
             rnn_states_batch = []
             rnn_states_critic_batch = []
             actions_batch = []
-            available_actions_batch = []
+            action_masks_batch = []
             value_preds_batch = []
             return_batch = []
             masks_batch = []
             active_masks_batch = []
             old_action_log_probs_batch = []
             adv_targ = []
 
@@ -879,16 +882,16 @@
                         policy_obs_batch[key].append(policy_obs[key][:-1, ind])
                 else:
                     critic_obs_batch.append(critic_obs[:-1, ind])
                     policy_obs_batch.append(policy_obs[:-1, ind])
                 rnn_states_batch.append(rnn_states[0:1, ind])
                 rnn_states_critic_batch.append(rnn_states_critic[0:1, ind])
                 actions_batch.append(actions[:, ind])
-                if self.available_actions is not None:
-                    available_actions_batch.append(available_actions[:-1, ind])
+                if self.action_masks is not None:
+                    action_masks_batch.append(action_masks[:-1, ind])
                 value_preds_batch.append(value_preds[:-1, ind])
                 return_batch.append(returns[:-1, ind])
                 masks_batch.append(masks[:-1, ind])
                 active_masks_batch.append(active_masks[:-1, ind])
                 old_action_log_probs_batch.append(action_log_probs[:, ind])
                 adv_targ.append(advantages[:, ind])
 
@@ -900,16 +903,16 @@
                     critic_obs_batch[key] = np.stack(critic_obs_batch[key], 1)
                 for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = np.stack(policy_obs_batch[key], 1)
             else:
                 critic_obs_batch = np.stack(critic_obs_batch, 1)
                 policy_obs_batch = np.stack(policy_obs_batch, 1)
             actions_batch = np.stack(actions_batch, 1)
-            if self.available_actions is not None:
-                available_actions_batch = np.stack(available_actions_batch, 1)
+            if self.action_masks is not None:
+                action_masks_batch = np.stack(action_masks_batch, 1)
             value_preds_batch = np.stack(value_preds_batch, 1)
             return_batch = np.stack(return_batch, 1)
             masks_batch = np.stack(masks_batch, 1)
             active_masks_batch = np.stack(active_masks_batch, 1)
             old_action_log_probs_batch = np.stack(old_action_log_probs_batch, 1)
             adv_targ = np.stack(adv_targ, 1)
 
@@ -927,26 +930,26 @@
                     critic_obs_batch[key] = _flatten(T, N, critic_obs_batch[key])
                 for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = _flatten(T, N, policy_obs_batch[key])
             else:
                 critic_obs_batch = _flatten(T, N, critic_obs_batch)
                 policy_obs_batch = _flatten(T, N, policy_obs_batch)
             actions_batch = _flatten(T, N, actions_batch)
-            if self.available_actions is not None:
-                available_actions_batch = _flatten(T, N, available_actions_batch)
+            if self.action_masks is not None:
+                action_masks_batch = _flatten(T, N, action_masks_batch)
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = _flatten(T, N, value_preds_batch)
             return_batch = _flatten(T, N, return_batch)
             masks_batch = _flatten(T, N, masks_batch)
             active_masks_batch = _flatten(T, N, active_masks_batch)
             old_action_log_probs_batch = _flatten(T, N, old_action_log_probs_batch)
             adv_targ = _flatten(T, N, adv_targ)
 
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
 
     def recurrent_generator_v2(
         self, advantages, num_mini_batch=None, mini_batch_size=None
     ):
         """
         Yield training data for MLP policies.
         :param advantages: (np.ndarray) advantage estimates.
@@ -987,17 +990,17 @@
 
         rnn_states_critic = self.rnn_states_critic[:-1].reshape(
             -1, *self.rnn_states_critic.shape[2:]
         )
 
         actions = self.actions.reshape(-1, *self.actions.shape[2:])
 
-        if self.available_actions is not None:
-            available_actions = self.available_actions[:-1].reshape(
-                -1, *self.available_actions.shape[2:]
+        if self.action_masks is not None:
+            action_masks = self.action_masks[:-1].reshape(
+                -1, *self.action_masks.shape[2:]
             )
 
         value_preds = self.value_preds[:-1].reshape(-1, *self.value_preds.shape[2:])
 
         returns = self.returns[:-1].reshape(-1, *self.returns.shape[2:])
 
         masks = self.masks[:-1].reshape(-1, *self.masks.shape[2:])
@@ -1010,16 +1013,16 @@
 
         advantages = advantages.reshape(-1, *advantages.shape[2:])
 
         shuffle = False
         if shuffle:
             rows, cols = _shuffle_agent_grid(batch_size, num_agents)
 
-            if self.available_actions is not None:
-                available_actions = available_actions[rows, cols]
+            if self.action_masks is not None:
+                action_masks = action_masks[rows, cols]
             critic_obs = critic_obs[rows, cols]
             policy_obs = policy_obs[rows, cols]
             rnn_states = rnn_states[rows, cols]
             rnn_states_critic = rnn_states_critic[rows, cols]
             actions = actions[rows, cols]
             value_preds = value_preds[rows, cols]
             returns = returns[rows, cols]
@@ -1033,39 +1036,40 @@
             critic_obs_batch = critic_obs[indices].reshape(-1, *critic_obs.shape[2:])
             policy_obs_batch = policy_obs[indices].reshape(-1, *policy_obs.shape[2:])
             rnn_states_batch = rnn_states[indices].reshape(-1, *rnn_states.shape[2:])
             rnn_states_critic_batch = rnn_states_critic[indices].reshape(
                 -1, *rnn_states_critic.shape[2:]
             )
             actions_batch = actions[indices].reshape(-1, *actions.shape[2:])
-            if self.available_actions is not None:
-                available_actions_batch = available_actions[indices].reshape(
-                    -1, *available_actions.shape[2:]
+            if self.action_masks is not None:
+                action_masks_batch = action_masks[indices].reshape(
+                    -1, *action_masks.shape[2:]
                 )
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = value_preds[indices].reshape(-1, *value_preds.shape[2:])
             return_batch = returns[indices].reshape(-1, *returns.shape[2:])
             masks_batch = masks[indices].reshape(-1, *masks.shape[2:])
             active_masks_batch = active_masks[indices].reshape(
                 -1, *active_masks.shape[2:]
             )
             old_action_log_probs_batch = action_log_probs[indices].reshape(
                 -1, *action_log_probs.shape[2:]
             )
             if advantages is None:
                 adv_targ = None
             else:
                 adv_targ = advantages[indices].reshape(-1, *advantages.shape[2:])
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
 
     def recurrent_generator(self, advantages, num_mini_batch, data_chunk_length):
         episode_length, n_rollout_threads, num_agents = self.rewards.shape[0:3]
         batch_size = n_rollout_threads * episode_length * num_agents
         data_chunks = batch_size // data_chunk_length  # [C=r*T*M/L]
+
         mini_batch_size = data_chunks // num_mini_batch
 
         assert n_rollout_threads * episode_length * num_agents >= data_chunk_length, (
             "PPO requires the number of processes ({})* number of agents ({}) * episode"
             " length ({}) to be greater than or equal to the number of data chunk"
             " length ({}).".format(
                 n_rollout_threads, num_agents, episode_length, data_chunk_length
@@ -1143,29 +1147,29 @@
         )
         rnn_states_critic = (
             self.rnn_states_critic[:-1]
             .transpose(1, 2, 0, 3, 4)
             .reshape(-1, *self.rnn_states_critic.shape[3:])
         )
 
-        if self.available_actions is not None:
-            available_actions = _cast(self.available_actions[:-1])
+        if self.action_masks is not None:
+            action_masks = _cast(self.action_masks[:-1])
 
         for indices in sampler:
             if self._mixed_obs:
                 critic_obs_batch = defaultdict(list)
                 policy_obs_batch = defaultdict(list)
             else:
                 critic_obs_batch = []
                 policy_obs_batch = []
 
             rnn_states_batch = []
             rnn_states_critic_batch = []
             actions_batch = []
-            available_actions_batch = []
+            action_masks_batch = []
             value_preds_batch = []
             return_batch = []
             masks_batch = []
             active_masks_batch = []
             old_action_log_probs_batch = []
             adv_targ = []
 
@@ -1182,17 +1186,17 @@
                             policy_obs[key][ind : ind + data_chunk_length]
                         )
                 else:
                     critic_obs_batch.append(critic_obs[ind : ind + data_chunk_length])
                     policy_obs_batch.append(policy_obs[ind : ind + data_chunk_length])
 
                 actions_batch.append(actions[ind : ind + data_chunk_length])
-                if self.available_actions is not None:
-                    available_actions_batch.append(
-                        available_actions[ind : ind + data_chunk_length]
+                if self.action_masks is not None:
+                    action_masks_batch.append(
+                        action_masks[ind : ind + data_chunk_length]
                     )
                 value_preds_batch.append(value_preds[ind : ind + data_chunk_length])
                 return_batch.append(returns[ind : ind + data_chunk_length])
                 masks_batch.append(masks[ind : ind + data_chunk_length])
                 active_masks_batch.append(active_masks[ind : ind + data_chunk_length])
                 old_action_log_probs_batch.append(
                     action_log_probs[ind : ind + data_chunk_length]
@@ -1211,16 +1215,16 @@
                 for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = np.stack(policy_obs_batch[key], axis=1)
             else:
                 critic_obs_batch = np.stack(critic_obs_batch, axis=1)
                 policy_obs_batch = np.stack(policy_obs_batch, axis=1)
 
             actions_batch = np.stack(actions_batch, axis=1)
-            if self.available_actions is not None:
-                available_actions_batch = np.stack(available_actions_batch, axis=1)
+            if self.action_masks is not None:
+                action_masks_batch = np.stack(action_masks_batch, axis=1)
             value_preds_batch = np.stack(value_preds_batch, axis=1)
             return_batch = np.stack(return_batch, axis=1)
             masks_batch = np.stack(masks_batch, axis=1)
             active_masks_batch = np.stack(active_masks_batch, axis=1)
             old_action_log_probs_batch = np.stack(old_action_log_probs_batch, axis=1)
             adv_targ = np.stack(adv_targ, axis=1)
 
@@ -1238,19 +1242,19 @@
                     critic_obs_batch[key] = _flatten(L, N, critic_obs_batch[key])
                 for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = _flatten(L, N, policy_obs_batch[key])
             else:
                 critic_obs_batch = _flatten(L, N, critic_obs_batch)
                 policy_obs_batch = _flatten(L, N, policy_obs_batch)
             actions_batch = _flatten(L, N, actions_batch)
-            if self.available_actions is not None:
-                available_actions_batch = _flatten(L, N, available_actions_batch)
+            if self.action_masks is not None:
+                action_masks_batch = _flatten(L, N, action_masks_batch)
             else:
-                available_actions_batch = None
+                action_masks_batch = None
             value_preds_batch = _flatten(L, N, value_preds_batch)
             return_batch = _flatten(L, N, return_batch)
             masks_batch = _flatten(L, N, masks_batch)
             active_masks_batch = _flatten(L, N, active_masks_batch)
             old_action_log_probs_batch = _flatten(L, N, old_action_log_probs_batch)
             adv_targ = _flatten(L, N, adv_targ)
 
-            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, available_actions_batch
+            yield critic_obs_batch, policy_obs_batch, rnn_states_batch, rnn_states_critic_batch, actions_batch, value_preds_batch, return_batch, masks_batch, active_masks_batch, old_action_log_probs_batch, adv_targ, action_masks_batch
```

### Comparing `openrl-0.0.9/openrl/buffers/utils/__init__.py` & `openrl-0.1.0/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/buffers/utils/obs_data.py` & `openrl-0.1.0/openrl/buffers/utils/obs_data.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/buffers/utils/util.py` & `openrl-0.1.0/openrl/buffers/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,21 +52,22 @@
             return get_shape_from_obs_space_v2(obs_space, model_name="critic")
     return get_shape_from_obs_space_v2(obs_space)
 
 
 def get_shape_from_obs_space_v2(obs_space, model_name=None):
     if model_name is not None:
         obs_space = obs_space[model_name]
-
     if obs_space.__class__.__name__ == "Box":
         obs_shape = obs_space.shape
     elif obs_space.__class__.__name__ == "list":
         obs_shape = obs_space
     elif obs_space.__class__.__name__ == "Dict":
         obs_shape = obs_space.spaces
+    elif obs_space.__class__.__name__ == "Discrete":
+        obs_shape = (obs_space.n,)
     else:
         raise NotImplementedError(
             "obs_space type {} not supported".format(obs_space.__class__.__name__)
         )
     return obs_shape
```

### Comparing `openrl-0.0.9/openrl/cli/__init__.py` & `openrl-0.1.0/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/cli/cli.py` & `openrl-0.1.0/openrl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/cli/train.py` & `openrl-0.1.0/openrl/cli/train.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/configs/__init__.py` & `openrl-0.1.0/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/configs/config.py` & `openrl-0.1.0/openrl/configs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """"""
+from typing import List
+
 from jsonargparse import ActionConfigFile, ArgumentParser
 
+from openrl.configs.utils import ProcessYamlAction
+
 
 def create_config_parser():
     """
     The configuration parser.
     """
     parser = ArgumentParser(
         description="openrl",
     )
+    parser.add_argument("--config", action=ProcessYamlAction)
     parser.add_argument("--seed", type=int, default=0, help="Random seed.")
     # For Transformers
     parser.add_argument("--encode_state", action="store_true", default=False)
     parser.add_argument("--n_block", type=int, default=1)
     parser.add_argument("--n_embd", type=int, default=64)
     parser.add_argument("--n_head", type=int, default=1)
     parser.add_argument("--dec_actor", action="store_true", default=False)
     parser.add_argument("--share_actor", action="store_true", default=False)
+
+    parser.add_argument("--callbacks", type=List[dict])
+
     # For Hierarchical RL
     parser.add_argument(
         "--step_difference",
         type=int,
         default=1,
         help="Frequency difference between Controller's step and Executor's step",
     )
@@ -43,16 +51,17 @@
     parser.add_argument(
         "--gail",
         action="store_true",
         default=False,
         help="do imitation learning with gail",
     )
     parser.add_argument(
-        "--gail-experts-dir",
-        default="./gail_experts",
+        "--expert_data",
+        type=str,
+        default=None,
         help="directory that contains expert demonstrations for gail",
     )
     parser.add_argument(
         "--gail_batch_size",
         type=int,
         default=128,
         help="gail batch size (default: 128)",
@@ -66,18 +75,18 @@
         default=None,
         help="gail loss target at warm up",
     )
     parser.add_argument(
         "--gail_epoch", type=int, default=5, help="gail epochs (default: 5)"
     )
     parser.add_argument(
-        "--disable_action",
-        action="store_true",
-        default=False,
-        help="whether to use action as the input of the discriminator",
+        "--gail_use_action",
+        type=bool,
+        default=True,
+        help="whether to use action as the input of the gail discriminator",
     )
     parser.add_argument(
         "--gail_hidden_size",
         type=int,
         default=256,
         help="gail hidden state size (default: 256)",
     )
@@ -112,14 +121,35 @@
     )
     parser.add_argument("--worker_num", type=int, default=1, help="number of workers")
     parser.add_argument(
         "--sample_interval", type=int, default=1, help="data sample interval"
     )
     # For Self-Play
     parser.add_argument(
+        "--selfplay_api.host",
+        default="127.0.0.1",
+        type=str,
+        help="host for selfplay api",
+    )
+    parser.add_argument(
+        "--selfplay_api.port",
+        default=10086,
+        type=int,
+        help="port for selfplay api",
+    )
+    parser.add_argument(
+        "--lazy_load_opponent",
+        default=True,
+        type=bool,
+        help=(
+            "if true, when the opponents are the same opponent_type, will only load the"
+            " weight. Otherwise, will load the pythoon script."
+        ),
+    )
+    parser.add_argument(
         "--self_play",
         action="store_true",
         default=False,
         help="whether to use selfplay",
     )
     parser.add_argument(
         "--selfplay_algo",
@@ -456,15 +486,14 @@
         "--use_popart",
         action="store_true",
         default=False,
         help="by default False, use PopArt to normalize rewards.",
     )
     parser.add_argument(
         "--dual_clip_ppo",
-        action="store_true",
         default=False,
         help="by default False, use dual-clip ppo.",
     )
     parser.add_argument(
         "--dual_clip_coeff",
         type=float,
         default=3,
@@ -513,15 +542,15 @@
         choices=["gru", "lstm"],
         help="rnn types: gru or lstm",
     )
     parser.add_argument("--rnn_num", type=int, default=1, help="rnn layer number")
     # recurrent parameters
     parser.add_argument(
         "--use_naive_recurrent_policy",
-        action="store_true",
+        type=bool,
         default=False,
         help="Whether to use a naive recurrent policy",
     )
     parser.add_argument(
         "--use_recurrent_policy",
         type=bool,
         default=False,
@@ -529,15 +558,15 @@
     )
     parser.add_argument(
         "--recurrent_N", type=int, default=1, help="The number of recurrent layers."
     )
     parser.add_argument(
         "--data_chunk_length",
         type=int,
-        default=10,
+        default=2,
         help="Time length of chunks used to train a recurrent_policy",
     )
     parser.add_argument(
         "--use_influence_policy",
         action="store_true",
         default=False,
         help="use a recurrent policy",
@@ -609,14 +638,22 @@
         type=float,
         default=1e-5,
         help="RMSprop optimizer epsilon (default: 1e-5)",
     )
     parser.add_argument(
         "--weight_decay", type=float, default=0, help="weight decay (defaul: 0)"
     )
+    # behavior cloning parameters
+    parser.add_argument(
+        "--bc_epoch",
+        type=int,
+        default=2,
+        help="number of behavior cloning epochs (default: 15)",
+    )
+
     # ppo parameters
     parser.add_argument(
         "--ppo_epoch", type=int, default=10, help="number of ppo epochs (default: 15)"
     )
     parser.add_argument(
         "--use_policy_vhead",
         action="store_true",
@@ -638,14 +675,20 @@
     parser.add_argument(
         "--num_mini_batch",
         type=int,
         default=1,
         help="number of batches for ppo (default: 1)",
     )
     parser.add_argument(
+        "--mini_batch_size",
+        type=int,
+        default=None,
+        help="batch size (default: 1)",
+    )
+    parser.add_argument(
         "--policy_value_loss_coef",
         type=float,
         default=0.5,
         help="policy value loss coefficient (default: 0.5)",
     )
     parser.add_argument(
         "--entropy_coef",
@@ -699,15 +742,15 @@
         "--use_huber_loss",
         action="store_false",
         default=True,
         help="by default, use huber loss. If set, do not use huber loss.",
     )
     parser.add_argument(
         "--use_value_active_masks",
-        action="store_false",
+        type=bool,
         default=True,
         help="by default True, whether to mask useless data in value loss.",
     )
     parser.add_argument(
         "--use_policy_active_masks",
         action="store_false",
         default=True,
@@ -740,16 +783,16 @@
         action="store_true",
         default=False,
         help="share base network between policy network and value network",
     )
     # run parameters
     parser.add_argument(
         "--use_linear_lr_decay",
-        action="store_true",
         default=False,
+        type=bool,
         help="use a linear schedule on the learning rate",
     )
     # save parameters
     parser.add_argument(
         "--save_interval",
         type=int,
         default=1,
@@ -764,14 +807,20 @@
     # log parameters
     parser.add_argument(
         "--log_interval",
         type=int,
         default=5,
         help="time duration between contiunous twice log printing.",
     )
+    parser.add_argument(
+        "--use_rich_handler",
+        type=bool,
+        default=True,
+        help="whether to use rich handler to print log.",
+    )
     # eval parameters
     parser.add_argument(
         "--use_eval",
         action="store_true",
         default=False,
         help=(
             "by default, do not start evaluation. If set`, start evaluation alongside"
@@ -952,14 +1001,51 @@
     )
     parser.add_argument(
         "--prev_act_inp",
         action="store_true",
         default=False,
         help="Whether the actor input takes in previous actions as part of its input",
     )
+    parser.add_argument(
+        "--target_update",
+        type=int,
+        default=10,
+        help=(
+            "After how many evaluation network updates target network should be updated"
+        ),
+    )
+    # for DDPG
+    parser.add_argument(
+        "--var",
+        type=float,
+        default=0.5,
+        help="Control the exploration variance of the generated actions",
+    )
+    parser.add_argument(
+        "actor_lr", type=float, default=0.001, help="The learning rate of actor network"
+    )
+    # for SAC
+    parser.add_argument(
+        "auto_alph",
+        type=bool,
+        default=False,
+        help="whether to use automatic alpha tuning",
+    )
+    parser.add_argument(
+        "alpha_value",
+        type=float,
+        default=0.2,
+        help="The value of alpha",
+    )
+    parser.add_argument(
+        "alpha_lr",
+        type=float,
+        default=2e-4,
+        help="The learning rate of temperature alpha",
+    )
     # update parameters
     parser.add_argument(
         "--use_soft_update",
         action="store_false",
         default=True,
         help="Whether to use soft update",
     )
@@ -987,15 +1073,15 @@
         type=float,
         default=0.05,
         help="Ending value for epsilon, for eps-greedy exploration",
     )
     parser.add_argument(
         "--epsilon_anneal_time",
         type=int,
-        default=50000,
+        default=5000,
         help="Number of episodes until epsilon reaches epsilon_finish",
     )
     # qmix parameters
     parser.add_argument(
         "--use_double_q",
         action="store_false",
         default=True,
@@ -1045,15 +1131,15 @@
         "--model_path",
         default=None,
         type=str,
         help="the path of the model",
     )
     parser.add_argument(
         "--use_share_model",
-        action="store_true",
+        type=bool,
         default=False,
         help="use one class to implement policy and value networks",
     )
 
     # rewards class
     parser.add_argument(
         "--reward_class.id",
@@ -1086,9 +1172,47 @@
     parser.add_argument(
         "--eval_metrics",
         nargs="+",
         type=dict,
         default=[],
         help="the id of the vec env's info class",
     )
-    parser.add_argument("--config", action=ActionConfigFile)
+
+    # selfplay parameters
+    parser.add_argument(
+        "--disable_update_enemy",
+        default=False,
+        type=bool,
+        help="whether update enemy model",
+    )
+    parser.add_argument(
+        "--least_win_rate",
+        default=0.5,
+        type=float,
+        help="least_win_rate",
+    )
+    parser.add_argument(
+        "--recent_list_max_len",
+        default=100,
+        type=int,
+        help="max length of recent player list",
+    )
+    parser.add_argument(
+        "--latest_weight",
+        default=0.5,
+        type=float,
+        help="latest_weight",
+    )
+    parser.add_argument(
+        "--newest_pos",
+        default=1,
+        type=int,
+        help="newest_pos",
+    )
+    parser.add_argument(
+        "--newest_weight",
+        default=0.5,
+        type=float,
+        help="newest_weight",
+    )
+
     return parser
```

### Comparing `openrl-0.0.9/openrl/drivers/__init__.py` & `openrl-0.1.0/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/drivers/rl_driver.py` & `openrl-0.1.0/openrl/utils/callbacks/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from abc import ABC, abstractmethod
 
-from openrl.drivers.base_driver import BaseDriver
 
+from openrl.utils.callbacks.callbacks_factory import CallbackFactory
 
-class RLDriver(BaseDriver, ABC):
-    @abstractmethod
-    def _inner_loop(self):
-        raise NotImplementedError
+__all__ = ["CallbackFactory"]
```

### Comparing `openrl-0.0.9/openrl/envs/common/__init__.py` & `openrl-0.1.0/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/common/build_envs.py` & `openrl-0.1.0/openrl/envs/common/build_envs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,69 @@
+import copy
+import inspect
 from typing import Callable, Iterable, List, Optional, Union
 
 from gymnasium import Env
 
+from openrl.envs.wrappers.base_wrapper import BaseWrapper
+
 
 def build_envs(
     make,
     id: str,
     env_num: int = 1,
     render_mode: Optional[Union[str, List[str]]] = None,
     disable_env_checker: Optional[bool] = None,
     wrappers: Optional[Union[Callable[[Env], Env], List[Callable[[Env], Env]]]] = None,
+    need_env_id: bool = False,
     **kwargs,
 ) -> List[Callable[[], Env]]:
-    def create_env(env_id: int) -> Callable[[], Env]:
+    cfg = kwargs.get("cfg", None)
+
+    def create_env(env_id: int, env_num: int, need_env_id: bool) -> Callable[[], Env]:
         """Creates an environment that can enable or disable the environment checker."""
         # If the env_id > 0 then disable the environment checker otherwise use the parameter
         _disable_env_checker = True if env_id > 0 else disable_env_checker
 
         def _make_env() -> Env:
             if isinstance(render_mode, list):
                 env_render_mode = render_mode[env_id]
             else:
                 env_render_mode = render_mode
+            new_kwargs = copy.deepcopy(kwargs)
+            if need_env_id:
+                new_kwargs["env_id"] = env_id
+                new_kwargs["env_num"] = env_num
 
             env = make(
                 id,
                 render_mode=env_render_mode,
                 disable_env_checker=_disable_env_checker,
-                **kwargs,
+                **new_kwargs,
             )
+
             if wrappers is not None:
                 if callable(wrappers):
-                    env = wrappers(env)
+                    if issubclass(wrappers, BaseWrapper):
+                        env = wrappers(env, cfg=cfg)
+                    else:
+                        env = wrappers(env)
                 elif isinstance(wrappers, Iterable) and all(
                     [callable(w) for w in wrappers]
                 ):
                     for wrapper in wrappers:
-                        env = wrapper(env)
+                        if (
+                            issubclass(wrapper, BaseWrapper)
+                            and "cfg" in inspect.signature(wrapper.__init__).parameters
+                        ):
+                            env = wrapper(env, cfg=cfg)
+                        else:
+                            env = wrapper(env)
                 else:
                     raise NotImplementedError
+
             return env
 
         return _make_env
 
-    env_fns = [create_env(env_id) for env_id in range(env_num)]
+    env_fns = [create_env(env_id, env_num, need_env_id) for env_id in range(env_num)]
     return env_fns
```

### Comparing `openrl-0.0.9/openrl/envs/gymnasium/__init__.py` & `openrl-0.1.0/openrl/envs/gymnasium/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,41 +11,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
+import copy
 from typing import Callable, List, Optional, Union
 
 import gymnasium as gym
 from gymnasium import Env
 
 from openrl.envs.common import build_envs
 
 
 def make_gym_envs(
     id: str,
     env_num: int = 1,
     render_mode: Optional[Union[str, List[str]]] = None,
     **kwargs,
 ) -> List[Callable[[], Env]]:
-    from openrl.envs.wrappers import (
-        AutoReset,
-        DictWrapper,
+    from openrl.envs.wrappers import (  # AutoReset,; DictWrapper,
         RemoveTruncated,
         Single2MultiAgentWrapper,
     )
 
-    env_wrappers = [
-        DictWrapper,
+    env_wrappers = copy.copy(kwargs.pop("env_wrappers", []))
+    env_wrappers += [
+        # DictWrapper,
         Single2MultiAgentWrapper,
-        AutoReset,
+        # AutoReset,
         RemoveTruncated,
     ]
+
     env_fns = build_envs(
         make=gym.envs.registration.make,
         id=id,
         env_num=env_num,
         render_mode=render_mode,
         wrappers=env_wrappers,
         **kwargs,
```

### Comparing `openrl-0.0.9/openrl/envs/mpe/__init__.py` & `openrl-0.1.0/openrl/envs/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/mpe/core.py` & `openrl-0.1.0/openrl/envs/mpe/core.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/mpe/mpe_env.py` & `openrl-0.1.0/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/mpe/multi_discrete.py` & `openrl-0.1.0/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/mpe/multiagent_env.py` & `openrl-0.1.0/openrl/envs/mpe/multiagent_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/mpe/rendering.py` & `openrl-0.1.0/openrl/envs/mpe/rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,16 +317,16 @@
 
 
 def make_polyline(v):
     return PolyLine(v, False)
 
 
 def make_capsule(length, width):
-    l, r, t, b = 0, length, width / 2, -width / 2
-    box = make_polygon([(l, b), (l, t), (r, t), (r, b)])
+    left, r, t, b = 0, length, width / 2, -width / 2
+    box = make_polygon([(left, b), (left, t), (r, t), (r, b)])
     circ0 = make_circle(width / 2)
     circ1 = make_circle(width / 2)
     circ1.add_attr(Transform(translation=(length, 0)))
     geom = Compound([box, circ0, circ1])
     return geom
```

### Comparing `openrl-0.0.9/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.1.0/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             landmark.state.p_vel = np.zeros(world.dim_p)
 
     def benchmark_data(self, agent, world):
         rew = 0
         collisions = 0
         occupied_landmarks = 0
         min_dists = 0
-        for l in world.landmarks:
+        for landmark in world.landmarks:
             dists = [
-                np.sqrt(np.sum(np.square(a.state.p_pos - l.state.p_pos)))
+                np.sqrt(np.sum(np.square(a.state.p_pos - landmark.state.p_pos)))
                 for a in world.agents
             ]
             min_dists += min(dists)
             rew -= min(dists)
             if min(dists) < 0.1:
                 occupied_landmarks += 1
         if agent.collide:
@@ -86,17 +86,17 @@
         dist = np.sqrt(np.sum(np.square(delta_pos)))
         dist_min = agent1.size + agent2.size
         return True if dist < dist_min else False
 
     def reward(self, agent, world):
         # Agents are rewarded based on minimum agent distance to each landmark, penalized for collisions
         rew = 0
-        for l in world.landmarks:
+        for landmark in world.landmarks:
             dists = [
-                np.sqrt(np.sum(np.square(a.state.p_pos - l.state.p_pos)))
+                np.sqrt(np.sum(np.square(a.state.p_pos - landmark.state.p_pos)))
                 for a in world.agents
             ]
             rew -= min(dists)
 
         if agent.collide:
             for a in world.agents:
                 if self.is_collision(a, agent):
```

### Comparing `openrl-0.0.9/openrl/envs/nlp/__init__.py` & `openrl-0.1.0/openrl/envs/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/daily_dialog_env.py` & `openrl-0.1.0/openrl/envs/nlp/daily_dialog_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/custom_text_generation_pools.py` & `openrl-0.1.0/openrl/envs/nlp/utils/custom_text_generation_pools.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/distribution.py` & `openrl-0.1.0/openrl/envs/nlp/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/evaluation_utils.py` & `openrl-0.1.0/openrl/envs/nlp/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/metrics/__init__.py` & `openrl-0.1.0/openrl/envs/nlp/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/metrics/meteor.py` & `openrl-0.1.0/openrl/envs/nlp/utils/metrics/meteor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/observation.py` & `openrl-0.1.0/openrl/envs/nlp/utils/observation.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/sampler.py` & `openrl-0.1.0/openrl/envs/nlp/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/nlp/utils/text_generation_pool.py` & `openrl-0.1.0/openrl/envs/nlp/utils/text_generation_pool.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/async_venv.py` & `openrl-0.1.0/openrl/envs/vec_env/async_venv.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         action_space: Optional[gym.Space] = None,
         shared_memory: bool = False,  # TODO True,
         copy: bool = True,
         context: Optional[str] = None,
         daemon: bool = True,
         worker: Optional[Callable] = None,
         render_mode: Optional[str] = None,
+        auto_reset: bool = True,
     ):
         """Vectorized environment that runs multiple environments in parallel.
 
         Args:
             env_fns: Functions that create the environments.
             observation_space: Observation space of a single environment. If ``None``,
                 then the observation space of the first environment is taken.
@@ -89,33 +90,39 @@
                 such as gymnasium.spaces.Box, gymnasium.spaces.Discrete, or gymnasium.spaces.Dict) and shared_memory is True.
         """
         ctx = mp.get_context(context)
         self.env_fns = env_fns
         self.shared_memory = shared_memory
         self.copy = copy
         dummy_env = env_fns[0]()
+        if hasattr(dummy_env, "set_render_mode"):
+            dummy_env.set_render_mode(None)
+
         self.metadata = dummy_env.metadata
 
         if (observation_space is None) or (action_space is None):
             observation_space = observation_space or dummy_env.observation_space
             action_space = action_space or dummy_env.action_space
         self._agent_num = dummy_env.agent_num
 
         if hasattr(dummy_env, "env_name"):
             self._env_name = dummy_env.env_name
+        elif "name" in self.metadata:
+            self._env_name = self.metadata["name"]
         else:
             self._env_name = dummy_env.unwrapped.spec.id
 
         dummy_env.close()
         del dummy_env
         super().__init__(
             parallel_env_num=len(env_fns),
             observation_space=observation_space,
             action_space=action_space,
             render_mode=render_mode,
+            auto_reset=auto_reset,
         )
 
         if self.shared_memory:
             try:
                 _obs_buffer = create_shared_memory(
                     self.observation_space,
                     n=self.parallel_env_num,
@@ -160,14 +167,15 @@
                     args=(
                         idx,
                         CloudpickleWrapper(env_fn),
                         child_pipe,
                         parent_pipe,
                         _obs_buffer,
                         self.error_queue,
+                        auto_reset,
                     ),
                 )
 
                 self.parent_pipes.append(parent_pipe)
                 self.processes.append(process)
 
                 process.daemon = daemon
@@ -348,14 +356,15 @@
              The batched environment step information, (obs, reward, terminated, truncated, info)
 
         Raises:
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             NoAsyncCallError: If :meth:`step_fetch` was called without any prior call to :meth:`step_send`.
             TimeoutError: If :meth:`step_fetch` timed out.
         """
+
         self._assert_is_running()
         if self._state != AsyncState.WAITING_STEP:
             raise NoAsyncCallError(
                 "Calling `step_fetch` without any prior call to `step_send`.",
                 AsyncState.WAITING_STEP.value,
             )
 
@@ -364,16 +373,18 @@
             raise mp.TimeoutError(
                 f"The call to `step_fetch` has timed out after {timeout} second(s)."
             )
 
         observations_list, rewards, terminateds, truncateds, infos = [], [], [], [], []
         result_len = None
         successes = []
+
         for i, pipe in enumerate(self.parent_pipes):
             result, success = pipe.recv()
+
             successes.append(success)
             if success:
                 if result_len is None:
                     result_len = len(result)
                 if result_len == 5:
                     obs, rew, terminated, truncated, info = result
                     truncateds.append(truncated)
@@ -575,16 +586,16 @@
             pipe.send(("_call", (name, args, kwargs)))
         self._state = AsyncState.WAITING_CALL
 
     def call_fetch(self, timeout: Union[int, float, None] = None) -> list:
         """Calls all parent pipes and waits for the results.
 
         Args:
-            timeout: Number of seconds before the call to `step_fetch` times out.
-                If `None` (default), the call to `step_fetch` never times out.
+            timeout: Number of seconds before the call to `call_fetch` times out.
+                If `None` (default), the call to `call_fetch` never times out.
 
         Returns:
             List of the results of the individual calls to the method or property for each environment.
 
         Raises:
             NoAsyncCallError: Calling `call_fetch` without any prior call to `call_send`.
             TimeoutError: The call to `call_fetch` has timed out after timeout second(s).
@@ -604,27 +615,73 @@
 
         results, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
         self._state = AsyncState.DEFAULT
 
         return results
 
-    def call(self, name: str, *args, **kwargs) -> List[Any]:
-        """Call a method, or get a property, from each parallel environment.
+    def exec_func_send(self, func: Callable, indices, *args, **kwargs):
+        """Calls the method with name asynchronously and apply args and kwargs to the method.
 
         Args:
-            name (str): Name of the method or property to call.
+            func: a function.
+            indices: Indices of the environments to call the method on.
             *args: Arguments to apply to the method call.
             **kwargs: Keyword arguments to apply to the method call.
 
+        Raises:
+            ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
+            AlreadyPendingCallError: Calling `call_send` while waiting for a pending call to complete
+        """
+        self._assert_is_running()
+        if self._state != AsyncState.DEFAULT:
+            raise AlreadyPendingCallError(
+                (
+                    "Calling `exec_func_send` while waiting "
+                    f"for a pending call to `{self._state.value}` to complete."
+                ),
+                str(self._state.value),
+            )
+
+        for pipe in self.parent_pipes:
+            pipe.send(("_func_exec", (func, indices, args, kwargs)))
+        self._state = AsyncState.WAITING_CALL
+
+    def exec_func_fetch(self, timeout: Union[int, float, None] = None) -> list:
+        """Calls all parent pipes and waits for the results.
+
+        Args:
+            timeout: Number of seconds before the call to `exec_func_fetch` times out.
+                If `None` (default), the call to `exec_func_fetch` never times out.
+
         Returns:
             List of the results of the individual calls to the method or property for each environment.
+
+        Raises:
+            NoAsyncCallError: Calling `call_fetch` without any prior call to `call_send`.
+            TimeoutError: The call to `call_fetch` has timed out after timeout second(s).
         """
-        self.call_send(name, *args, **kwargs)
-        return self.call_fetch()
+        self._assert_is_running()
+        if self._state != AsyncState.WAITING_CALL:
+            raise NoAsyncCallError(
+                "Calling `exec_func_fetch` without any prior call to `exec_func_send`.",
+                AsyncState.WAITING_CALL.value,
+            )
+
+        if not self._poll(timeout):
+            self._state = AsyncState.DEFAULT
+            raise mp.TimeoutError(
+                f"The call to `call_fetch` has timed out after {timeout} second(s)."
+            )
+
+        results, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
+        self._raise_if_errors(successes)
+        self._state = AsyncState.DEFAULT
+
+        return results
 
     def get_attr(self, name: str):
         """Get a property from each parallel environment.
 
         Args:
             name (str): Name of the property to be get from each individual environment.
 
@@ -674,14 +731,15 @@
 def _worker(
     index: int,
     env_fn: callable,
     pipe: Connection,
     parent_pipe: Connection,
     shared_memory: bool,
     error_queue: Queue,
+    auto_reset: bool = True,
 ):
     env = env_fn()
     observation_space = env.observation_space
     action_space = env.action_space
 
     _subenv_auto_reset = hasattr(env, "has_auto_reset") and env.has_auto_reset
     _agent_num = env.agent_num
@@ -698,14 +756,15 @@
             observation = None
         return observation
 
     parent_pipe.close()
     try:
         while True:
             command, data = pipe.recv()
+
             if command == "reset":
                 result = env.reset(**data)
 
                 if isinstance(result, tuple):
                     assert len(result) == 2, (
                         "The `reset` method of the environment must return either a"
                         " single observation or a tuple of (observation, info)."
@@ -741,52 +800,65 @@
                         info,
                     ) = result
                     need_reset = _need_reset and (all(terminated) or all(truncated))
                 else:
                     raise NotImplementedError(
                         "Step result length can not be {}.".format(result_len)
                     )
-                if need_reset:
+                if need_reset and auto_reset:
                     old_observation, old_info = observation, info
                     observation, info = env.reset()
+                    info = deepcopy(info)
                     info["final_observation"] = old_observation
                     info["final_info"] = old_info
 
                 observation = prepare_obs(observation)
+
                 if result_len == 4:
                     pipe.send(((observation, reward, terminated, info), True))
                 else:
                     pipe.send(
                         ((observation, reward, terminated, truncated, info), True)
                     )
+
             elif command == "seed":
                 env.seed(data)
                 pipe.send((None, True))
             elif command == "close":
                 pipe.send((None, True))
                 break
             elif command == "_check_spaces":
                 pipe.send(
                     (
                         (data[0] == observation_space, data[1] == action_space),
                         True,
                     )
                 )
+            elif command == "_func_exec":
+                function, indices, args, kwargs = data
+                if index in indices:
+                    if callable(function):
+                        pipe.send((function(env, *args, **kwargs), True))
+                    else:
+                        pipe.send((function, True))
+                else:
+                    pipe.send((None, True))
             elif command == "_call":
                 name, args, kwargs = data
                 if name in ["reset", "step", "seed", "close"]:
                     raise ValueError(
                         f"Trying to call function `{name}` with "
                         f"`_call`. Use `{name}` directly instead."
                     )
                 function = getattr(env, name)
                 if callable(function):
                     pipe.send((function(*args, **kwargs), True))
                 else:
                     pipe.send((function, True))
+
             elif command == "_setattr":
                 name, value = data
                 setattr(env, name, value)
                 pipe.send((None, True))
             else:
                 raise RuntimeError(
                     f"Received unknown command `{command}`. Must "
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/sync_venv.py` & `openrl-0.1.0/openrl/envs/vec_env/sync_venv.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def __init__(
         self,
         env_fns: Iterable[Callable[[], Env]],
         observation_space: Space = None,
         action_space: Space = None,
         copy: bool = True,
         render_mode: Optional[str] = None,
+        auto_reset: bool = True,
     ):
         """Vectorized environment that serially runs multiple environments.
 
         Args:
             env_fns: iterable of callable functions that create the environments.
             observation_space: Observation space of a single environment. If ``None``,
                 then the observation space of the first environment is taken.
@@ -52,31 +53,35 @@
                 then the action space of the first environment is taken.
             copy: If ``True``, then the :meth:`reset` and :meth:`step` methods return a copy of the observations.
 
         Raises:
             RuntimeError: If the observation space of some sub-environment does not match observation_space
                 (or, by default, the observation space of the first sub-environment).
         """
+        self.viewer = None
         self.env_fns = env_fns
-        self.envs = [env_fn() for env_fn in env_fns]
+        self.envs = []
+        self.envs += [env_fn() for env_fn in env_fns]
 
         self.copy = copy
         self.metadata = self.envs[0].metadata
         self._subenv_auto_reset = (
             hasattr(self.envs[0], "has_auto_reset") and self.envs[0].has_auto_reset
         )
 
         if (observation_space is None) or (action_space is None):
             observation_space = observation_space or self.envs[0].observation_space
             action_space = action_space or self.envs[0].action_space
+
         super().__init__(
             parallel_env_num=len(self.envs),
             observation_space=observation_space,
             action_space=action_space,
             render_mode=render_mode,
+            auto_reset=auto_reset,
         )
 
         self._check_spaces()
         self._agent_num = self.envs[0].agent_num
 
         self.observations = create_empty_array(
             self.observation_space,
@@ -182,14 +187,15 @@
         for i, (env, action) in enumerate(zip(self.envs, _actions)):
             returns = env.step(action)
             assert isinstance(
                 returns, tuple
             ), "step return must be tuple, but got: {}".format(type(returns))
 
             _need_reset = not self._subenv_auto_reset
+
             if len(returns) == 5:
                 (
                     observation,
                     self._rewards[i],
                     self._terminateds[i],
                     self._truncateds[i],
                     info,
@@ -202,17 +208,18 @@
                     observation,
                     self._rewards[i],
                     self._terminateds[i],
                     info,
                 ) = returns
                 need_reset = _need_reset and all(self._terminateds[i])
 
-            if need_reset:
+            if need_reset and self.auto_reset:
                 old_observation, old_info = observation, info
                 observation, info = env.reset()
+                info = deepcopy(info)
                 info["final_observation"] = old_observation
                 info["final_info"] = old_info
 
             observations.append(observation)
             infos.append(info)
 
         if len(returns) == 5:
@@ -263,17 +270,42 @@
         else:
             return [env.render() for env in self.envs]
 
     @property
     def env_name(self):
         if hasattr(self.envs[0], "env_name"):
             return self.envs[0].env_name
+        elif "name" in self.metadata:
+            self._env_name = self.metadata["name"]
         else:
             return self.envs[0].unwrapped.spec.id
 
+    def exec_func(self, func: Callable, indices: List[int], *args, **kwargs) -> tuple:
+        """Calls the method with name and applies args and kwargs.
+
+        Args:
+            func: The method name
+            *args: The method args
+            **kwargs: The method kwargs
+
+        Returns:
+            Tuple of results
+        """
+        results = []
+        for i, env in enumerate(self.envs):
+            if i in indices:
+                if callable(func):
+                    results.append(func(env, *args, **kwargs))
+                else:
+                    results.append(func)
+            else:
+                results.append(None)
+
+        return tuple(results)
+
     def call(self, name, *args, **kwargs) -> tuple:
         """Calls the method with name and applies args and kwargs.
 
         Args:
             name: The method name
             *args: The method args
             **kwargs: The method kwargs
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.1.0/openrl/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.1.0/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # source code from https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/vector/utils/numpy_utils.py
 """Numpy utility functions: concatenate space samples and create empty array."""
 from collections import OrderedDict
 from functools import singledispatch
-from typing import Callable, Iterable, Iterator, Union
+from typing import Callable, Iterable, Iterator, List, Optional, Union
 
 import numpy as np
 from gymnasium.error import CustomSpaceError
 from gymnasium.spaces import (
     Box,
     Dict,
     Discrete,
@@ -16,14 +16,15 @@
     Tuple,
 )
 
 __all__ = [
     "concatenate",
     "create_empty_array",
     "iterate_action",
+    "single_random_action",
 ]
 
 
 @singledispatch
 def iterate_action(space: Space, actions) -> Iterator:
     """Iterate over the elements of a batched actions.
 
@@ -49,15 +50,15 @@
     return iter(action)
 
 
 @iterate_action.register(Box)
 @iterate_action.register(MultiDiscrete)
 @iterate_action.register(MultiBinary)
 def _iterate_base(space, actions):
-    raise NotImplementedError("Not implemented yet.")
+    return iter(actions)
 
 
 @iterate_action.register(Tuple)
 def _iterate_tuple(space, actions):
     raise NotImplementedError("Not implemented yet.")
 
 
@@ -169,25 +170,32 @@
     raise ValueError(
         f"Space of type `{type(space)}` is not a valid `gymnasium.Space` instance."
     )
 
 
 # It is possible for the some of the Box low to be greater than 0, then array is not in space
 @create_empty_array.register(Box)
-# If the Discrete start > 0 or start + length < 0 then array is not in space
-@create_empty_array.register(Discrete)
 @create_empty_array.register(MultiDiscrete)
 @create_empty_array.register(MultiBinary)
 def _create_empty_array_base(space, n=1, agent_num=1, fn=np.zeros):
     # shape = space.shape if (agent_num is None) else (agent_num,) + space.shape
     shape = (agent_num,) + space.shape
     shape = shape if (n is None) else (n,) + shape
     return fn(shape, dtype=space.dtype)
 
 
+# If the Discrete start > 0 or start + length < 0 then array is not in space
+@create_empty_array.register(Discrete)
+def _create_empty_array_discrete(space, n=1, agent_num=1, fn=np.zeros):
+    # shape = space.shape if (agent_num is None) else (agent_num,) + space.shape
+    shape = (agent_num, space.n)
+    shape = shape if (n is None) else (n,) + shape
+    return fn(shape, dtype=space.dtype)
+
+
 @create_empty_array.register(Tuple)
 def _create_empty_array_tuple(space, n=1, agent_num=1, fn=np.zeros):
     return tuple(
         create_empty_array(subspace, n=n, agent_num=agent_num, fn=fn)
         for subspace in space.spaces
     )
 
@@ -201,7 +209,35 @@
         ]
     )
 
 
 @create_empty_array.register(Space)
 def _create_empty_array_custom(space, n=1, agent_num=1, fn=np.zeros):
     return None
+
+
+@singledispatch
+def single_random_action(
+    space: Space, action_mask: Optional[Union[List[int], np.ndarray]] = None
+) -> Union[tuple, dict, np.ndarray]:
+    raise ValueError(
+        f"Space of type `{type(space)}` is not a valid `gymnasium.Space` instance."
+    )
+
+
+@single_random_action.register(Discrete)
+def _single_random_action_discrete(
+    space, action_mask: Optional[Union[List[int], np.ndarray]] = None
+):
+    if action_mask is not None:
+        print(action_mask)
+
+        if isinstance(action_mask, list):
+            action_mask = np.array(action_mask, dtype=np.int8)
+    return [space.sample(mask=action_mask)]
+
+
+@single_random_action.register(Box)
+def _single_random_action_box(
+    space, action_mask: Optional[Union[List[int], np.ndarray]] = None
+):
+    return space.sample()
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.1.0/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/vec_info/__init__.py` & `openrl-0.1.0/openrl/envs/vec_env/vec_info/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,7 +26,11 @@
     def auto_register(vec_info_class: Any):
         if vec_info_class is None:
             return
         elif vec_info_class.id == "NLPVecInfo":
             from openrl.envs.vec_env.vec_info.nlp_vec_info import NLPVecInfo
 
             VecInfoFactory.register("NLPVecInfo", NLPVecInfo)
+        elif vec_info_class.id == "EPS_RewardInfo":
+            from openrl.envs.vec_env.vec_info.episode_rewards_info import EPS_RewardInfo
+
+            VecInfoFactory.register("EPS_RewardInfo", EPS_RewardInfo)
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/vec_info/base_vec_info.py` & `openrl-0.1.0/openrl/envs/vec_env/vec_info/base_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/vec_info/nlp_vec_info.py` & `openrl-0.1.0/openrl/envs/vec_env/vec_info/nlp_vec_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/vec_info/simple_vec_info.py` & `openrl-0.1.0/openrl/envs/vec_env/vec_info/simple_vec_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         self.total_step += np.prod(rewards.shape[:2])
         rewards = rewards.transpose(2, 1, 0, 3)
         info_dict = {}
         ep_rewards = []
         for i in range(self.agent_num):
             agent_reward = rewards[i].mean(0).sum()
             ep_rewards.append(agent_reward)
-            info_dict["agent_{}/episode_reward".format(i)] = agent_reward
+            info_dict["agent_{}/rollout_episode_reward".format(i)] = agent_reward
 
         info_dict["FPS"] = int(self.total_step / (time.time() - self.start_time))
-        info_dict["episode_reward"] = np.mean(ep_rewards)
+        info_dict["rollout_episode_reward"] = np.mean(ep_rewards)
         return info_dict
 
     def append(self, info: Dict[str, Any]) -> None:
         self.infos.append(info)
 
     def reset(self) -> None:
         self.infos = []
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.1.0/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.1.0/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-
-from typing import Any, Dict, Optional, Sequence, SupportsFloat, Tuple, TypeVar, Union
+from abc import ABC
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    SupportsFloat,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
 from gymnasium import spaces
 from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
 from gymnasium.utils import seeding
 
-from openrl.envs.vec_env.base_venv import BaseVecEnv
+from openrl.envs.vec_env.base_venv import BaseVecEnv, VecEnvIndices
+from openrl.envs.wrappers import BaseWrapper
 
 ArrayType = TypeVar("ArrayType")
 
 
-class VecEnvWrapper(BaseVecEnv):
+class VecEnvWrapper(BaseVecEnv, ABC):
     """Wraps the vectorized environment to allow a modular transformation.
 
     This class is the base class for all wrappers for vectorized environments. The subclass
     could override some methods to change the behavior of the original vectorized environment
     without touching the original code.
 
     Note:
@@ -102,24 +114,24 @@
         self._metadata = value
 
     @property
     def render_mode(self) -> Optional[str]:
         """Returns the :attr:`Env` :attr:`render_mode`."""
         return self.env.render_mode
 
-    def random_action(self):
-        return self.env.random_action()
+    def random_action(self, infos=None):
+        return self.env.random_action(infos=infos)
 
     def reset(self, **kwargs):
         """Reset all environments."""
         return self.env.reset(**kwargs)
 
-    def step(self, actions):
+    def step(self, actions, *args, **kwargs):
         """Step all environments."""
-        return self.env.step(actions)
+        return self.env.step(actions, *args, **kwargs)
 
     def close(self, **kwargs):
         return self.env.close(**kwargs)
 
     def close_extras(self, **kwargs):
         return self.env.close_extras(**kwargs)
 
@@ -134,17 +146,14 @@
     def use_monitor(self):
         return False
 
     @property
     def unwrapped(self):
         return self.env.unwrapped
 
-    def __del__(self):
-        self.env.__del__()
-
     def _get_images(self) -> Sequence[np.ndarray]:
         return self.env._get_images()
 
     @property
     def env_name(self):
         if hasattr(self.env, "env_name"):
             return self.env.env_name
@@ -175,47 +184,50 @@
             self._np_random, seed = seeding.np_random()
         return self._np_random
 
     @np_random.setter
     def np_random(self, value: np.random.Generator):
         self._np_random = value
 
+    def env_is_wrapped(
+        self, wrapper_class: Type[BaseWrapper], indices: VecEnvIndices = None
+    ) -> List[bool]:
+        return self.env.env_is_wrapped(wrapper_class, indices=indices)
+
 
 class VectorObservationWrapper(VecEnvWrapper):
     """Wraps the vectorized environment to allow a modular transformation of the observation. Equivalent to :class:`gym.ObservationWrapper` for vectorized environments."""
 
     def reset(self, **kwargs):
         """Modifies the observation returned from the environment ``reset`` using the :meth:`observation`."""
         results = self.env.reset(**kwargs)
         if isinstance(results, tuple) and len(results) == 2:
             observation, info = results
             return self.observation(observation), info
         else:
             observation = results
             return self.observation(observation)
 
-    def step(self, actions):
+    def step(self, actions, *args, **kwargs):
         """Modifies the observation returned from the environment ``step`` using the :meth:`observation`."""
-        results = self.env.step(actions)
+        results = self.env.step(actions, *args, **kwargs)
 
         if len(results) == 5:
             observation, reward, termination, truncation, info = results
             return (
                 self.observation(observation),
-                observation,
                 reward,
                 termination,
                 truncation,
                 info,
             )
         elif len(results) == 4:
             observation, reward, done, info = results
             return (
                 self.observation(observation),
-                observation,
                 reward,
                 done,
                 info,
             )
         else:
             raise ValueError(
                 "Invalid step return value, expected 4 or 5 values, got {} values"
@@ -233,17 +245,17 @@
         """
         raise NotImplementedError
 
 
 class VectorActionWrapper(VecEnvWrapper):
     """Wraps the vectorized environment to allow a modular transformation of the actions. Equivalent of :class:`~gym.ActionWrapper` for vectorized environments."""
 
-    def step(self, actions: ActType):
+    def step(self, actions: ActType, *args, **kwargs):
         """Steps through the environment using a modified action by :meth:`action`."""
-        return self.env.step(self.action(actions))
+        return self.env.step(self.action(actions), *args, **kwargs)
 
     def actions(self, actions: ActType) -> ActType:
         """Transform the actions before sending them to the environment.
 
         Args:
             actions (ActType): the actions to transform
 
@@ -252,17 +264,17 @@
         """
         raise NotImplementedError
 
 
 class VectorRewardWrapper(VecEnvWrapper):
     """Wraps the vectorized environment to allow a modular transformation of the reward. Equivalent of :class:`~gym.RewardWrapper` for vectorized environments."""
 
-    def step(self, actions):
+    def step(self, actions, *args, **kwargs):
         """Steps through the environment returning a reward modified by :meth:`reward`."""
-        results = self.env.step(actions)
+        results = self.env.step(actions, *args, **kwargs)
         reward = self.reward(results[1])
         return results[0], reward, *results[2:]
 
     def reward(self, reward: ArrayType) -> ArrayType:
         """Transform the reward before returning it.
 
         Args:
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/wrappers/reward_wrapper.py` & `openrl-0.1.0/openrl/envs/vec_env/wrappers/reward_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from openrl.rewards.base_reward import BaseReward
 
 
 class RewardWrapper(VecEnvWrapper):
     def __init__(self, env: BaseVecEnv, reward_class: BaseReward):
         super().__init__(env)
         self.reward_class = reward_class
-        if len(self.reward_class.inner_reward_fn) > 0:
-            env.call("set_reward", **{"reward_fn": self.reward_class.inner_reward_fn})
+        if len(self.reward_class.inner_rew_funcs) > 0:
+            env.call("set_reward", **{"reward_fn": self.reward_class.inner_rew_funcs})
 
     def step(
         self, action: ActType, extra_data: Optional[Dict[str, Any]]
     ) -> Union[Any, np.ndarray, np.ndarray, List[Dict[str, Any]]]:
         obs, rewards, dones, infos = self.env.step(action)
 
         if extra_data:
@@ -47,13 +47,14 @@
 
             num_envs = len(infos)
             for i in range(num_envs):
                 if isinstance(infos[i], list):
                     for j in range(len(infos[i])):
                         infos[i][j].update(new_infos[i])
                 else:
-                    infos[i].update(new_infos[i])
+                    if len(new_infos) > 0:
+                        infos[i].update(new_infos[i])
 
         return obs, rewards, dones, infos
 
     def batch_rewards(self, buffer):
         return self.reward_class.batch_rewards(buffer)
```

### Comparing `openrl-0.0.9/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py` & `openrl-0.1.0/openrl/envs/vec_env/wrappers/vec_monitor_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/wrappers/extra_wrappers.py` & `openrl-0.1.0/openrl/envs/wrappers/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,75 +11,61 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from copy import deepcopy
+
+from typing import Any, Optional, Type
 
 import gymnasium as gym
-from gymnasium.wrappers import AutoResetWrapper, StepAPICompatibility
+import numpy as np
+from gymnasium.spaces.box import Box
 
-from openrl.envs.wrappers import BaseObservationWrapper, BaseWrapper
+from openrl.envs.wrappers.base_wrapper import BaseWrapper
 
 
-class RemoveTruncated(StepAPICompatibility, BaseWrapper):
-    def __init__(
-        self,
-        env: gym.Env,
-    ):
-        output_truncation_bool = False
-        super().__init__(env, output_truncation_bool=output_truncation_bool)
-
-
-class AutoReset(AutoResetWrapper, BaseWrapper):
-    def __init__(
-        self,
-        env: gym.Env,
-    ):
-        super().__init__(env)
-
-    @property
-    def has_auto_reset(self):
-        return True
-
-
-class DictWrapper(BaseObservationWrapper):
-    def __init__(self, env):
-        super().__init__(env)
-        need_convert = "Dict" not in self.env.observation_space.__class__.__name__
-        if need_convert:
-            self.observation_space = gym.spaces.Dict(
-                {
-                    "policy": self.env.observation_space,
-                    "critic": self.env.observation_space,
-                }
-            )
-
-    def observation(self, observation):
-        return {"policy": observation, "critic": deepcopy(observation)}
-
-
-class GIFWrapper(BaseWrapper):
-    def __init__(self, env, gif_path: str):
-        super().__init__(env)
-        self.gif_path = gif_path
-        import imageio
-
-        self.writter = imageio.get_writer(self.gif_path, mode="I")
-
-    def reset(self, **kwargs):
-        results = self.env.reset(**kwargs)
-        img = self.env.render()
-        self.writter.append_data(img)
-        return results
-
-    def step(self, action):
-        results = self.env.step(action)
-        img = self.env.render()
-        self.writter.append_data(img)
-        return results
-
-    def close(self):
-        self.env.close()
-        self.writter.close()
+def nest_expand_dim(input: Any) -> Any:
+    if isinstance(input, (np.ndarray, float, int)):
+        return np.expand_dims(input, 0)
+    elif isinstance(input, list):
+        return [input]
+    elif isinstance(input, dict):
+        for key in input:
+            input[key] = nest_expand_dim(input[key])
+        return input
+    elif isinstance(input, Box):
+        return [input]
+    elif isinstance(input, np.int64):
+        return [input]
+    else:
+        raise NotImplementedError("Not support type: {}".format(type(input)))
+
+
+def unwrap_wrapper(
+    env: gym.Env, wrapper_class: Type[BaseWrapper]
+) -> Optional[BaseWrapper]:
+    """
+    Retrieve a ``BaseWrapper`` object by recursively searching.
+
+    :param env: Environment to unwrap
+    :param wrapper_class: Wrapper to look for
+    :return: Environment unwrapped till ``wrapper_class`` if it has been wrapped with it
+    """
+    env_tmp = env
+    while isinstance(env_tmp, BaseWrapper):
+        if isinstance(env_tmp, wrapper_class):
+            return env_tmp
+        env_tmp = env_tmp.env
+    return None
+
+
+def is_wrapped(env: gym.Env, wrapper_class: Type[BaseWrapper]) -> bool:
+    """
+    Check if a given environment has been wrapped with a given wrapper.
+
+    :param env: Environment to check
+    :param wrapper_class: Wrapper class to look for
+    :return: True if environment has been wrapped with ``wrapper_class``.
+    """
+    return unwrap_wrapper(env, wrapper_class) is not None
```

### Comparing `openrl-0.0.9/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.1.0/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/envs/wrappers/util.py` & `openrl-0.1.0/openrl/envs/vec_env/wrappers/zero_reward_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,26 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-from typing import Any
-
 import numpy as np
-from gymnasium.spaces.box import Box
+
+from openrl.envs.vec_env.wrappers.base_wrapper import ArrayType, VectorRewardWrapper
 
 
-def nest_expand_dim(input: Any) -> Any:
-    if isinstance(input, (np.ndarray, float, int)):
-        return np.expand_dims(input, 0)
-    elif isinstance(input, list):
-        return [input]
-    elif isinstance(input, dict):
-        for key in input:
-            input[key] = nest_expand_dim(input[key])
-        return input
-    elif isinstance(input, Box):
-        return [input]
-    else:
-        raise NotImplementedError("Not support type: {}".format(type(input)))
+class ZeroRewardWrapper(VectorRewardWrapper):
+    def reward(self, reward: ArrayType) -> ArrayType:
+        return np.zeros_like(reward)
```

### Comparing `openrl-0.0.9/openrl/modules/__init__.py` & `openrl-0.1.0/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/base_module.py` & `openrl-0.1.0/openrl/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/common/base_net.py` & `openrl-0.1.0/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/common/ppo_net.py` & `openrl-0.1.0/openrl/modules/common/ppo_net.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,37 +19,41 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 import torch
 
 from openrl.configs.config import create_config_parser
+from openrl.envs.vec_env.base_venv import BaseVecEnv
+from openrl.modules.base_module import BaseModule
 from openrl.modules.common.base_net import BaseNet
 from openrl.modules.ppo_module import PPOModule
 from openrl.utils.util import set_seed
 
 
 class PPONet(BaseNet):
     def __init__(
         self,
-        env: Union[gym.Env, str],
+        env: Union[BaseVecEnv, gym.Env, str],
         cfg=None,
         device: Union[torch.device, str] = "cpu",
         n_rollout_threads: int = 1,
         model_dict: Optional[Dict[str, Any]] = None,
+        module_class: BaseModule = PPOModule,
     ) -> None:
         super().__init__()
 
         if cfg is None:
             cfg_parser = create_config_parser()
             cfg = cfg_parser.parse_args([])
 
         set_seed(cfg.seed)
         env.reset(seed=cfg.seed)
 
+        cfg.num_agents = env.agent_num
         cfg.n_rollout_threads = n_rollout_threads
         cfg.learner_n_rollout_threads = cfg.n_rollout_threads
 
         if cfg.rnn_type == "gru":
             rnn_hidden_size = cfg.hidden_size
         elif cfg.rnn_type == "lstm":
             rnn_hidden_size = cfg.hidden_size * 2
@@ -58,15 +62,15 @@
                 f"RNN type {cfg.rnn_type} has not been implemented."
             )
         cfg.rnn_hidden_size = rnn_hidden_size
 
         if isinstance(device, str):
             device = torch.device(device)
 
-        self.module = PPOModule(
+        self.module = module_class(
             cfg=cfg,
             policy_input_space=env.observation_space,
             critic_input_space=env.observation_space,
             act_space=env.action_space,
             share_model=cfg.use_share_model,
             device=device,
             rank=0,
@@ -79,21 +83,22 @@
         self.device = device
         self.rnn_states_actor = None
         self.masks = None
 
     def act(
         self,
         observation: Union[np.ndarray, Dict[str, np.ndarray]],
+        action_masks: Optional[np.ndarray] = None,
         deterministic: bool = False,
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
         actions, self.rnn_states_actor = self.module.act(
             obs=observation,
             rnn_states_actor=self.rnn_states_actor,
             masks=self.masks,
-            available_actions=None,
+            action_masks=action_masks,
             deterministic=deterministic,
         )
 
         return actions, self.rnn_states_actor
 
     def reset(self, env: Optional[gym.Env] = None) -> None:
         if env is not None:
```

### Comparing `openrl-0.0.9/openrl/modules/model_config.py` & `openrl-0.1.0/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/__init__.py` & `openrl-0.1.0/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/base_policy_network.py` & `openrl-0.1.0/openrl/modules/networks/base_policy_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/base_value_network.py` & `openrl-0.1.0/openrl/modules/networks/base_value_network.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/policy_network.py` & `openrl-0.1.0/openrl/modules/networks/policy_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     def __init__(
         self,
         cfg,
         input_space,
         action_space,
         device=torch.device("cpu"),
         use_half=False,
+        extra_args=None,
     ) -> None:
         super(PolicyNetwork, self).__init__(cfg, device)
         self.hidden_size = cfg.hidden_size
 
         self._gain = cfg.gain
         self._use_orthogonal = cfg.use_orthogonal
         self._activation_id = cfg.activation_id
@@ -120,61 +121,61 @@
             return self.forward_original(*args, **kwargs)
         elif forward_type == "eval_actions":
             return self.eval_actions(*args, **kwargs)
         else:
             raise NotImplementedError
 
     def forward_original(
-        self, raw_obs, rnn_states, masks, available_actions=None, deterministic=False
+        self, raw_obs, rnn_states, masks, action_masks=None, deterministic=False
     ):
         policy_obs = get_policy_obs(raw_obs)
         if self._mixed_obs:
             for key in policy_obs.keys():
                 policy_obs[key] = check(policy_obs[key], self.use_half, self.tpdv)
                 if self.use_half:
                     policy_obs[key].half()
         else:
             policy_obs = check(policy_obs, self.use_half, self.tpdv)
             # if self.use_half:
             #     obs = obs.half()
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
         masks = check(masks, self.use_half, self.tpdv)
 
-        if available_actions is not None:
-            available_actions = check(available_actions, self.use_half, self.tpdv)
+        if action_masks is not None:
+            action_masks = check(action_masks, self.use_half, self.tpdv)
 
         actor_features = self.base(policy_obs)
 
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
             actor_features, rnn_states = self.rnn(actor_features, rnn_states, masks)
 
         if self._use_influence_policy:
             mlp_obs = self.mlp(policy_obs)
             actor_features = torch.cat([actor_features, mlp_obs], dim=1)
 
         actions, action_log_probs = self.act(
-            actor_features, available_actions, deterministic
+            actor_features, action_masks, deterministic
         )
         return actions, action_log_probs, rnn_states
 
     def eval_actions(
-        self, obs, rnn_states, action, masks, available_actions=None, active_masks=None
+        self, obs, rnn_states, action, masks, action_masks=None, active_masks=None
     ):
         if self._mixed_obs:
             for key in obs.keys():
                 obs[key] = check(obs[key], self.use_half, self.tpdv)
         else:
             obs = check(obs, self.use_half, self.tpdv)
 
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
         action = check(action, self.use_half, self.tpdv)
         masks = check(masks, self.use_half, self.tpdv)
 
-        if available_actions is not None:
-            available_actions = check(available_actions, self.use_half, self.tpdv)
+        if action_masks is not None:
+            action_masks = check(action_masks, self.use_half, self.tpdv)
 
         if active_masks is not None:
             active_masks = check(active_masks, self.use_half, self.tpdv)
 
         actor_features = self.base(obs)
 
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
@@ -183,15 +184,15 @@
         if self._use_influence_policy:
             mlp_obs = self.mlp(obs)
             actor_features = torch.cat([actor_features, mlp_obs], dim=1)
 
         action_log_probs, dist_entropy = self.act.evaluate_actions(
             actor_features,
             action,
-            available_actions,
+            action_masks,
             active_masks=active_masks if self._use_policy_active_masks else None,
         )
 
         values = self.v_out(actor_features) if self._use_policy_vhead else None
 
         return action_log_probs, dist_entropy, values
```

### Comparing `openrl-0.0.9/openrl/modules/networks/policy_value_network.py` & `openrl-0.1.0/openrl/modules/networks/policy_value_network.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,76 +16,65 @@
 
 """"""
 
 import torch
 import torch.nn as nn
 
 from openrl.buffers.utils.util import get_policy_obs_space
+from openrl.modules.networks.base_value_policy_network import BaseValuePolicyNetwork
 from openrl.modules.networks.utils.act import ACTLayer
 from openrl.modules.networks.utils.cnn import CNNBase
 from openrl.modules.networks.utils.mlp import MLPBase, MLPLayer
 from openrl.modules.networks.utils.popart import PopArt
 from openrl.modules.networks.utils.rnn import RNNLayer
 from openrl.modules.networks.utils.util import init
 from openrl.utils.util import check_v2 as check
 
 
-class PolicyValueNetwork(nn.Module):
+class PolicyValueNetwork(BaseValuePolicyNetwork):
     def __init__(
         self,
         cfg,
-        obs_space,
-        critic_obs_space,
+        input_space,
         action_space,
         device=torch.device("cpu"),
         use_half=False,
+        extra_args=None,
     ):
-        super(PolicyValueNetwork, self).__init__()
+        super(PolicyValueNetwork, self).__init__(cfg, device)
         self._gain = cfg.gain
         self._use_orthogonal = cfg.use_orthogonal
         self._activation_id = cfg.activation_id
         self._recurrent_N = cfg.recurrent_N
         self._use_naive_recurrent_policy = cfg.use_naive_recurrent_policy
         self._use_recurrent_policy = cfg.use_recurrent_policy
-        self._concat_obs_as_critic_obs = cfg.concat_obs_as_critic_obs
+
         self._use_popart = cfg.use_popart
         self.hidden_size = cfg.hidden_size
         self.device = device
         self.use_half = use_half
         self.tpdv = dict(dtype=torch.float32, device=device)
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][
             self._use_orthogonal
         ]
 
         # obs space
-        policy_obs_shape = get_policy_obs_space(obs_space)
+        policy_obs_shape = get_policy_obs_space(input_space)
 
         self.obs_prep = (
             CNNBase(cfg, policy_obs_shape)
             if len(policy_obs_shape) == 3
             else MLPBase(
                 cfg,
                 policy_obs_shape,
                 use_attn_internal=cfg.use_attn_internal,
                 use_cat_self=True,
             )
         )
 
-        # critic_obs_shape = get_critic_obs_space(critic_obs_space)
-        # self.critic_obs_prep = (
-        #     CNNBase(cfg, critic_obs_shape)
-        #     if len(critic_obs_shape) == 3
-        #     else MLPBase(
-        #         cfg,
-        #         critic_obs_shape,
-        #         use_attn_internal=True,
-        #         use_cat_self=cfg.use_cat_self,
-        #     )
-        # )
-        #
         self.critic_obs_prep = self.obs_prep
 
         # common layer
         self.common = MLPLayer(
             self.hidden_size,
             self.hidden_size,
             layer_N=0,
@@ -117,60 +106,60 @@
             action_space, self.hidden_size, self._use_orthogonal, self._gain
         )
         if use_half:
             self.half()
         self.to(self.device)
 
     def get_actions(
-        self, obs, rnn_states, masks, available_actions=None, deterministic=False
+        self, obs, rnn_states, masks, action_masks=None, deterministic=False
     ):
         obs = check(obs, self.use_half, self.tpdv)
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
         masks = check(masks, self.use_half, self.tpdv)
-        if available_actions is not None:
-            available_actions = check(available_actions, self.use_half, self.tpdv)
+        if action_masks is not None:
+            action_masks = check(action_masks, self.use_half, self.tpdv)
 
         x = obs
         x = self.obs_prep(x)
 
         # common
         actor_features = self.common(x)
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
             actor_features, rnn_states = self.rnn(actor_features, rnn_states, masks)
 
         actions, action_log_probs = self.act(
-            actor_features, available_actions, deterministic
+            actor_features, action_masks, deterministic
         )
 
         return actions, action_log_probs, rnn_states
 
-    def evaluate_actions(
-        self, obs, rnn_states, action, masks, available_actions, active_masks=None
+    def eval_actions(
+        self, obs, rnn_states, action, masks, action_masks, active_masks=None
     ):
         obs = check(obs, self.use_half, self.tpdv)
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
         action = check(action, self.use_half, self.tpdv)
         masks = check(masks, self.use_half, self.tpdv)
-        if available_actions is not None:
-            available_actions = check(available_actions, self.use_half, self.tpdv)
+        if action_masks is not None:
+            action_masks = check(action_masks, self.use_half, self.tpdv)
         if active_masks is not None:
             active_masks = check(active_masks, self.use_half, self.tpdv)
 
         x = obs
         x = self.obs_prep(x)
 
         actor_features = self.common(x)
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
             actor_features, rnn_states = self.rnn(actor_features, rnn_states, masks)
 
         action_log_probs, dist_entropy = self.act.evaluate_actions(
-            actor_features, action, available_actions, active_masks
+            actor_features, action, action_masks, active_masks
         )
 
-        return action_log_probs, dist_entropy
+        return action_log_probs, dist_entropy, None
 
     def get_values(self, critic_obs, rnn_states, masks):
         critic_obs = check(critic_obs, self.use_half, self.tpdv)
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
         masks = check(masks, self.use_half, self.tpdv)
 
         share_x = critic_obs
```

### Comparing `openrl-0.0.9/openrl/modules/networks/policy_value_network_gpt.py` & `openrl-0.1.0/openrl/modules/networks/policy_value_network_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self,
         cfg: Any,
         input_space,
         action_space,
         device=torch.device("cpu"),
         use_half=False,
         disable_drop_out: bool = True,
+        extra_args=None,
     ):
         self.disable_drop_out = disable_drop_out
         self._use_valuenorm = cfg.use_valuenorm
         super(CausalLMActorCriticPolicy, self).__init__(
             input_space,
             action_space,
             model_name=cfg.model_path,
@@ -57,15 +58,15 @@
             return self.eval_actions(*args, **kwargs)
         elif forward_type == "get_values":
             return self.get_values(*args, **kwargs)
         else:
             raise NotImplementedError
 
     def get_actions(
-        self, obs, rnn_states, masks, available_actions=None, deterministic=False
+        self, obs, rnn_states, masks, action_masks=None, deterministic=False
     ):
         for key in obs.keys():
             obs[key] = check(obs[key], self.use_half, self.tpdv)
         rnn_states = check(rnn_states, self.use_half, self.tpdv)
 
         past_model_kwargs = None
         policy_output, past_model_kwargs = super().get_distribution(
@@ -74,15 +75,15 @@
         actions = policy_output.mode() if deterministic else policy_output.sample()
         action_log_probs = policy_output.log_prob(actions)
 
         return actions.unsqueeze(-1), action_log_probs.unsqueeze(-1), rnn_states
         # TODO: add past_model_kwargs, i.e., past key value.
 
     def eval_actions(
-        self, obs, rnn_states, action, masks, available_actions, active_masks=None
+        self, obs, rnn_states, action, masks, action_masks, active_masks=None
     ):
         for key in obs.keys():
             obs[key] = check(obs[key], self.use_half, self.tpdv)
         action = check(action, self.use_half, self.tpdv).squeeze()
 
         eval_output = super().evaluate_actions(obs, action)
         action_log_probs = eval_output.log_prob
```

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/act.py` & `openrl-0.1.0/openrl/modules/networks/utils/act.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             self.action_outs = nn.ModuleList(
                 [
                     DiagGaussian(inputs_dim, continous_dim, use_orthogonal, gain),
                     Categorical(inputs_dim, discrete_dim, use_orthogonal, gain),
                 ]
             )
 
-    def forward(self, x, available_actions=None, deterministic=False):
+    def forward(self, x, action_masks=None, deterministic=False):
         if self.mixed_action:
             actions = []
             action_log_probs = []
             for action_out in self.action_outs:
                 action_logit = action_out(x)
                 action = action_logit.mode() if deterministic else action_logit.sample()
                 action_log_prob = action_logit.log_probs(action)
@@ -73,38 +73,38 @@
 
         elif self.continuous_action:
             action_logits = self.action_out(x)
             actions = action_logits.mode() if deterministic else action_logits.sample()
             action_log_probs = action_logits.log_probs(actions)
 
         else:
-            action_logits = self.action_out(x, available_actions)
+            action_logits = self.action_out(x, action_masks)
             actions = action_logits.mode() if deterministic else action_logits.sample()
             action_log_probs = action_logits.log_probs(actions)
         return actions, action_log_probs
 
-    def get_probs(self, x, available_actions=None):
+    def get_probs(self, x, action_masks=None):
         if self.mixed_action or self.multidiscrete_action:
             action_probs = []
             for action_out in self.action_outs:
                 action_logit = action_out(x)
                 action_prob = action_logit.probs
                 action_probs.append(action_prob)
             action_probs = torch.cat(action_probs, -1)
         elif self.continuous_action:
             action_logits = self.action_out(x)
             action_probs = action_logits.probs
         else:
-            action_logits = self.action_out(x, available_actions)
+            action_logits = self.action_out(x, action_masks)
             action_probs = action_logits.probs
 
         return action_probs
 
     def evaluate_actions(
-        self, x, action, available_actions=None, active_masks=None, get_probs=False
+        self, x, action, action_masks=None, active_masks=None, get_probs=False
     ):
         if self.mixed_action:
             a, b = action.split((2, 1), -1)
             b = b.long()
             action = [a, b]
             action_log_probs = []
             dist_entropy = []
@@ -154,15 +154,15 @@
             act_entropy = action_logits.entropy()
             if active_masks is not None:
                 dist_entropy = (act_entropy * active_masks).sum() / active_masks.sum()
             else:
                 dist_entropy = act_entropy.mean()
 
         else:
-            action_logits = self.action_out(x, available_actions)
+            action_logits = self.action_out(x, action_masks)
             action_log_probs = action_logits.log_probs(action)
             if active_masks is not None:
                 dist_entropy = (
                     action_logits.entropy() * active_masks.squeeze(-1)
                 ).sum() / active_masks.sum()
             else:
                 dist_entropy = action_logits.entropy().mean()
```

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/attention.py` & `openrl-0.1.0/openrl/modules/networks/utils/attention.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.1.0/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/distributions.py` & `openrl-0.1.0/openrl/modules/networks/utils/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain)
 
         self.linear = init_(nn.Linear(num_inputs, num_outputs))
 
-    def forward(self, x, available_actions=None):
+    def forward(self, x, action_masks=None):
         x = self.linear(x)
-        if available_actions is not None:
-            x[available_actions == 0] = -1e10
+        if action_masks is not None:
+            x[action_masks == 0] = -1e10
         return FixedCategorical(logits=x)
 
 
 class DiagGaussian(nn.Module):
     def __init__(self, num_inputs, num_outputs, use_orthogonal=True, gain=0.01):
         super(DiagGaussian, self).__init__()
```

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/mix.py` & `openrl-0.1.0/openrl/modules/networks/utils/mix.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,18 @@
         self.embed_keys = []
         self.mlp_keys = []
         self.n_cnn_input = 0
         self.n_embed_input = 0
         self.n_mlp_input = 0
 
         for key in obs_shape:
-            if obs_shape[key].__class__.__name__ == "Box":
+            if (
+                obs_shape[key].__class__.__name__ == "Box"
+                or obs_shape[key].__class__.__name__ == "MultiBinary"
+            ):
                 key_obs_shape = obs_shape[key].shape
                 if len(key_obs_shape) == 3:
                     self.cnn_keys.append(key)
                 else:
                     if "orientation" in key:
                         self.embed_keys.append(key)
                     else:
@@ -81,16 +84,16 @@
     ):
         if cnn_layers_params is None:
             cnn_layers_params = [(32, 8, 4, 0), (64, 4, 2, 0), (64, 3, 1, 0)]
         else:
 
             def _convert(params):
                 output = []
-                for l in params.split(" "):
-                    output.append(tuple(map(int, l.split(","))))
+                for line in params.split(" "):
+                    output.append(tuple(map(int, line.split(","))))
                 return output
 
             cnn_layers_params = _convert(cnn_layers_params)
 
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
         gain = nn.init.calculate_gain(
```

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/mlp.py` & `openrl-0.1.0/openrl/modules/networks/utils/mlp.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/nlp/base_policy.py` & `openrl-0.1.0/openrl/modules/networks/utils/nlp/base_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         Args:
             observation_space (DictSpace): Observation space
             action_space (Discrete): Action space
             model_name (str): name of the causal or seq2seq model from transformers library
             optimizer_kwargs (Dict[str, Any], optional): optimizer kwargs. Defaults to {}.
             weight_decay (float, optional): weight decay. Defaults to 1e-6.
-            use_sde (bool, optional): Use state-dependent exploration. Defaults to None. (Unused parameter from stable-baselines3)
+            use_sde (bool, optional): Use state-dependent exploration. Defaults to None.
             apply_model_parallel (bool, optional): whether to apply model parallel. Defaults to True.
             optimizer_class (torch.optim.Optimizer, optional): Optimizer class. Defaults to torch.optim.AdamW.
             generation_kwargs (Dict[str, Any], optional): generation parameters for rollout. Defaults to {}.
             prompt_truncation_side (str, optional): truncation side for prompt text. Defaults to "left".
         """
         super().__init__()
         self._action_space = action_space
```

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/nlp/causal_policy.py` & `openrl-0.1.0/openrl/modules/networks/utils/nlp/causal_policy.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/nlp/hf_generation_utils.py` & `openrl-0.1.0/openrl/modules/networks/utils/nlp/hf_generation_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/popart.py` & `openrl-0.1.0/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/rnn.py` & `openrl-0.1.0/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.1.0/openrl/modules/networks/utils/transformer_act.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     decoder,
     obs_rep,
     obs,
     batch_size,
     n_agent,
     action_dim,
     tpdv,
-    available_actions=None,
+    action_masks=None,
     deterministic=False,
 ):
     shifted_action = torch.zeros((batch_size, n_agent, action_dim + 1)).to(**tpdv)
     shifted_action[:, 0, 0] = 1
     output_action = torch.zeros((batch_size, n_agent, 1), dtype=torch.long)
     output_action_log = torch.zeros_like(output_action, dtype=torch.float32)
 
     for i in range(n_agent):
         logit = decoder(shifted_action, obs_rep, obs)[:, i, :]
-        if available_actions is not None:
-            logit[available_actions[:, i, :] == 0] = -1e10
+        if action_masks is not None:
+            logit[action_masks[:, i, :] == 0] = -1e10
 
         distri = Categorical(logits=logit)
         action = distri.probs.argmax(dim=-1) if deterministic else distri.sample()
         action_log = distri.log_prob(action)
 
         output_action[:, i, :] = action.unsqueeze(-1)
         output_action_log[:, i, :] = action_log.unsqueeze(-1)
@@ -40,25 +40,25 @@
     obs_rep,
     obs,
     action,
     batch_size,
     n_agent,
     action_dim,
     tpdv,
-    available_actions=None,
+    action_masks=None,
 ):
     one_hot_action = F.one_hot(
         action.squeeze(-1), num_classes=action_dim
     )  # (batch, n_agent, action_dim)
     shifted_action = torch.zeros((batch_size, n_agent, action_dim + 1)).to(**tpdv)
     shifted_action[:, 0, 0] = 1
     shifted_action[:, 1:, 1:] = one_hot_action[:, :-1, :]
     logit = decoder(shifted_action, obs_rep, obs)
-    if available_actions is not None:
-        logit[available_actions == 0] = -1e10
+    if action_masks is not None:
+        logit[action_masks == 0] = -1e10
 
     distri = Categorical(logits=logit)
     action_log = distri.log_prob(action.squeeze(-1)).unsqueeze(-1)
     entropy = distri.entropy().unsqueeze(-1)
     return action_log, entropy
```

### Comparing `openrl-0.0.9/openrl/modules/networks/value_network.py` & `openrl-0.1.0/openrl/modules/networks/value_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     def __init__(
         self,
         cfg,
         input_space,
         action_space=None,
         use_half=False,
         device=torch.device("cpu"),
+        extra_args=None,
     ):
         super(ValueNetwork, self).__init__(cfg, device)
 
         self.hidden_size = cfg.hidden_size
         self._use_orthogonal = cfg.use_orthogonal
         self._activation_id = cfg.activation_id
         self._use_naive_recurrent_policy = cfg.use_naive_recurrent_policy
```

### Comparing `openrl-0.0.9/openrl/modules/ppo_module.py` & `openrl-0.1.0/openrl/modules/ppo_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-
 from typing import Any, Dict, Optional, Union
 
 import gym
 import numpy as np
 import torch
 
 from openrl.modules.model_config import ModelTrainConfig
@@ -39,102 +38,107 @@
         act_space: gym.spaces.Box,
         share_model: bool = False,
         device: Union[str, torch.device] = "cpu",
         rank: Optional[int] = None,
         world_size: Optional[int] = None,
         model_dict: Optional[Dict[str, Any]] = None,
     ):
+        self.share_model = share_model
+        self.policy_input_space = policy_input_space
+        self.critic_input_space = critic_input_space
+        self.model_dict = model_dict
+
+        super(PPOModule, self).__init__(
+            cfg=cfg,
+            act_space=act_space,
+            rank=rank,
+            world_size=world_size,
+            device=device,
+        )
+
+    def get_model_configs(self, cfg) -> Dict[str, Any]:
         model_configs = {}
-        if share_model:
+        if self.share_model:
             model_configs["model"] = ModelTrainConfig(
                 lr=cfg.lr,
                 model=(
-                    model_dict["model"]
-                    if model_dict and "model" in model_dict
+                    self.model_dict["model"]
+                    if self.model_dict and "model" in self.model_dict
                     else PolicyValueNetwork
                 ),
-                input_space=policy_input_space,
+                input_space=self.policy_input_space,
             )
         else:
             model_configs["policy"] = ModelTrainConfig(
                 lr=cfg.lr,
                 model=(
-                    model_dict["policy"]
-                    if model_dict and "policy" in model_dict
+                    self.model_dict["policy"]
+                    if self.model_dict and "policy" in self.model_dict
                     else PolicyNetwork
                 ),
-                input_space=policy_input_space,
+                input_space=self.policy_input_space,
             )
             model_configs["critic"] = ModelTrainConfig(
                 lr=cfg.critic_lr,
                 model=(
-                    model_dict["critic"]
-                    if model_dict and "critic" in model_dict
+                    self.model_dict["critic"]
+                    if self.model_dict and "critic" in self.model_dict
                     else ValueNetwork
                 ),
-                input_space=critic_input_space,
+                input_space=self.critic_input_space,
             )
-
-        super(PPOModule, self).__init__(
-            cfg=cfg,
-            model_configs=model_configs,
-            act_space=act_space,
-            rank=rank,
-            world_size=world_size,
-            device=device,
-        )
-        self.share_model = share_model
-        self.cfg = cfg
+        return model_configs
 
     def lr_decay(self, episode, episodes):
         if self.share_model:
             update_linear_schedule(self.optimizers["model"], episode, episodes, self.lr)
         else:
-            update_linear_schedule(self.optimizers["actor"], episode, episodes, self.lr)
+            update_linear_schedule(
+                self.optimizers["policy"], episode, episodes, self.lr
+            )
             update_linear_schedule(
                 self.optimizers["critic"], episode, episodes, self.critic_lr
             )
 
     def get_actions(
         self,
         critic_obs,
         obs,
         rnn_states_actor,
         rnn_states_critic,
         masks,
-        available_actions=None,
+        action_masks=None,
         deterministic=False,
     ):
         if self.share_model:
             actions, action_log_probs, rnn_states_actor = self.models["model"](
                 "original",
                 obs,
                 rnn_states_actor,
                 masks,
-                available_actions,
+                action_masks,
                 deterministic,
             )
 
             values, rnn_states_critic = self.models["model"](
                 "get_values", critic_obs, rnn_states_critic, masks
             )
         else:
             actions, action_log_probs, rnn_states_actor = self.models["policy"](
                 "original",
                 obs,
                 rnn_states_actor,
                 masks,
-                available_actions,
+                action_masks,
                 deterministic,
             )
 
             values, rnn_states_critic = self.models["critic"](
                 critic_obs, rnn_states_critic, masks
             )
-
         return values, actions, action_log_probs, rnn_states_actor, rnn_states_critic
 
     def get_values(self, critic_obs, rnn_states_critic, masks):
         if self.share_model:
             values, _ = self.models["model"](
                 "get_values", critic_obs, rnn_states_critic, masks
             )
@@ -146,15 +150,15 @@
         self,
         critic_obs,
         obs,
         rnn_states_actor,
         rnn_states_critic,
         action,
         masks,
-        available_actions=None,
+        action_masks=None,
         active_masks=None,
         critic_masks_batch=None,
     ):
         if critic_masks_batch is None:
             critic_masks_batch = masks
 
         if self.share_model:
@@ -164,48 +168,46 @@
 
             action_log_probs, dist_entropy, policy_values = self.models["model"](
                 "eval_actions",
                 obs,
                 rnn_states_actor,
                 action,
                 masks,
-                available_actions,
+                action_masks,
                 active_masks,
             )
         else:
             values, _ = self.models["critic"](
                 critic_obs, rnn_states_critic, critic_masks_batch
             )
 
             action_log_probs, dist_entropy, policy_values = self.models["policy"](
                 "eval_actions",
                 obs,
                 rnn_states_actor,
                 action,
                 masks,
-                available_actions,
+                action_masks,
                 active_masks,
             )
 
         return values, action_log_probs, dist_entropy, policy_values
 
-    def act(
-        self, obs, rnn_states_actor, masks, available_actions=None, deterministic=False
-    ):
+    def act(self, obs, rnn_states_actor, masks, action_masks=None, deterministic=False):
         if self.share_model:
             model = self.models["model"]
         else:
             model = self.models["policy"]
 
         actions, _, rnn_states_actor = model(
             "original",
             obs,
             rnn_states_actor,
             masks,
-            available_actions,
+            action_masks,
             deterministic,
         )
 
         return actions, rnn_states_actor
 
     def get_critic_value_normalizer(self):
         if self.share_model:
```

### Comparing `openrl-0.0.9/openrl/modules/rl_module.py` & `openrl-0.1.0/openrl/modules/rl_module.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from abc import abstractmethod
 from pathlib import Path
-from typing import Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import torch
 from gym import spaces
 
 from openrl.modules.base_module import BaseModule
 from openrl.modules.model_config import ModelTrainConfig
 
 
 class RLModule(BaseModule):
     def __init__(
         self,
         cfg,
-        model_configs: Dict[str, ModelTrainConfig],
         act_space: spaces.Box,
         rank: int = 0,
         world_size: int = 1,
         device: Union[str, torch.device] = "cpu",
+        model_configs: Optional[Dict[str, ModelTrainConfig]] = None,
     ) -> None:
         super(RLModule, self).__init__(cfg)
 
         if isinstance(device, str):
             device = torch.device(device)
 
+        self.cfg = cfg
         self.device = device
         self.lr = cfg.lr
         self.critic_lr = cfg.critic_lr
         self.opti_eps = cfg.opti_eps
         self.weight_decay = cfg.weight_decay
         self.load_optimizer = cfg.load_optimizer
 
@@ -52,22 +53,26 @@
 
         self.program_type = cfg.program_type
         self.rank = rank
         self.world_size = world_size
 
         use_half_actor = self.program_type == "actor" and cfg.use_half_actor
 
+        if model_configs is None:
+            model_configs = self.get_model_configs(cfg)
+
         for model_key in model_configs:
             model_cg = model_configs[model_key]
             model = model_cg["model"](
                 cfg=cfg,
                 input_space=model_cg["input_space"],
                 action_space=act_space,
                 device=device,
                 use_half=use_half_actor,
+                extra_args=model_cg["extra_args"] if "extra_args" in model_cg else None,
             )
             self.models.update({model_key: model})
 
             if self.program_type == "actor":
                 continue
 
             optimizer = torch.optim.Adam(
@@ -79,50 +84,31 @@
             self.optimizers.update({model_key: optimizer})
 
             if cfg.use_amp:
                 self.scaler = torch.cuda.amp.GradScaler()
             else:
                 self.scaler = None
 
+    def get_model_configs(self, cfg) -> Dict[str, Any]:
+        raise NotImplementedError
+
     @abstractmethod
-    def get_actions(
-        self,
-        critic_obs,
-        obs,
-        rnn_states_actor,
-        rnn_states_critic,
-        masks,
-        available_actions=None,
-        deterministic=False,
-    ):
+    def get_actions(self):
         raise NotImplementedError
 
     @abstractmethod
-    def get_values(self, critic_obs, rnn_states_critic, masks):
+    def get_values(self):
         raise NotImplementedError
 
     @abstractmethod
-    def evaluate_actions(
-        self,
-        critic_obs,
-        obs,
-        rnn_states_actor,
-        rnn_states_critic,
-        action,
-        masks,
-        available_actions=None,
-        active_masks=None,
-        critic_masks_batch=None,
-    ):
+    def evaluate_actions(self):
         raise NotImplementedError
 
     @abstractmethod
-    def act(
-        self, obs, rnn_states_actor, masks, available_actions=None, deterministic=False
-    ):
+    def act(self):
         raise NotImplementedError
 
     @abstractmethod
     def get_critic_value_normalizer(self):
         raise NotImplementedError
 
     def load_policy(self, model_path: str) -> None:
```

### Comparing `openrl-0.0.9/openrl/modules/utils/__init__.py` & `openrl-0.1.0/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/modules/utils/util.py` & `openrl-0.1.0/openrl/modules/utils/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 
 
-def get_gard_norm(it):
+def get_grad_norm(it):
     sum_grad = 0
     for x in it:
         if x.grad is None:
             continue
         sum_grad += x.grad.norm() ** 2
     return math.sqrt(sum_grad)
```

### Comparing `openrl-0.0.9/openrl/modules/utils/valuenorm.py` & `openrl-0.1.0/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/rewards/__init__.py` & `openrl-0.1.0/openrl/rewards/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 
 
 class RewardFactory:
     @staticmethod
     def get_reward_class(reward_class: Any, env: BaseVecEnv):
         RewardFactory.auto_register(reward_class)
         if reward_class is None or reward_class.id is None:
-            return registed_rewards["default"]()
+            return registed_rewards["default"](env)
         return registed_rewards[reward_class.id](env, **reward_class.args)
 
     @staticmethod
     def register(reward_name, reward_class):
         registed_rewards.update({reward_name: reward_class})
 
     @staticmethod
     def auto_register(reward_class: Any):
         if reward_class is None:
             return
         if reward_class.id == "NLPReward":
             from openrl.rewards.nlp_reward import NLPReward
 
             registed_rewards.update({"NLPReward": NLPReward})
+        elif reward_class.id == "GAILReward":
+            from openrl.rewards.gail_reward import GAILReward
+
+            registed_rewards.update({"GAILReward": GAILReward})
```

### Comparing `openrl-0.0.9/openrl/rewards/nlp_reward.py` & `openrl-0.1.0/openrl/rewards/nlp_reward.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, env: Env, ref_model: str, intent_model: str):
         self.rew_infos = []
         self.env_infos = []
 
         meteor_config = {
             "meteor_coeff": 0.5,
         }
-        self.inner_reward_fn = {
+        self.inner_rew_funcs = {
             "meteor": Meteor(**meteor_config),
         }
 
         kl_config = {
             "action_space": env.action_space,
             "ref_model": ref_model,
         }
```

### Comparing `openrl-0.0.9/openrl/runners/__init__.py` & `openrl-0.1.0/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/runners/common/base_agent.py` & `openrl-0.1.0/openrl/runners/common/base_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import io
 import pathlib
 from abc import ABC, abstractmethod
-from typing import TypeVar, Union
+from typing import Optional, TypeVar, Union
+
+from openrl.envs.vec_env import BaseVecEnv
+from openrl.utils.logger import Logger
 
 SelfAgent = TypeVar("SelfAgent", bound="BaseAgent")
 
 SelfBaseAgent = TypeVar("SelfBaseAgent", bound="BaseAgent")
 
 
 class BaseAgent(ABC):
@@ -39,7 +42,20 @@
 
     @abstractmethod
     def load(
         self,
         path: Union[str, pathlib.Path, io.BufferedIOBase],
     ):
         raise NotImplementedError
+
+    def get_env(self) -> Optional[BaseVecEnv]:
+        """
+        Returns the current environment (can be None if not defined).
+
+        :return: The current environment
+        """
+        return self._env
+
+    @property
+    def logger(self) -> Logger:
+        """Getter for the logger object."""
+        return self._logger
```

### Comparing `openrl-0.0.9/openrl/runners/common/chat_agent.py` & `openrl-0.1.0/openrl/runners/common/chat_agent.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/runners/common/ppo_agent.py` & `openrl-0.1.0/openrl/runners/common/vdn_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,42 +11,54 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import Optional, Union
+from typing import Dict, Optional, Tuple, Type, Union
 
 import gym
+import numpy as np
 import torch
 
-from openrl.algorithms.ppo import PPOAlgorithm as TrainAlgo
-from openrl.buffers import NormalReplayBuffer as ReplayBuffer
-from openrl.drivers.onpolicy_driver import OnPolicyDriver as Driver
-from openrl.runners.common.rl_agent import RLAgent
+from openrl.algorithms.base_algorithm import BaseAlgorithm
+from openrl.algorithms.vdn import VDNAlgorithm as TrainAlgo
+from openrl.buffers import OffPolicyReplayBuffer as ReplayBuffer
+from openrl.buffers.utils.obs_data import ObsData
+from openrl.drivers.offpolicy_driver import OffPolicyDriver as Driver
 from openrl.runners.common.base_agent import SelfAgent
+from openrl.runners.common.rl_agent import RLAgent
 from openrl.utils.logger import Logger
+from openrl.utils.type_aliases import MaybeCallback
 
 
-class PPOAgent(RLAgent):
+class VDNAgent(RLAgent):
     def __init__(
         self,
         net: Optional[torch.nn.Module] = None,
         env: Union[gym.Env, str] = None,
         run_dir: Optional[str] = None,
         env_num: Optional[int] = None,
         rank: int = 0,
         world_size: int = 1,
         use_wandb: bool = False,
         use_tensorboard: bool = False,
     ) -> None:
-        super(PPOAgent, self).__init__(net, env, run_dir, env_num, rank, world_size, use_wandb, use_tensorboard)
+        super(VDNAgent, self).__init__(
+            net, env, run_dir, env_num, rank, world_size, use_wandb, use_tensorboard
+        )
 
-    def train(self: SelfAgent, total_time_steps: int) -> None:
+    def train(
+        self: SelfAgent,
+        total_time_steps: int,
+        callback: MaybeCallback = None,
+        train_algo_class: Type[BaseAlgorithm] = TrainAlgo,
+        logger: Optional[Logger] = None,
+    ) -> None:
         self._cfg.num_env_steps = total_time_steps
 
         self.config = {
             "cfg": self._cfg,
             "num_agents": self.agent_num,
             "run_dir": self.run_dir,
             "envs": self._env,
@@ -62,29 +74,57 @@
 
         buffer = ReplayBuffer(
             self._cfg,
             self.agent_num,
             self._env.observation_space,
             self._env.action_space,
             data_client=None,
+            episode_length=self._cfg.episode_length,
         )
 
         logger = Logger(
             cfg=self._cfg,
-            project_name="PPOAgent",
+            project_name="VDNAgent",
             scenario_name=self._env.env_name,
             wandb_entity=self._cfg.wandb_entity,
             exp_name=self.exp_name,
             log_path=self.run_dir,
             use_wandb=self._use_wandb,
             use_tensorboard=self._use_tensorboard,
         )
+        self._logger = logger
+
+        total_time_steps, callback = self._setup_train(
+            total_time_steps,
+            callback,
+            reset_num_time_steps=True,
+            progress_bar=False,
+        )
+
         driver = Driver(
             config=self.config,
             trainer=trainer,
             buffer=buffer,
+            agent=self,
             client=self.client,
             rank=self.rank,
             world_size=self.world_size,
             logger=logger,
+            callback=callback,
         )
+
+        callback.on_training_start(locals(), globals())
+
         driver.run()
+
+        callback.on_training_end()
+
+    def act(
+        self, observation: Union[np.ndarray, Dict[str, np.ndarray]], deterministic=None
+    ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
+        assert self.net is not None, "net is None"
+        observation = ObsData.prepare_input(observation)
+        action, rnn_state = self.net.act(observation)
+
+        # action = np.array(np.split(_t2n(action), self.env_num))
+
+        return action, rnn_state
```

### Comparing `openrl-0.0.9/openrl/runners/common/rl_agent.py` & `openrl-0.1.0/openrl/runners/common/sac_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,130 +11,132 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-import io
-import pathlib
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Type, Union
 
 import gym
 import numpy as np
 import torch
 
+from openrl.algorithms.base_algorithm import BaseAlgorithm
+from openrl.algorithms.sac import SACAlgorithm as TrainAlgo
+from openrl.buffers import OffPolicyReplayBuffer as ReplayBuffer
 from openrl.buffers.utils.obs_data import ObsData
-from openrl.runners.common.base_agent import BaseAgent, SelfAgent
-from openrl.utils.util import _t2n
+from openrl.drivers.base_driver import BaseDriver
+from openrl.drivers.offpolicy_driver import OffPolicyDriver as Driver
+from openrl.runners.common.base_agent import SelfAgent
+from openrl.runners.common.rl_agent import RLAgent
+from openrl.utils.logger import Logger
+from openrl.utils.type_aliases import MaybeCallback
 
 
-class RLAgent(BaseAgent):
+class SACAgent(RLAgent):
     def __init__(
         self,
         net: Optional[torch.nn.Module] = None,
         env: Union[gym.Env, str] = None,
         run_dir: Optional[str] = None,
         env_num: Optional[int] = None,
         rank: int = 0,
         world_size: int = 1,
         use_wandb: bool = False,
         use_tensorboard: bool = False,
+        project_name: str = "SACAgent",
     ) -> None:
-        self.net = net
-        self._cfg = net.cfg
-        self._use_wandb = use_wandb
-        self._use_tensorboard = not use_wandb and use_tensorboard
-
-        if env is not None:
-            self._env = env
-        elif hasattr(net, "env") and net.env is not None:
-            self._env = net.env
-        else:
-            raise ValueError("env is None")
-
-        if env_num is not None:
-            self.env_num = env_num
-        else:
-            self.env_num = self._env.parallel_env_num
-
-        self._cfg.n_rollout_threads = self.env_num
-        self._cfg.learner_n_rollout_threads = self._cfg.n_rollout_threads
-
-        self.rank = rank
-        self.world_size = world_size
-
-        self.client = None
-        self.agent_num = self._env.agent_num
-        if run_dir is None:
-            self.run_dir = self._cfg.run_dir
-        else:
-            self.run_dir = run_dir
-
-        if self.run_dir is None:
-            assert (not self._use_wandb) and (not self._use_tensorboard), (
-                "run_dir must be set when using wandb or tensorboard. Please set"
-                " run_dir in the config file or pass run_dir in the"
-                " command line."
+        super(SACAgent, self).__init__(
+            net,
+            env,
+            run_dir,
+            env_num,
+            rank,
+            world_size,
+            use_wandb,
+            use_tensorboard,
+            project_name=project_name,
+        )
+
+    def train(
+        self: SelfAgent,
+        total_time_steps: int,
+        callback: MaybeCallback = None,
+        train_algo_class: Type[BaseAlgorithm] = TrainAlgo,
+        logger: Optional[Logger] = None,
+        DriverClass: Type[BaseDriver] = Driver,
+    ) -> None:
+        self._cfg.num_env_steps = total_time_steps
+
+        self.config = {
+            "cfg": self._cfg,
+            "num_agents": self.agent_num,
+            "run_dir": self.run_dir,
+            "envs": self._env,
+            "device": self.net.device,
+        }
+
+        trainer = train_algo_class(
+            cfg=self._cfg,
+            init_module=self.net.module,
+            device=self.net.device,
+            agent_num=self.agent_num,
+        )
+
+        buffer = ReplayBuffer(
+            self._cfg,
+            self.agent_num,
+            self._env.observation_space,
+            self._env.action_space,
+            data_client=None,
+            episode_length=self._cfg.episode_length,
+        )
+
+        if logger is None:
+            logger = Logger(
+                cfg=self._cfg,
+                project_name=self.project_name,
+                scenario_name=self._env.env_name,
+                wandb_entity=self._cfg.wandb_entity,
+                exp_name=self.exp_name,
+                log_path=self.run_dir,
+                use_wandb=self._use_wandb,
+                use_tensorboard=self._use_tensorboard,
             )
+        self._logger = logger
+
+        total_time_steps, callback = self._setup_train(
+            total_time_steps,
+            callback,
+            reset_num_time_steps=True,
+            progress_bar=False,
+        )
+
+        driver = DriverClass(
+            config=self.config,
+            trainer=trainer,
+            buffer=buffer,
+            agent=self,
+            client=self.client,
+            rank=self.rank,
+            world_size=self.world_size,
+            logger=logger,
+            callback=callback,
+        )
 
-        if self._cfg.experiment_name == "":
-            self.exp_name = "rl"
-        else:
-            self.exp_name = self._cfg.experiment_name
+        callback.on_training_start(locals(), globals())
 
-    def train(self: SelfAgent, total_time_steps: int) -> None:
-        raise NotImplementedError
+        driver.run()
+
+        callback.on_training_end()
 
     def act(
-        self,
-        observation: Union[np.ndarray, Dict[str, np.ndarray]],
-        deterministic: bool = True,
+        self, observation: Union[np.ndarray, Dict[str, np.ndarray]], deterministic=True
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
         assert self.net is not None, "net is None"
         observation = ObsData.prepare_input(observation)
-        action, rnn_state = self.net.act(observation, deterministic=deterministic)
 
-        action = np.array(np.split(_t2n(action), self.env_num))
-
-        return action, rnn_state
-
-    def set_env(
-        self,
-        env: Union[gym.Env, str] = None,
-    ):
-        self.net.reset()
-        if env is not None:
-            self._env = env
-            self.env_num = env.parallel_env_num
-        env.reset(seed=self._cfg.seed)
-        self.net.reset(env)
-
-    def save(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
-        if isinstance(path, str):
-            path = pathlib.Path(path)
-        path.mkdir(parents=True, exist_ok=True)
-        torch.save(self.net.module, path / "module.pt")
-
-    def load(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
-        if isinstance(path, str):
-            path = pathlib.Path(path)
-
-        assert path.exists(), f"{path} does not exist"
-
-        if path.is_dir():
-            path = path / "module.pt"
-
-        assert path.exists(), f"{path} does not exist"
-
-        if not torch.cuda.is_available():
-            self.net.module = torch.load(path, map_location=torch.device("cpu"))
-            self.net.module.device = torch.device("cpu")
-            for key in self.net.module.models:
-                self.net.module.models[key].tpdv = dict(
-                    dtype=torch.float32, device=torch.device("cpu")
-                )
-        else:
-            self.net.module = torch.load(path)
+        action = self.net.act(observation, deterministic=deterministic)
+        action = np.array(np.split(action, self.env_num))
 
-    def load_policy(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
-        self.net.load_policy(path)
+        return action, None
```

### Comparing `openrl-0.0.9/openrl/supports/__init__.py` & `openrl-0.1.0/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opendata/__init__.py` & `openrl-0.1.0/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opendata/utils/__init__.py` & `openrl-0.1.0/openrl/selfplay/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opendata/utils/opendata_utils.py` & `openrl-0.1.0/openrl/supports/opendata/utils/opendata_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opengpu/__init__.py` & `openrl-0.1.0/openrl/selfplay/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opengpu/gpu_info.py` & `openrl-0.1.0/openrl/supports/opengpu/gpu_info.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/supports/opengpu/manager.py` & `openrl-0.1.0/openrl/supports/opengpu/manager.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/utils/__init__.py` & `openrl-0.1.0/openrl/selfplay/multiplayer_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/openrl/utils/logger.py` & `openrl-0.1.0/openrl/utils/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,24 +36,26 @@
         scenario_name: str,
         wandb_entity: str,
         exp_name: Optional[str] = None,
         log_path: Optional[str] = None,
         use_wandb: bool = False,
         use_tensorboard: bool = False,
         log_level: int = logging.DEBUG,
+        log_to_terminal: bool = True,
     ) -> None:
         # TODO: change these flags to log_backend
         self.use_wandb = use_wandb
         self.use_tensorboard = use_tensorboard
 
         self.log_level = log_level
         self.log_path = log_path
         self.project_name = project_name
         self.scenario_name = scenario_name
         self.wandb_entity = wandb_entity
+        self.log_to_terminal = log_to_terminal
         if exp_name is not None:
             self.exp_name = exp_name
         else:
             self.exp_name = cfg.experiment_name
         self.cfg = cfg
         self._init()
 
@@ -102,19 +104,25 @@
                 run_dir = run_dir / curr_run
                 if not run_dir.exists():
                     os.makedirs(str(run_dir))
 
         if hasattr(self.cfg, "render"):
             self.cfg.render_save_path = run_dir / "render.png"
 
-        handlers = [RichHandler()]
+        handlers = []
+        if self.cfg.use_rich_handler:
+            handlers.append(RichHandler())
+
         if run_dir is not None:
             log_file = os.path.join(run_dir, "log.txt")
             handlers.append(logging.FileHandler(log_file))
 
+        for handler in logging.root.handlers[:]:
+            logging.root.removeHandler(handler)
+
         logging.basicConfig(
             level=self.log_level,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
         if self.use_wandb:
@@ -168,21 +176,24 @@
                 )
 
     def log_info(
         self,
         infos: Dict[str, Any],
         step: int,
     ) -> None:
-        if not (self.use_wandb or self.use_tensorboard):
+        if not (self.use_wandb or self.use_tensorboard or self.log_to_terminal):
             return
-
+        logging_info_str = "\n"
         for k, v in infos.items():
             if isinstance(v, torch.Tensor):
                 v = v.item()
 
             if not isinstance(v, (int, float)):
                 v = np.mean(v)
+            logging_info_str += f"\t{k}: {v}\n"
 
             if self.use_wandb:
                 wandb.log({k: v}, step=step)
             elif self.use_tensorboard:
                 self.writter.add_scalars(k, {k: v}, step)
+        if self.log_to_terminal:
+            logging.info(logging_info_str)
```

### Comparing `openrl-0.0.9/openrl/utils/util.py` & `openrl-0.1.0/openrl/utils/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     return x.detach().cpu().numpy()
 
 
 def get_system_info() -> Dict[str, str]:
     """
     Retrieve system and python env info for the current system.
 
-    :param print_info: Whether to print or not those infos
     :return: Dictionary summing up the version for each relevant package
         and a formatted string.
     """
 
     env_info = {
         # In OS, a regex is used to add a space between a "#" and a number to avoid
         # wrongly linking to another issue on GitHub.
```

### Comparing `openrl-0.0.9/openrl.egg-info/PKG-INFO` & `openrl-0.1.0/openrl.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,261 +1,328 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.9
+Version: 0.1.0
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mpe
 Provides-Extra: nlp
+Provides-Extra: selfplay
+Provides-Extra: retro
+Provides-Extra: super_mario
 License-File: LICENSE
-License-File: LICENSE.txt
 
 <div align="center">
-    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="./docs/images/openrl_text.png"></a>
+    <a href="https://openrl-docs.readthedocs.io/zh/latest/index.html"><img width="450px" height="auto" src="docs/images/openrl_text.png"></a>
 </div>
 
 ---
 [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/openrl/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://codecov.io/gh/OpenRL-Lab/openrl)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
-[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/en/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL-Lab)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl)
 [![GitHub issues](https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls)
 [![Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/blob/master/LICENSE)
 
-OpenRL-v0.0.9 is updated on May 6, 2023 
+[![Embark](https://img.shields.io/badge/discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT)
+[![slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg)
+
+OpenRL-v0.0.16 is updated on July 30, 2023
 
 The main branch is the latest version of OpenRL, which is under active development. If you just want to have a try with OpenRL, you can switch to the stable branch.
 
-## 欢迎来到OpenRL
+## Welcome to OpenRL
+
+[Documentation](https://openrl-docs.readthedocs.io/en/latest/) | [中文介绍](README_zh.md) |  [中文文档](https://openrl-docs.readthedocs.io/zh/latest/)
+
+<div align="center">
+    Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights Welcome.   <br><br>
+</div>
+
+OpenRL is an open-source general reinforcement learning research framework that supports training for various tasks 
+such as single-agent, multi-agent, offline RL, self-play, and natural language. 
+Developed based on PyTorch, the goal of OpenRL is to provide a simple-to-use, flexible, efficient and sustainable platform for the reinforcement learning research community.
+
+Currently, the features supported by OpenRL include:
+
+- A simple-to-use universal interface that supports training for both single-agent and multi-agent
+
+- Support for offline RL training with expert dataset
+
+- Support self-play training
+
+- Reinforcement learning training support for natural language tasks (such as dialogue)
+
+- Importing models and datasets from [Hugging Face](https://huggingface.co/)
+
+- Support for models such as LSTM, GRU, Transformer etc.
+
+- Multiple training acceleration methods including automatic mixed precision training and data collecting wth half precision policy network
+
+- User-defined training models, reward models, training data and environment support
+
+- Support for [gymnasium](https://gymnasium.farama.org/) environments
+
+- Support for [Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html), which can be used to implement various functions such as logging, saving, and early stopping
+
+- Dictionary observation space support
+
+- Popular visualization tools such as [wandb](https://wandb.ai/),  [tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html) are supported
+
+- Serial or parallel environment training while ensuring consistent results in both modes
 
-[English](./README_en.md) | [中文文档](https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://openrl-docs.readthedocs.io/en/latest/)
+- Chinese and English documentation
 
-OpenRL是一个开源的通用强化学习研究框架，支持单智能体、多智能体、自然语言等多种任务的训练。 OpenRL基于PyTorch进行开发，目标是为强化学习研究社区提供一个简单易用、灵活高效、可持续扩展的平台。
-目前，OpenRL支持的特性包括：
+- Provides unit testing and code coverage testing
 
-- 简单易用且支持单智能体、多智能体训练的通用接口
-- 支持自然语言任务（如对话任务）的强化学习训练
-- 支持从[Hugging Face](https://huggingface.co/)上导入模型和数据
-- 支持LSTM，GRU，Transformer等模型
-- 支持多种训练加速，例如：自动混合精度训练，半精度策略网络收集数据等
-- 支持用户自定义训练模型、奖励模型、训练数据以及环境
-- 支持[gymnasium](https://gymnasium.farama.org/)环境
-- 支持字典观测空间
-- 支持[wandb](https://wandb.ai/)，[tensorboardX](https://tensorboardx.readthedocs.io/en/latest/index.html)等主流训练可视化工具
-- 支持环境的串行和并行训练，同时保证两种模式下的训练效果一致
-- 中英文文档
-- 提供单元测试和代码覆盖测试
-- 符合Black Code Style和类型检查
-
-该框架经过了[OpenRL-Lab](https://github.com/OpenRL-Lab)的多次迭代并应用于学术研究，目前已经成为了一个成熟的强化学习框架。
-OpenRL-Lab将持续维护和更新OpenRL，欢迎大家加入我们的[开源社区](./CONTRIBUTING.md)，一起为强化学习的发展做出贡献。
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
-
-## 目录
-
-- [欢迎来到OpenRL](#欢迎来到openrl)
-- [目录](#目录)
-- [安装](#安装)
-- [使用Docker](#使用docker)
-- [快速上手](#快速上手)
-- [Gallery](#Gallery)
-- [使用OpenRL的项目](#使用OpenRL的项目)
-- [反馈和贡献](#反馈和贡献)
-- [维护人员](#维护人员)
-- [支持者](#支持者)
-  - [&#8627; Contributors](#-contributors)  
+- Compliant with Black Code Style guidelines and type checking
+
+Algorithms currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Proximal Policy Optimization (PPO)](https://arxiv.org/abs/1707.06347)
+- [Dual-clip PPO](https://arxiv.org/abs/1912.09729)
+- [Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955)
+- [Joint-ratio Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515)
+- [Generative Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476)
+- [Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf)
+- Self-Play
+- [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602)
+- [Multi-Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953)
+- [Value-Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296)
+- [Soft Actor Critic (SAC)](https://arxiv.org/abs/1812.05905)
+- [Deep Deterministic Policy Gradient (DDPG)](https://arxiv.org/abs/1509.02971)
+
+Environments currently supported by OpenRL (for more details, please refer to [Gallery](./Gallery.md)):
+- [Gymnasium](https://gymnasium.farama.org/)
+- [MuJoCo](https://github.com/deepmind/mujoco)
+- [PettingZoo](https://pettingzoo.farama.org/)
+- [MPE](https://github.com/openai/multiagent-particle-envs)
+- [Chat Bot](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
+- [Atari](https://gymnasium.farama.org/environments/atari/)
+- [StarCraft II](https://github.com/oxwhirl/smac)
+- [Omniverse Isaac Gym](https://github.com/NVIDIA-Omniverse/OmniIsaacGymEnvs)
+- [GridWorld](./examples/gridworld/)
+- [Super Mario Bros](https://github.com/Kautenja/gym-super-mario-bros)
+- [Gym Retro](https://github.com/openai/retro)
+
+This framework has undergone multiple iterations by the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in academic research. 
+It has now become a mature reinforcement learning framework.
+
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone to join our [open-source community](./CONTRIBUTING.md) 
+to contribute towards the development of reinforcement learning.
+
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
+
+## Outline
+
+- [Welcome to OpenRL](#welcome-to-openrl)
+- [Outline](#outline)
+- [Installation](#installation)
+- [Use Docker](#use-docker)
+- [Quick Start](#quick-start)
+- [Gallery](#gallery)
+- [Projects Using OpenRL](#projects-using-openrl)
+- [Feedback and Contribution](#feedback-and-contribution)
+- [Maintainers](#maintainers)
+- [Supporters](#supporters)
+  - [&#8627; Contributors](#-contributors) 
   - [&#8627; Stargazers](#-stargazers)
   - [&#8627; Forkers](#-forkers)
 - [Citing OpenRL](#citing-openrl)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
-## 安装
+## Installation
+
+Users can directly install OpenRL via pip:
 
-用户可以直接通过pip安装OpenRL:
 ```bash
 pip install openrl
 ```
 
-如果用户使用了Anaconda或者Miniconda，也可以通过conda安装OpenRL:
+If users are using Anaconda or Miniconda, they can also install OpenRL via conda:
+
 ```bash
 conda install -c openrl openrl
 ```
 
-想要修改源码的用户也可以从源码安装OpenRL:
+Users who want to modify the source code can also install OpenRL from the source code:
+
 ```bash
 git clone https://github.com/OpenRL-Lab/openrl.git && cd openrl
 pip install -e .
 ```
 
-安装完成后，用户可以直接通过命令行查看OpenRL的版本：
+After installation, users can check the version of OpenRL through command line:
+
 ```bash
 openrl --version
 ```
 
-**Tips**：无需安装，通过Colab在线试用OpenRL: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-
-## 使用Docker
+**Tips**: No installation required, try OpenRL online through Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
 
-OpenRL目前也提供了包含显卡支持和非显卡支持的Docker镜像。
-如果用户的电脑上没有英伟达显卡，则可以通过以下命令获取不包含显卡插件的镜像：
+## Use Docker
 
+OpenRL currently provides Docker images with and without GPU support. 
+If the user's computer does not have an NVIDIA GPU, they can obtain an image without the GPU plugin using the following command:
 ```bash
 sudo docker pull openrllab/openrl-cpu
 ```
 
-如果用户想要通过显卡加速训练，则可以通过以下命令获取：
+If the user wants to accelerate training with a GPU, they can obtain it using the following command:
 ```bash
 sudo docker pull openrllab/openrl
 ```
 
-镜像拉取成功后，用户可以通过以下命令运行OpenRL的Docker镜像：
+After successfully pulling the image, users can run OpenRL's Docker image using the following commands:
 ```bash
-# 不带显卡加速
+# Without GPU acceleration
 sudo docker run -it openrllab/openrl-cpu
-# 带显卡加速
+# With GPU acceleration 
 sudo docker run -it --gpus all --net host openrllab/openrl
 ```
 
-进入Docker镜像后，用户可以通过以下命令查看OpenRL的版本然后运行测例：
-```bash
-# 查看Docker镜像中OpenRL的版本
-openrl --version
-# 运行测例
-openrl --mode train --env CartPole-v1
+Once inside the Docker container, users can check OpenRL's version and then run test cases using these commands: 
+```bash 
+# Check OpenRL version in Docker container  
+openrl --version  
+# Run test case  
+openrl --mode train --env CartPole-v1  
 ```
 
+## Quick Start
 
-## 快速上手
-
-OpenRL为强化学习入门用户提供了简单易用的接口，
-下面是一个使用PPO算法训练`CartPole`环境的例子：
+OpenRL provides a simple and easy-to-use interface for beginners in reinforcement learning. 
+Below is an example of using the PPO algorithm to train the `CartPole` environment:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-env = make("CartPole-v1", env_num=9) # 创建环境，并设置环境并行数为9
-net = Net(env) # 创建神经网络
-agent = Agent(net) # 初始化智能体
-agent.train(total_time_steps=20000) # 开始训练，并设置环境运行总步数为20000
+env = make("CartPole-v1", env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network.
+agent = Agent(net) # Initialize the agent.
+agent.train(total_time_steps=20000) # Start training and set the total number of steps to 20,000 for the running environment.
 ```
-使用OpenRL训练智能体只需要简单的四步：**创建环境**=>**初始化模型**=>**初始化智能体**=>**开始训练**！
+Training an agent using OpenRL only requires four simple steps: 
+**Create Environment** => **Initialize Model** => **Initialize Agent** => **Start Training**!
 
-对于训练好的智能体，用户也可以方便地进行智能体的测试:
+For a well-trained agent, users can also easily test the agent:
 ```python
 # train_ppo.py
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
-agent = Agent(Net(make("CartPole-v1", env_num=9))) # 初始化训练器
+agent = Agent(Net(make("CartPole-v1", env_num=9))) # Initialize trainer.
 agent.train(total_time_steps=20000)
-# 创建用于测试的环境，并设置环境并行数为9，设置渲染模式为group_human
+# Create an environment for test, set the parallelism of the environment to 9, and set the rendering mode to group_human.
 env = make("CartPole-v1", env_num=9, render_mode="group_human")
-agent.set_env(env) # 训练好的智能体设置需要交互的环境
-obs, info = env.reset() # 环境进行初始化，得到初始的观测值和环境信息
+agent.set_env(env) # The agent requires an interactive environment.
+obs, info = env.reset() # Initialize the environment to obtain initial observations and environmental information.
 while True:
-    action, _ = agent.act(obs) # 智能体根据环境观测输入预测下一个动作
-    # 环境根据动作执行一步，得到下一个观测值、奖励、是否结束、环境信息
+    action, _ = agent.act(obs) # The agent predicts the next action based on environmental observations.
+    # The environment takes one step according to the action, obtains the next observation, reward, whether it ends and environmental information.
     obs, r, done, info = env.step(action)
     if any(done): break
-env.close() # 关闭测试环境
+env.close() # Close test environment
 ```
-在普通笔记本电脑上执行以上代码，只需要几秒钟，便可以完成该智能体的训练和可视化测试：
+Executing the above code on a regular laptop only takes **a few seconds**
+to complete the training. Below shows the visualization of the agent:
 
 <div align="center">
-  <img src="./docs/images/train_ppo_cartpole.gif"></a>
+  <img src="docs/images/train_ppo_cartpole.gif"></a>
 </div>
 
 
-**Tips:** 用户还可以在终端中通过执行一行命令快速训练`CartPole`环境:
+**Tips:** Users can also quickly train the `CartPole` environment by executing a command line in the terminal.
 ```bash
 openrl --mode train --env CartPole-v1
 ```
 
-对于多智能体、自然语言等任务的训练，OpenRL也提供了同样简单易用的接口。
+For training tasks such as multi-agent and natural language processing, OpenRL also provides a similarly simple and easy-to-use interface.
 
-关于如何进行多智能体训练、训练超参数设置、训练配置文件加载、wandb使用、保存gif动画等信息，请参考：
-- [多智能体训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/multi_agent_RL.html)
+For information on how to perform multi-agent training, set hyperparameters for training, load training configurations, use wandb, save GIF animations, etc., please refer to:
+- [Multi-Agent Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html)
 
-关于自然语言任务训练、Hugging Face上模型(数据)加载、自定义训练模型(奖励模型)等信息，请参考：
-- [对话任务训练例子](https://openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
+For information on natural language task training, loading models/datasets on Hugging Face, customizing training models/reward models, etc., please refer to:
+- [Dialogue Task Training Example](https://openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html)
 
-关于OpenRL的更多信息，请参考[文档](https://openrl-docs.readthedocs.io/zh/latest/)。
+For more information about OpenRL, please refer to the [documentation](https://openrl-docs.readthedocs.io/en/latest/).
 
 ## Gallery
 
-为了方便用户熟悉该框架，
-我们在[Gallery](./Gallery.md)中提供了更多使用OpenRL的示例和demo。
-也欢迎用户将自己的训练示例和demo贡献到Gallery中。
-
-## 使用OpenRL的研究项目
-
-我们在 [OpenRL Project](./Project.md) 中列举了使用OpenRL的研究项目。 
-如果你在研究项目中使用了OpenRL，也欢迎加入该列表。
-
-## 反馈和贡献
-- 有问题和发现bugs可以到 [Issues](https://github.com/OpenRL-Lab/openrl/issues) 处进行查询或提问
-- 加入QQ群：[OpenRL官方交流群](./docs/images/qq.png)
+In order to facilitate users' familiarity with the framework, we provide more examples and demos of using OpenRL in [Gallery](./Gallery.md). 
+Users are also welcome to contribute their own training examples and demos to the Gallery.
 
-<div align="center">
-    <a href="./docs/images/qq.png"><img width="250px" height="auto" src="./docs/images/qq.png"></a>
-</div>
+## Projects Using OpenRL
 
-- 加入 [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) 群组，与我们一起讨论OpenRL的使用和开发。
-- 加入 [Discord](https://discord.gg/tyy96TGbep) 群组，与我们一起讨论OpenRL的使用和开发。
-- 发送邮件到: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
-- 加入 [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
+We have listed research projects that use OpenRL in the [OpenRL Project](./Project.md). 
+If you are using OpenRL in your research project, you are also welcome to join this list.
 
-OpenRL框架目前还在持续开发和文档建设，欢迎加入我们让该项目变得更好：
+## Feedback and Contribution
+- If you have any questions or find bugs, you can check or ask in the [Issues](https://github.com/OpenRL-Lab/openrl/issues).
+- Join the QQ group: [OpenRL Official Communication Group](docs/images/qq.png)
+<div align="center">
+<a href="docs/images/qq.png"><img width="250px" height="auto" src="docs/images/qq.png"></a>
+</div>
 
-- 如何贡献代码：阅读 [贡献者手册](./CONTRIBUTING.md)
-- [OpenRL开发计划](https://github.com/OpenRL-Lab/openrl/issues/2)
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development with us.
+- Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss OpenRL usage and development with us.
+- Send an E-mail to: [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)
+- Join the [GitHub Discussion](https://github.com/orgs/OpenRL-Lab/discussions).
+
+The OpenRL framework is still under continuous development and documentation. 
+We welcome you to join us in making this project better:
+- How to contribute code: Read the [Contributors' Guide](./CONTRIBUTING.md)
+- [OpenRL Roadmap](https://github.com/OpenRL-Lab/openrl/issues/2)
 
-## 维护人员
+## Maintainers
 
-目前，OpenRL由以下维护人员维护：
+At present, OpenRL is maintained by the following maintainers:
 - [Shiyu Huang](https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13))
 - Wenze Chen([@Chen001117](https://github.com/Chen001117))
+- Yiwen Sun([@YiwenAI](https://github.com/YiwenAI))
 
-欢迎更多的贡献者加入我们的维护团队 (发送邮件到[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com)申请加入OpenRL团队)。
+Welcome more contributors to join our maintenance team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) 
+to apply for joining the OpenRL team).
 
-## 支持者
+## Supporters
 
 ### &#8627; Contributors
 
 <a href="https://github.com/OpenRL-Lab/openrl/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=OpenRL-Lab/openrl" />
 </a>
 
@@ -265,15 +332,15 @@
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们:
+If our work has been helpful to you, please feel free to cite us:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
```

#### html2text {}

```diff
@@ -1,181 +1,221 @@
-Metadata-Version: 2.1 Name: openrl Version: 0.0.9 Summary: unified
+Metadata-Version: 2.1 Name: openrl Version: 0.1.0 Summary: unified
 reinforcement learning framework Home-page: https://github.com/OpenRL-Lab/
 openrl Author: openrl contributors Author-email: huangsy1314@163.com Project-
 URL: Code, https://github.com/OpenRL-Lab/openrl Project-URL: Documentation,
 https://openrl-docs.readthedocs.io/zh/latest/ Keywords: reinforcement-learning
 multi-agent reinforcement-learning-algorithms pytorch machine-learning
 baselines toolbox python data-science gym gymnasium Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: test
-Provides-Extra: dev Provides-Extra: mpe Provides-Extra: nlp License-File:
-LICENSE License-File: LICENSE.txt
-                        [./docs/images/openrl_text.png]
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev Provides-Extra: mpe Provides-Extra:
+nlp Provides-Extra: selfplay Provides-Extra: retro Provides-Extra: super_mario
+License-File: LICENSE
+                         [docs/images/openrl_text.png]
 --- [![PyPI](https://img.shields.io/pypi/v/openrl)](https://pypi.org/project/
 openrl/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 openrl) [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/
 version.svg)](https://anaconda.org/openrl/openrl) [![Anaconda-Server Badge]
 (https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://
 anaconda.org/openrl/openrl) [![Anaconda-Server Badge](https://anaconda.org/
 openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![Hits-of-Code](https://
 hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/
 github/OpenRL-Lab/openrl/view?branch=main) [![codecov](https://codecov.io/gh/
-OpenRL-Lab/openrl/branch/main/graph/badge.svg?token=T6BqaTiT0l)](https://
-codecov.io/gh/OpenRL-Lab/openrl) [![Documentation Status](https://
+OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https:
+//codecov.io/gh/OpenRL-Lab/openrl_release) [![Documentation Status](https://
 readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-
-docs.readthedocs.io/zh/latest/?badge=latest) [![Read the Docs](https://
+docs.readthedocs.io/en/latest/?badge=latest) [![Read the Docs](https://
 img.shields.io/readthedocs/openrl-docs-
 zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-
 docs.readthedocs.io/zh/latest/) ![GitHub Org's stars](https://img.shields.io/
 github/stars/OpenRL-Lab) [![GitHub stars](https://img.shields.io/github/stars/
 OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers) [![GitHub
 forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://
 github.com/OpenRL-Lab/openrl/network) ![GitHub commit activity](https://
 img.shields.io/github/commit-activity/m/OpenRL-Lab/openrl) [![GitHub issues]
 (https://img.shields.io/github/issues/OpenRL-Lab/openrl)](https://github.com/
 OpenRL-Lab/openrl/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/pulls) [!
 [Contributors](https://img.shields.io/github/contributors/OpenRL-Lab/openrl)]
 (https://github.com/OpenRL-Lab/openrl/graphs/contributors) [![GitHub license]
 (https://img.shields.io/github/license/OpenRL-Lab/openrl)](https://github.com/
-OpenRL-Lab/openrl/blob/master/LICENSE) OpenRL-v0.0.9 is updated on May 6, 2023
-The main branch is the latest version of OpenRL, which is under active
-development. If you just want to have a try with OpenRL, you can switch to the
-stable branch. ## æ¬¢è¿æ¥å°OpenRL [English](./README_en.md) | [ä¸­æææ¡£]
-(https://openrl-docs.readthedocs.io/zh/latest/) | [Documentation](https://
-openrl-docs.readthedocs.io/en/latest/
-)
-OpenRLæ¯ä¸ä¸ªå¼æºçéç¨å¼ºåå­¦ä¹ ç ç©¶æ¡æ¶ï¼æ¯æåæºè½ä½ãå¤æºè½ä½ãèªç¶è¯­è¨ç­å¤ç§ä»»å¡çè®­ç»ã
-OpenRLåºäºPyTorchè¿è¡å¼åï¼ç®æ æ¯ä¸ºå¼ºåå­¦ä¹ ç ç©¶ç¤¾åºæä¾ä¸ä¸ªç®åæç¨ãçµæ´»é«æãå¯æç»­æ©å±çå¹³å°ã
-ç®åï¼OpenRLæ¯æçç¹æ§åæ¬ï¼ -
-ç®åæç¨ä¸æ¯æåæºè½ä½ãå¤æºè½ä½è®­ç»çéç¨æ¥å£ -
-æ¯æèªç¶è¯­è¨ä»»å¡ï¼å¦å¯¹è¯ä»»å¡ï¼çå¼ºåå­¦ä¹ è®­ç» - æ¯æä»
-[Hugging Face](https://huggingface.co/)ä¸å¯¼å¥æ¨¡ååæ°æ® -
-æ¯æLSTMï¼GRUï¼Transformerç­æ¨¡å -
-æ¯æå¤ç§è®­ç»å éï¼ä¾å¦ï¼èªå¨æ··åç²¾åº¦è®­ç»ï¼åç²¾åº¦ç­ç¥ç½ç»æ¶éæ°æ®ç­
-- æ¯æç¨æ·èªå®ä¹è®­ç»æ¨¡åãå¥å±æ¨¡åãè®­ç»æ°æ®ä»¥åç¯å¢ -
-æ¯æ[gymnasium](https://gymnasium.farama.org/)ç¯å¢ -
-æ¯æå­å¸è§æµç©ºé´ - æ¯æ[wandb](https://wandb.ai/)ï¼[tensorboardX]
-(https://tensorboardx.readthedocs.io/en/latest/
-index.html)ç­ä¸»æµè®­ç»å¯è§åå·¥å· -
-æ¯æç¯å¢çä¸²è¡åå¹¶è¡è®­ç»ï¼åæ¶ä¿è¯ä¸¤ç§æ¨¡å¼ä¸çè®­ç»ææä¸è´
-- ä¸­è±æææ¡£ - æä¾ååæµè¯åä»£ç è¦çæµè¯ - ç¬¦åBlack Code
-Styleåç±»åæ£æ¥ è¯¥æ¡æ¶ç»è¿äº[OpenRL-Lab](https://github.com/OpenRL-
-Lab)çå¤æ¬¡è¿­ä»£å¹¶åºç¨äºå­¦æ¯ç ç©¶ï¼ç®åå·²ç»æä¸ºäºä¸ä¸ªæççå¼ºåå­¦ä¹ æ¡æ¶ã
-OpenRL-Labå°æç»­ç»´æ¤åæ´æ°OpenRLï¼æ¬¢è¿å¤§å®¶å å¥æä»¬ç
-[å¼æºç¤¾åº](./
-CONTRIBUTING.md)ï¼ä¸èµ·ä¸ºå¼ºåå­¦ä¹ çåå±ååºè´¡ç®ã
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## ç®å½ - [æ¬¢è¿æ¥å°OpenRL]
-(#æ¬¢è¿æ¥å°openrl) - [ç®å½](#ç®å½) - [å®è£](#å®è£) - [ä½¿ç¨Docker]
-(#ä½¿ç¨docker) - [å¿«éä¸æ](#å¿«éä¸æ) - [Gallery](#Gallery) -
-[ä½¿ç¨OpenRLçé¡¹ç®](#ä½¿ç¨OpenRLçé¡¹ç®) - [åé¦åè´¡ç®]
-(#åé¦åè´¡ç®) - [ç»´æ¤äººå](#ç»´æ¤äººå) - [æ¯æè](#æ¯æè) -
-[↳ Contributors](#-contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers]
-(#-forkers) - [Citing OpenRL](#citing-openrl) - [License](#license) -
-[Acknowledgments](#acknowledgments) ## å®è£
-ç¨æ·å¯ä»¥ç´æ¥éè¿pipå®è£OpenRL: ```bash pip install openrl ```
-å¦æç¨æ·ä½¿ç¨äºAnacondaæèMinicondaï¼ä¹å¯ä»¥éè¿condaå®è£OpenRL:
-```bash conda install -c openrl openrl ```
-æ³è¦ä¿®æ¹æºç çç¨æ·ä¹å¯ä»¥ä»æºç å®è£OpenRL: ```bash git clone
-https://github.com/OpenRL-Lab/openrl.git && cd openrl pip install -e . ```
-å®è£å®æåï¼ç¨æ·å¯ä»¥ç´æ¥éè¿å½ä»¤è¡æ¥çOpenRLççæ¬ï¼
-```bash openrl --version ```
-**Tips**ï¼æ éå®è£ï¼éè¿Colabå¨çº¿è¯ç¨OpenRL: [![Open In Colab]
+OpenRL-Lab/openrl/blob/master/LICENSE) [![Embark](https://img.shields.io/badge/
+discord-OpenRL-%237289da.svg?logo=discord)](https://discord.gg/qfPBcVvT) [!
+[slack badge](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&)]
+(https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
+Eeh0IxQ~DIaGqYXoW2IUQg) OpenRL-v0.0.16 is updated on July 30, 2023 The main
+branch is the latest version of OpenRL, which is under active development. If
+you just want to have a try with OpenRL, you can switch to the stable branch.
+## Welcome to OpenRL [Documentation](https://openrl-docs.readthedocs.io/en/
+latest/) | [ä¸­æä»ç»](README_zh.md) | [ä¸­æææ¡£](https://openrl-
+docs.readthedocs.io/zh/latest/)
+Crafting Reinforcement Learning Frameworks with Passion, Your Valuable Insights
+                                   Welcome.
+
+OpenRL is an open-source general reinforcement learning research framework that
+supports training for various tasks such as single-agent, multi-agent, offline
+RL, self-play, and natural language. Developed based on PyTorch, the goal of
+OpenRL is to provide a simple-to-use, flexible, efficient and sustainable
+platform for the reinforcement learning research community. Currently, the
+features supported by OpenRL include: - A simple-to-use universal interface
+that supports training for both single-agent and multi-agent - Support for
+offline RL training with expert dataset - Support self-play training -
+Reinforcement learning training support for natural language tasks (such as
+dialogue) - Importing models and datasets from [Hugging Face](https://
+huggingface.co/) - Support for models such as LSTM, GRU, Transformer etc. -
+Multiple training acceleration methods including automatic mixed precision
+training and data collecting wth half precision policy network - User-defined
+training models, reward models, training data and environment support - Support
+for [gymnasium](https://gymnasium.farama.org/) environments - Support for
+[Callbacks](https://openrl-docs.readthedocs.io/en/latest/callbacks/index.html),
+which can be used to implement various functions such as logging, saving, and
+early stopping - Dictionary observation space support - Popular visualization
+tools such as [wandb](https://wandb.ai/), [tensorboardX](https://
+tensorboardx.readthedocs.io/en/latest/index.html) are supported - Serial or
+parallel environment training while ensuring consistent results in both modes -
+Chinese and English documentation - Provides unit testing and code coverage
+testing - Compliant with Black Code Style guidelines and type checking
+Algorithms currently supported by OpenRL (for more details, please refer to
+[Gallery](./Gallery.md)): - [Proximal Policy Optimization (PPO)](https://
+arxiv.org/abs/1707.06347) - [Dual-clip PPO](https://arxiv.org/abs/1912.09729) -
+[Multi-agent PPO (MAPPO)](https://arxiv.org/abs/2103.01955) - [Joint-ratio
+Policy Optimization (JRPO)](https://arxiv.org/abs/2302.07515) - [Generative
+Adversarial Imitation Learning (GAIL)](https://arxiv.org/abs/1606.03476) -
+[Behavior Cloning (BC)](http://www.cse.unsw.edu.au/~claude/papers/MI15.pdf) -
+Self-Play - [Deep Q-Network (DQN)](https://arxiv.org/abs/1312.5602) - [Multi-
+Agent Transformer (MAT)](https://arxiv.org/abs/2205.14953) - [Value-
+Decomposition Network (VDN)](https://arxiv.org/abs/1706.05296) - [Soft Actor
+Critic (SAC)](https://arxiv.org/abs/1812.05905) - [Deep Deterministic Policy
+Gradient (DDPG)](https://arxiv.org/abs/1509.02971) Environments currently
+supported by OpenRL (for more details, please refer to [Gallery](./
+Gallery.md)): - [Gymnasium](https://gymnasium.farama.org/) - [MuJoCo](https://
+github.com/deepmind/mujoco) - [PettingZoo](https://pettingzoo.farama.org/) -
+[MPE](https://github.com/openai/multiagent-particle-envs) - [Chat Bot](https://
+openrl-docs.readthedocs.io/en/latest/quick_start/train_nlp.html) - [Atari]
+(https://gymnasium.farama.org/environments/atari/) - [StarCraft II](https://
+github.com/oxwhirl/smac) - [Omniverse Isaac Gym](https://github.com/NVIDIA-
+Omniverse/OmniIsaacGymEnvs) - [GridWorld](./examples/gridworld/) - [Super Mario
+Bros](https://github.com/Kautenja/gym-super-mario-bros) - [Gym Retro](https://
+github.com/openai/retro) This framework has undergone multiple iterations by
+the [OpenRL-Lab](https://github.com/OpenRL-Lab) team which has applied it in
+academic research. It has now become a mature reinforcement learning framework.
+OpenRL-Lab will continue to maintain and update OpenRL, and we welcome everyone
+to join our [open-source community](./CONTRIBUTING.md) to contribute towards
+the development of reinforcement learning. For more information about OpenRL,
+please refer to the [documentation](https://openrl-docs.readthedocs.io/en/
+latest/). ## Outline - [Welcome to OpenRL](#welcome-to-openrl) - [Outline]
+(#outline) - [Installation](#installation) - [Use Docker](#use-docker) - [Quick
+Start](#quick-start) - [Gallery](#gallery) - [Projects Using OpenRL](#projects-
+using-openrl) - [Feedback and Contribution](#feedback-and-contribution) -
+[Maintainers](#maintainers) - [Supporters](#supporters) - [↳ Contributors](#-
+contributors) - [↳ Stargazers](#-stargazers) - [↳ Forkers](#-forkers) - [Citing
+OpenRL](#citing-openrl) - [License](#license) - [Acknowledgments]
+(#acknowledgments) ## Installation Users can directly install OpenRL via pip:
+```bash pip install openrl ``` If users are using Anaconda or Miniconda, they
+can also install OpenRL via conda: ```bash conda install -c openrl openrl ```
+Users who want to modify the source code can also install OpenRL from the
+source code: ```bash git clone https://github.com/OpenRL-Lab/openrl.git && cd
+openrl pip install -e . ``` After installation, users can check the version of
+OpenRL through command line: ```bash openrl --version ``` **Tips**: No
+installation required, try OpenRL online through Colab: [![Open In Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/15VBA-B7AJF8dBazzRcWAxJxZI7Pl9m-g?usp=sharing)
-## ä½¿ç¨Docker
-OpenRLç®åä¹æä¾äºåå«æ¾å¡æ¯æåéæ¾å¡æ¯æçDockeréåã
-å¦æç¨æ·ççµèä¸æ²¡æè±ä¼è¾¾æ¾å¡ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åä¸åå«æ¾å¡æä»¶çéåï¼
-```bash sudo docker pull openrllab/openrl-cpu ```
-å¦æç¨æ·æ³è¦éè¿æ¾å¡å éè®­ç»ï¼åå¯ä»¥éè¿ä»¥ä¸å½ä»¤è·åï¼
-```bash sudo docker pull openrllab/openrl ```
-éåæåæååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤è¿è¡OpenRLçDockeréåï¼
-```bash # ä¸å¸¦æ¾å¡å é sudo docker run -it openrllab/openrl-cpu #
-å¸¦æ¾å¡å é sudo docker run -it --gpus all --net host openrllab/openrl ```
-è¿å¥Dockeréååï¼ç¨æ·å¯ä»¥éè¿ä»¥ä¸å½ä»¤æ¥çOpenRLççæ¬ç¶åè¿è¡æµä¾ï¼
-```bash # æ¥çDockeréåä¸­OpenRLççæ¬ openrl --version # è¿è¡æµä¾
-openrl --mode train --env CartPole-v1 ``` ## å¿«éä¸æ
-OpenRLä¸ºå¼ºåå­¦ä¹ å¥é¨ç¨æ·æä¾äºç®åæç¨çæ¥å£ï¼
-ä¸é¢æ¯ä¸ä¸ªä½¿ç¨PPOç®æ³è®­ç»`CartPole`ç¯å¢çä¾å­ï¼ ```python #
-train_ppo.py from openrl.envs.common import make from openrl.modules.common
-import PPONet as Net from openrl.runners.common import PPOAgent as Agent env =
-make("CartPole-v1", env_num=9) # åå»ºç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9
-net = Net(env) # åå»ºç¥ç»ç½ç» agent = Agent(net) # åå§åæºè½ä½
-agent.train(total_time_steps=20000) #
-å¼å§è®­ç»ï¼å¹¶è®¾ç½®ç¯å¢è¿è¡æ»æ­¥æ°ä¸º20000 ```
-ä½¿ç¨OpenRLè®­ç»æºè½ä½åªéè¦ç®åçåæ­¥ï¼**åå»ºç¯å¢**=>**åå§åæ¨¡å**=>**åå§åæºè½ä½**=>**å¼å§è®­ç»**ï¼
-å¯¹äºè®­ç»å¥½çæºè½ä½ï¼ç¨æ·ä¹å¯ä»¥æ¹ä¾¿å°è¿è¡æºè½ä½çæµè¯:
-```python # train_ppo.py from openrl.envs.common import make from
-openrl.modules.common import PPONet as Net from openrl.runners.common import
-PPOAgent as Agent agent = Agent(Net(make("CartPole-v1", env_num=9))) #
-åå§åè®­ç»å¨ agent.train(total_time_steps=20000) #
-åå»ºç¨äºæµè¯çç¯å¢ï¼å¹¶è®¾ç½®ç¯å¢å¹¶è¡æ°ä¸º9ï¼è®¾ç½®æ¸²ææ¨¡å¼ä¸ºgroup_human
-env = make("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env
-(env) # è®­ç»å¥½çæºè½ä½è®¾ç½®éè¦äº¤äºçç¯å¢ obs, info = env.reset
-() # ç¯å¢è¿è¡åå§åï¼å¾å°åå§çè§æµå¼åç¯å¢ä¿¡æ¯ while
-True: action, _ = agent.act(obs) #
-æºè½ä½æ ¹æ®ç¯å¢è§æµè¾å¥é¢æµä¸ä¸ä¸ªå¨ä½ #
-ç¯å¢æ ¹æ®å¨ä½æ§è¡ä¸æ­¥ï¼å¾å°ä¸ä¸ä¸ªè§æµå¼ãå¥å±ãæ¯å¦ç»æãç¯å¢ä¿¡æ¯
-obs, r, done, info = env.step(action) if any(done): break env.close() #
-å³é­æµè¯ç¯å¢ ```
-å¨æ®éç¬è®°æ¬çµèä¸æ§è¡ä»¥ä¸ä»£ç ï¼åªéè¦å ç§éï¼ä¾¿å¯ä»¥å®æè¯¥æºè½ä½çè®­ç»åå¯è§åæµè¯ï¼
-                    [./docs/images/train_ppo_cartpole.gif]
-**Tips:**
-ç¨æ·è¿å¯ä»¥å¨ç»ç«¯ä¸­éè¿æ§è¡ä¸è¡å½ä»¤å¿«éè®­ç»`CartPole`ç¯å¢:
-```bash openrl --mode train --env CartPole-v1 ```
-å¯¹äºå¤æºè½ä½ãèªç¶è¯­è¨ç­ä»»å¡çè®­ç»ï¼OpenRLä¹æä¾äºåæ ·ç®åæç¨çæ¥å£ã
-å³äºå¦ä½è¿è¡å¤æºè½ä½è®­ç»ãè®­ç»è¶åæ°è®¾ç½®ãè®­ç»éç½®æä»¶å è½½ãwandbä½¿ç¨ãä¿å­gifå¨ç»ç­ä¿¡æ¯ï¼è¯·åèï¼
-- [å¤æºè½ä½è®­ç»ä¾å­](https://openrl-docs.readthedocs.io/zh/latest/
-quick_start/multi_agent_RL.html) å³äºèªç¶è¯­è¨ä»»å¡è®­ç»ãHugging
-Faceä¸æ¨¡å(æ°æ®)å è½½ãèªå®ä¹è®­ç»æ¨¡å
-(å¥å±æ¨¡å)ç­ä¿¡æ¯ï¼è¯·åèï¼ - [å¯¹è¯ä»»å¡è®­ç»ä¾å­](https://
-openrl-docs.readthedocs.io/zh/latest/quick_start/train_nlp.html)
-å³äºOpenRLçæ´å¤ä¿¡æ¯ï¼è¯·åè[ææ¡£](https://openrl-
-docs.readthedocs.io/zh/latest/)ã ## Gallery
-ä¸ºäºæ¹ä¾¿ç¨æ·çæè¯¥æ¡æ¶ï¼ æä»¬å¨[Gallery](./
-Gallery.md)ä¸­æä¾äºæ´å¤ä½¿ç¨OpenRLçç¤ºä¾ådemoã
-ä¹æ¬¢è¿ç¨æ·å°èªå·±çè®­ç»ç¤ºä¾ådemoè´¡ç®å°Galleryä¸­ã ##
-ä½¿ç¨OpenRLçç ç©¶é¡¹ç® æä»¬å¨ [OpenRL Project](./Project.md)
-ä¸­åä¸¾äºä½¿ç¨OpenRLçç ç©¶é¡¹ç®ã
-å¦æä½ å¨ç ç©¶é¡¹ç®ä¸­ä½¿ç¨äºOpenRLï¼ä¹æ¬¢è¿å å¥è¯¥åè¡¨ã ##
-åé¦åè´¡ç® - æé®é¢ååç°bugså¯ä»¥å° [Issues](https://github.com/
-OpenRL-Lab/openrl/issues) å¤è¿è¡æ¥è¯¢ææé® - å å¥QQç¾¤ï¼
-[OpenRLå®æ¹äº¤æµç¾¤](./docs/images/qq.png)
-                            [./docs/images/qq.png]
-- å å¥ [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-1tqwpvthd-
-Eeh0IxQ~DIaGqYXoW2IUQg)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - å å¥ [Discord]
-(https://discord.gg/tyy96TGbep)
-ç¾¤ç»ï¼ä¸æä»¬ä¸èµ·è®¨è®ºOpenRLçä½¿ç¨åå¼åã - åéé®ä»¶å°:
-[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - å å¥ [GitHub
-Discussion](https://github.com/orgs/OpenRL-Lab/discussions)
-OpenRLæ¡æ¶ç®åè¿å¨æç»­å¼ååææ¡£å»ºè®¾ï¼æ¬¢è¿å å¥æä»¬è®©è¯¥é¡¹ç®åå¾æ´å¥½ï¼
-- å¦ä½è´¡ç®ä»£ç ï¼éè¯» [è´¡ç®èæå](./CONTRIBUTING.md) -
-[OpenRLå¼åè®¡å](https://github.com/OpenRL-Lab/openrl/issues/2) ##
-ç»´æ¤äººå ç®åï¼OpenRLç±ä»¥ä¸ç»´æ¤äººåç»´æ¤ï¼ - [Shiyu Huang]
-(https://huangshiyu13.github.io/)([@huangshiyu13](https://github.com/
-huangshiyu13)) - Wenze Chen([@Chen001117](https://github.com/Chen001117))
-æ¬¢è¿æ´å¤çè´¡ç®èå å¥æä»¬çç»´æ¤å¢é (åéé®ä»¶å°
-[huangshiyu@4paradigm.com]
-(huangshiyu@4paradigm.com)ç³è¯·å å¥OpenRLå¢é)ã ## æ¯æè ### ↳
-Contributors [https://contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳
-Stargazers [![Stargazers repo roster for @OpenRL-Lab/openrl](https://
-reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/
-stargazers) ### ↳ Forkers [![Forkers repo roster for @OpenRL-Lab/openrl](https:
-//reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/
-openrl/network/members) ## Citing OpenRL
-å¦ææä»¬çå·¥ä½å¯¹ä½ æå¸®å©ï¼æ¬¢è¿å¼ç¨æä»¬: ```latex @misc
+## Use Docker OpenRL currently provides Docker images with and without GPU
+support. If the user's computer does not have an NVIDIA GPU, they can obtain an
+image without the GPU plugin using the following command: ```bash sudo docker
+pull openrllab/openrl-cpu ``` If the user wants to accelerate training with a
+GPU, they can obtain it using the following command: ```bash sudo docker pull
+openrllab/openrl ``` After successfully pulling the image, users can run
+OpenRL's Docker image using the following commands: ```bash # Without GPU
+acceleration sudo docker run -it openrllab/openrl-cpu # With GPU acceleration
+sudo docker run -it --gpus all --net host openrllab/openrl ``` Once inside the
+Docker container, users can check OpenRL's version and then run test cases
+using these commands: ```bash # Check OpenRL version in Docker container openrl
+--version # Run test case openrl --mode train --env CartPole-v1 ``` ## Quick
+Start OpenRL provides a simple and easy-to-use interface for beginners in
+reinforcement learning. Below is an example of using the PPO algorithm to train
+the `CartPole` environment: ```python # train_ppo.py from openrl.envs.common
+import make from openrl.modules.common import PPONet as Net from
+openrl.runners.common import PPOAgent as Agent env = make("CartPole-v1",
+env_num=9) # Create an environment and set the environment parallelism to 9.
+net = Net(env) # Create neural network. agent = Agent(net) # Initialize the
+agent. agent.train(total_time_steps=20000) # Start training and set the total
+number of steps to 20,000 for the running environment. ``` Training an agent
+using OpenRL only requires four simple steps: **Create Environment** =>
+**Initialize Model** => **Initialize Agent** => **Start Training**! For a well-
+trained agent, users can also easily test the agent: ```python # train_ppo.py
+from openrl.envs.common import make from openrl.modules.common import PPONet as
+Net from openrl.runners.common import PPOAgent as Agent agent = Agent(Net(make
+("CartPole-v1", env_num=9))) # Initialize trainer. agent.train
+(total_time_steps=20000) # Create an environment for test, set the parallelism
+of the environment to 9, and set the rendering mode to group_human. env = make
+("CartPole-v1", env_num=9, render_mode="group_human") agent.set_env(env) # The
+agent requires an interactive environment. obs, info = env.reset() # Initialize
+the environment to obtain initial observations and environmental information.
+while True: action, _ = agent.act(obs) # The agent predicts the next action
+based on environmental observations. # The environment takes one step according
+to the action, obtains the next observation, reward, whether it ends and
+environmental information. obs, r, done, info = env.step(action) if any(done):
+break env.close() # Close test environment ``` Executing the above code on a
+regular laptop only takes **a few seconds** to complete the training. Below
+shows the visualization of the agent:
+                     [docs/images/train_ppo_cartpole.gif]
+**Tips:** Users can also quickly train the `CartPole` environment by executing
+a command line in the terminal. ```bash openrl --mode train --env CartPole-v1
+``` For training tasks such as multi-agent and natural language processing,
+OpenRL also provides a similarly simple and easy-to-use interface. For
+information on how to perform multi-agent training, set hyperparameters for
+training, load training configurations, use wandb, save GIF animations, etc.,
+please refer to: - [Multi-Agent Training Example](https://openrl-
+docs.readthedocs.io/en/latest/quick_start/multi_agent_RL.html) For information
+on natural language task training, loading models/datasets on Hugging Face,
+customizing training models/reward models, etc., please refer to: - [Dialogue
+Task Training Example](https://openrl-docs.readthedocs.io/en/latest/
+quick_start/train_nlp.html) For more information about OpenRL, please refer to
+the [documentation](https://openrl-docs.readthedocs.io/en/latest/). ## Gallery
+In order to facilitate users' familiarity with the framework, we provide more
+examples and demos of using OpenRL in [Gallery](./Gallery.md). Users are also
+welcome to contribute their own training examples and demos to the Gallery. ##
+Projects Using OpenRL We have listed research projects that use OpenRL in the
+[OpenRL Project](./Project.md). If you are using OpenRL in your research
+project, you are also welcome to join this list. ## Feedback and Contribution -
+If you have any questions or find bugs, you can check or ask in the [Issues]
+(https://github.com/OpenRL-Lab/openrl/issues). - Join the QQ group: [OpenRL
+Official Communication Group](docs/images/qq.png)
+                             [docs/images/qq.png]
+- Join the [slack](https://join.slack.com/t/openrlhq/shared_invite/zt-
+1tqwpvthd-Eeh0IxQ~DIaGqYXoW2IUQg) group to discuss OpenRL usage and development
+with us. - Join the [Discord](https://discord.gg/qfPBcVvT) group to discuss
+OpenRL usage and development with us. - Send an E-mail to:
+[huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) - Join the [GitHub
+Discussion](https://github.com/orgs/OpenRL-Lab/discussions). The OpenRL
+framework is still under continuous development and documentation. We welcome
+you to join us in making this project better: - How to contribute code: Read
+the [Contributors' Guide](./CONTRIBUTING.md) - [OpenRL Roadmap](https://
+github.com/OpenRL-Lab/openrl/issues/2) ## Maintainers At present, OpenRL is
+maintained by the following maintainers: - [Shiyu Huang](https://
+huangshiyu13.github.io/)([@huangshiyu13](https://github.com/huangshiyu13)) -
+Wenze Chen([@Chen001117](https://github.com/Chen001117)) - Yiwen Sun([@YiwenAI]
+(https://github.com/YiwenAI)) Welcome more contributors to join our maintenance
+team (send an E-mail to [huangshiyu@4paradigm.com](huangshiyu@4paradigm.com) to
+apply for joining the OpenRL team). ## Supporters ### ↳ Contributors [https://
+contrib.rocks/image?repo=OpenRL-Lab/openrl] ### ↳ Stargazers [![Stargazers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/stargazers) ### ↳ Forkers [![Forkers repo
+roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)]
+(https://github.com/OpenRL-Lab/openrl/network/members) ## Citing OpenRL If our
+work has been helpful to you, please feel free to cite us: ```latex @misc
 {openrl2023, title={OpenRL}, author={OpenRL Contributors}, publisher =
 {GitHub}, howpublished = {\url{https://github.com/OpenRL-Lab/openrl}}, year=
 {2023}, } ``` ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/
 #OpenRL-Lab/openrl&Date) ## License OpenRL under the Apache 2.0 license. ##
 Acknowledgments The development of the OpenRL framework has drawn on the
 strengths of other reinforcement learning frameworks: - Stable-baselines3:
```

### Comparing `openrl-0.0.9/setup.py` & `openrl-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,37 +34,43 @@
         "rich",
         "wandb",
         "seaborn",
         "jsonargparse",
         "imageio",
         "opencv-python",
         "pygame",
+        "mujoco",
+        "tqdm",
     ]
 
 
 def get_extra_requires() -> dict:
     req = {
         "test": [
             "pytest",
             "pytest-cov",
             "mypy",
             "isort",
             "black",
             "ruff",
             "gpustat",
+            "gym-super-mario-bros",
         ],
         "dev": ["build", "twine"],
         "mpe": ["pyglet==1.5.27"],
         "nlp": [
             "transformers==4.18.0",
             "datasets",
             "nltk",
             "evaluate",
             "icetk",
         ],
+        "selfplay": ["ray[default]", "ray[serve]", "pettingzoo[classic]"],
+        "retro": ["gym-retro"],
+        "super_mario": ["gym-super-mario-bros"],
     }
     return req
 
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
     init = open(os.path.join("openrl", "__init__.py"), "r").read().split()
@@ -89,14 +95,16 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     keywords=(
         "reinforcement-learning multi-agent "
         "reinforcement-learning-algorithms pytorch machine-learning "
         "baselines toolbox python data-science gym gymnasium"
```

### Comparing `openrl-0.0.9/tests/__init__.py` & `openrl-0.1.0/openrl/selfplay/opponents/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/tests/project/__init__.py` & `openrl-0.1.0/openrl/selfplay/selfplay_api/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/tests/project/test_version.py` & `openrl-0.1.0/tests/project/test_version.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/tests/test_buffer/__init__.py` & `openrl-0.1.0/openrl/selfplay/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.9/tests/test_buffer/test_buffer.py` & `openrl-0.1.0/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*

