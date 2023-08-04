# Comparing `tmp/alpaca_eval-0.2.7.tar.gz` & `tmp/alpaca_eval-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.7.tar", last modified: Mon Jul 31 02:10:28 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.8.tar", last modified: Fri Aug  4 10:30:00 2023, max compression
```

## Comparing `alpaca_eval-0.2.7.tar` & `alpaca_eval-0.2.8.tar`

### file list

```diff
@@ -1,234 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66684 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.194441 alpaca_eval-0.2.7/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.182441 alpaca_eval-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.198441 alpaca_eval-0.2.7/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 02:10:11.000000 alpaca_eval-0.2.7/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/decoders/replicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.206441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.206441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.210441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.186441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23982 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.194441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.214441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.218441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b-api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.222441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v3.1-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.226441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.230441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.202441 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 02:10:28.000000 alpaca_eval-0.2.7/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:10:28.234441 alpaca_eval-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-31 02:09:52.000000 alpaca_eval-0.2.7/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-08-04 10:29:31.000000 alpaca_eval-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-04 10:29:31.000000 alpaca_eval-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    69479 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    68657 2023-08-04 10:29:31.000000 alpaca_eval-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.967764 alpaca_eval-0.2.8/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-08-04 10:29:31.000000 alpaca_eval-0.2.8/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.955764 alpaca_eval-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.971765 alpaca_eval-0.2.8/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 10:29:44.000000 alpaca_eval-0.2.8/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.971765 alpaca_eval-0.2.8/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28881 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.971765 alpaca_eval-0.2.8/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/decoders/replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.975765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.975765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.975765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.975765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.975765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.979765 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.959764 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24223 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.967764 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.983765 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-33b-api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.987766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.991766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v3.1-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.995766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.971765 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    69479 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 10:29:59.000000 alpaca_eval-0.2.8/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:29:59.999766 alpaca_eval-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-04 10:29:32.000000 alpaca_eval-0.2.8/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.7/LICENSE` & `alpaca_eval-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/PKG-INFO` & `alpaca_eval-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.7
+Version: 0.2.8
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -81,14 +81,15 @@
 4. [Analysis](#additional-analysis-and-plots)
     - [Analyzing an evaluator](#analyzing-an-evaluator)
     - [Analyzing an eval set](#analyzing-an-eval-set)
 5. [Contributing](#contributing)
     - [Contributing a model](#contributing-a-model)
     - [Contributing an evaluator](#contributing-an-evaluator)
     - [Contributing an eval set](#contributing-an-eval-set)
+    - [Contributing a completion function](#contributing-a-completion-function)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
     - [Major updates](#major-updates)
@@ -1049,15 +1050,15 @@
 Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4' 
+  --annotators_config 'alpaca_eval_gpt4'
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
@@ -1118,14 +1119,31 @@
   --reference_outputs <path_to_json_file>
 ```
 
 Please submit a PR with the eval set json and corresponding leaderboard csv.
 
 </details>
 
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Contributing a completion function</h2></summary>
+
+Currently, we allow different completion functions, e.g., `openai`, `anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to contribute a new completion function / API with which to perform inference then follow those steps:
+1. add a file <name>.py with a function  `<name>_completions(prompts : Sequence[str], model_name :str, ... )`  in the [decoder folder](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This function should take as argument the prompts + kwargs and return the completions. Please look at other completion functions in the directory for templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or [anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/anthropic.py).
+2. add `<name>_completions` and dependencies in [__init__](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py) . Again you can follow the example of [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py#L30)
+3. update optional dependencies in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py)
+4. add a model you want to evaluate in the [models configs](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs)
+5. evaluate your model using `alpaca_eval evaluate_from_model --model_configs '<model_configs>'`
+6. (optional) push the results from the previous model on AlpacaEval leaderboard following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/main#contributing-a-model)
+
+Feel free to start a PR early, we'll be able to provide some help in the process! 
+
+</details>
+
 # Limitations
 
 The AlpacaEval evaluation pipeline, like other current evaluators have important limitations and should therefore not be
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.7 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.8 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -60,27 +60,28 @@
 them) - [Models](#models) - [Evaluators](#evaluators) 3. [Use-cases](#use-
 cases) - [Evaluating a model](#evaluating-a-model) - [Making a new leaderboard]
 (#making-a-new-leaderboard) - [Making a new evaluator](#making-a-new-evaluator)
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
-set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
-(#citation) 8. [Additional information](#additional-information) - [Data
-Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
-# Quick Start To install the stable release, run ```bash pip install alpaca-
-eval ``` To install the nightly version, run ```bash pip install git+https://
-github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
-export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
-this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` This will print the leaderboard to the console, and save both
-the leaderboard and the annotations to the same directory as the
-`model_outputs` file. Important parameters are the following: -
-**model_outputs** : A path to a json file for the outputs of the model to add
+set](#contributing-an-eval-set) - [Contributing a completion function]
+(#contributing-a-completion-function) 6. [Limitations](#limitations) 7.
+[Citation](#citation) 8. [Additional information](#additional-information) -
+[Data Release](#data-release) - [Differences with AlpacaFarm](#differences-
+with-alpacafarm) - [Related work](#related-work) - [Major updates](#major-
+updates)  # Quick Start To install the stable release, run ```bash pip install
+alpaca-eval ``` To install the nightly version, run ```bash pip install
+git+https://github.com/tatsu-lab/alpaca_eval ``` Then you can use it as
+follows: ```bash export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= #
+Optional; if not set, this will be your default org id. alpaca_eval --
+model_outputs 'example/outputs.json' ``` This will print the leaderboard to the
+console, and save both the leaderboard and the annotations to the same
+directory as the `model_outputs` file. Important parameters are the following:
+- **model_outputs** : A path to a json file for the outputs of the model to add
 to the leaderboard. Each dictionary should contain the keys `instruction` and
 `output`. - **annotators_config**: This is the annotator to use (e.g.,
 `alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
 has the highest agreement rate with our human annotation data. `claude` has a
 decent agreement and is free for academics. `chatgpt_fn` is the worst of the
 three, but is available to everyone, cheap, and has 2x larger context window
 (16K tokens). For a comparison of annotators see [here](#evaluators). -
@@ -655,58 +656,82 @@
 [alpaca_eval.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/
 main/alpaca_eval.json) as a guide (the `dataset` field is not necessary).
 Finally, we ask that you create a minimal leaderboard on this new evaluation
 set. You can do this with the following: ```bash alpaca_eval make_leaderboard \
 --leaderboard_path
 lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
 all_model_outputs alpaca_eval_all_outputs.json \ --reference_outputs  ```
-Please submit a PR with the eval set json and corresponding leaderboard csv.  #
-Limitations The AlpacaEval evaluation pipeline, like other current evaluators
-have important limitations and should therefore not be used as replacement for
-human evaluation in important settings, such as to decide whether a model is
-ready to be deployed. Those can broadly be clustered into 3 categories: 1.
-**Instructions might not be representative of real-usage**: the AlpacaEval set
-contains examples from a variety of datasets ([self-instruct](https://
-github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
-datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
-[vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
-github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
-datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
-representative of real-usage and advanced applications of better models like
-GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
-seem more similar to the open models than what they are. Indeed, those closed
-models seem to be pretrained/finetuned on much more diverse data. See for
-example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
-more complex instructions. Note, however, that in [AlpacaFarm](https://
-arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
-highly correlated (0.97 R2) with win-rates on instructions from user
-interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
-shows larger gap between the open models and OpenAI models than other
-leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
-**Biases of automatic annotators**: the automatic annotators seem to have
-implicit biases. In particular, we found that they tend to prefer longer
-outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
-and 0.62 / 0.58 for `claude`). Although we found that humans have similar
-biases (0.64 / 0.61), we believe that this could be more of a limitation of
-human annotation pipeline we used rather than a true human bias. More
-generally, through qualitative analysis, we found that automatic annotators
-give more importance to the style of the output than its content (e.g.
-factuality). Finally, we found that automatic evaluators tend to prefer outputs
-from models that are similar (likely trained on the same data) as suggested by
-the big difference between ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s
-leaderboard. 3. **Lack of safety evaluation**: importantly, AlpacaEval only
-evaluates the instruction-following capabilities of models rather than the harm
-that they could cause (e.g. toxic behavior or bias). As a result the small gap
-between current ChatGPT and the best open source models **should not** be
-interpreted as if that the latter are ready to be deployed. Beyond those
-limitations about the evaluation pipelines, there are also limitations about
-our validation of the evaluators and our [proposed approach](#analyzing-an-
-eval-set) to selecting evaluation sets.  Limitations about our validation
-pipeline
+Please submit a PR with the eval set json and corresponding leaderboard csv.
+***** Contributing a completion function *****
+Currently, we allow different completion functions, e.g., `openai`,
+`anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to
+contribute a new completion function / API with which to perform inference then
+follow those steps: 1. add a file .py with a function `_completions(prompts :
+Sequence[str], model_name :str, ... )` in the [decoder folder](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This
+function should take as argument the prompts + kwargs and return the
+completions. Please look at other completion functions in the directory for
+templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/
+alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or
+[anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+decoders/anthropic.py). 2. add `_completions` and dependencies in [__init__]
+(https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/
+__init__.py) . Again you can follow the example of
+[huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/
+main/src/alpaca_eval/decoders/__init__.py#L30) 3. update optional dependencies
+in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py) 4.
+add a model you want to evaluate in the [models configs](https://github.com/
+tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) 5. evaluate
+your model using `alpaca_eval evaluate_from_model --model_configs ''` 6.
+(optional) push the results from the previous model on AlpacaEval leaderboard
+following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/
+main#contributing-a-model) Feel free to start a PR early, we'll be able to
+provide some help in the process!  # Limitations The AlpacaEval evaluation
+pipeline, like other current evaluators have important limitations and should
+therefore not be used as replacement for human evaluation in important
+settings, such as to decide whether a model is ready to be deployed. Those can
+broadly be clustered into 3 categories: 1. **Instructions might not be
+representative of real-usage**: the AlpacaEval set contains examples from a
+variety of datasets ([self-instruct](https://github.com/yizhongw/self-
+instruct), [open-assistant](https://huggingface.co/datasets/OpenAssistant/
+oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/
+blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-
+test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/
+Anthropic--hh-rlhf/test)) which might not be representative of real-usage and
+advanced applications of better models like GPT4. This likely makes the best
+closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open
+models than what they are. Indeed, those closed models seem to be pretrained/
+finetuned on much more diverse data. See for example [this blog](https://
+medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-
+harder-tasks-aa0395c31610) for preliminary results on more complex
+instructions. Note, however, that in [AlpacaFarm](https://arxiv.org/abs/
+2305.14387) we showed that win-rates on our evaluation set are highly
+correlated (0.97 R2) with win-rates on instructions from user interactions with
+the Alpaca Demo. Furthermore, the AlpacaEval leaderboard shows larger gap
+between the open models and OpenAI models than other leaderboards ( e.g.
+[lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2. **Biases of automatic
+annotators**: the automatic annotators seem to have implicit biases. In
+particular, we found that they tend to prefer longer outputs and outputs that
+contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4` and 0.62 / 0.58 for
+`claude`). Although we found that humans have similar biases (0.64 / 0.61), we
+believe that this could be more of a limitation of human annotation pipeline we
+used rather than a true human bias. More generally, through qualitative
+analysis, we found that automatic annotators give more importance to the style
+of the output than its content (e.g. factuality). Finally, we found that
+automatic evaluators tend to prefer outputs from models that are similar
+(likely trained on the same data) as suggested by the big difference between
+ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s leaderboard. 3. **Lack of
+safety evaluation**: importantly, AlpacaEval only evaluates the instruction-
+following capabilities of models rather than the harm that they could cause
+(e.g. toxic behavior or bias). As a result the small gap between current
+ChatGPT and the best open source models **should not** be interpreted as if
+that the latter are ready to be deployed. Beyond those limitations about the
+evaluation pipelines, there are also limitations about our validation of the
+evaluators and our [proposed approach](#analyzing-an-eval-set) to selecting
+evaluation sets.  Limitations about our validation pipeline
  First, our validation of evaluators based on human cross-annotations suffers
 from the following limitations: (1) we qualitatively found that our crowd-
 workers tend to also favor style such as length and presence of lists over
 factuality; (2) this does not validate whether win-rates against a reference
 model is a good evaluation strategy in the first place; (3) preferences from 16
 crowd-workers are not representative of preferences of all humans. Second, our
 suggested approach to selecting evaluation sets based on statistical power
```

### Comparing `alpaca_eval-0.2.7/README.md` & `alpaca_eval-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 4. [Analysis](#additional-analysis-and-plots)
     - [Analyzing an evaluator](#analyzing-an-evaluator)
     - [Analyzing an eval set](#analyzing-an-eval-set)
 5. [Contributing](#contributing)
     - [Contributing a model](#contributing-a-model)
     - [Contributing an evaluator](#contributing-an-evaluator)
     - [Contributing an eval set](#contributing-an-eval-set)
+    - [Contributing a completion function](#contributing-a-completion-function)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
     - [Major updates](#major-updates)
@@ -1026,15 +1027,15 @@
 Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4' 
+  --annotators_config 'alpaca_eval_gpt4'
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
@@ -1095,14 +1096,31 @@
   --reference_outputs <path_to_json_file>
 ```
 
 Please submit a PR with the eval set json and corresponding leaderboard csv.
 
 </details>
 
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Contributing a completion function</h2></summary>
+
+Currently, we allow different completion functions, e.g., `openai`, `anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to contribute a new completion function / API with which to perform inference then follow those steps:
+1. add a file <name>.py with a function  `<name>_completions(prompts : Sequence[str], model_name :str, ... )`  in the [decoder folder](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This function should take as argument the prompts + kwargs and return the completions. Please look at other completion functions in the directory for templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or [anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/anthropic.py).
+2. add `<name>_completions` and dependencies in [__init__](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py) . Again you can follow the example of [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py#L30)
+3. update optional dependencies in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py)
+4. add a model you want to evaluate in the [models configs](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs)
+5. evaluate your model using `alpaca_eval evaluate_from_model --model_configs '<model_configs>'`
+6. (optional) push the results from the previous model on AlpacaEval leaderboard following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/main#contributing-a-model)
+
+Feel free to start a PR early, we'll be able to provide some help in the process! 
+
+</details>
+
 # Limitations
 
 The AlpacaEval evaluation pipeline, like other current evaluators have important limitations and should therefore not be
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
```

#### html2text {}

```diff
@@ -49,27 +49,28 @@
 them) - [Models](#models) - [Evaluators](#evaluators) 3. [Use-cases](#use-
 cases) - [Evaluating a model](#evaluating-a-model) - [Making a new leaderboard]
 (#making-a-new-leaderboard) - [Making a new evaluator](#making-a-new-evaluator)
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
-set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
-(#citation) 8. [Additional information](#additional-information) - [Data
-Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
-# Quick Start To install the stable release, run ```bash pip install alpaca-
-eval ``` To install the nightly version, run ```bash pip install git+https://
-github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
-export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
-this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` This will print the leaderboard to the console, and save both
-the leaderboard and the annotations to the same directory as the
-`model_outputs` file. Important parameters are the following: -
-**model_outputs** : A path to a json file for the outputs of the model to add
+set](#contributing-an-eval-set) - [Contributing a completion function]
+(#contributing-a-completion-function) 6. [Limitations](#limitations) 7.
+[Citation](#citation) 8. [Additional information](#additional-information) -
+[Data Release](#data-release) - [Differences with AlpacaFarm](#differences-
+with-alpacafarm) - [Related work](#related-work) - [Major updates](#major-
+updates)  # Quick Start To install the stable release, run ```bash pip install
+alpaca-eval ``` To install the nightly version, run ```bash pip install
+git+https://github.com/tatsu-lab/alpaca_eval ``` Then you can use it as
+follows: ```bash export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= #
+Optional; if not set, this will be your default org id. alpaca_eval --
+model_outputs 'example/outputs.json' ``` This will print the leaderboard to the
+console, and save both the leaderboard and the annotations to the same
+directory as the `model_outputs` file. Important parameters are the following:
+- **model_outputs** : A path to a json file for the outputs of the model to add
 to the leaderboard. Each dictionary should contain the keys `instruction` and
 `output`. - **annotators_config**: This is the annotator to use (e.g.,
 `alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
 has the highest agreement rate with our human annotation data. `claude` has a
 decent agreement and is free for academics. `chatgpt_fn` is the worst of the
 three, but is available to everyone, cheap, and has 2x larger context window
 (16K tokens). For a comparison of annotators see [here](#evaluators). -
@@ -644,58 +645,82 @@
 [alpaca_eval.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/
 main/alpaca_eval.json) as a guide (the `dataset` field is not necessary).
 Finally, we ask that you create a minimal leaderboard on this new evaluation
 set. You can do this with the following: ```bash alpaca_eval make_leaderboard \
 --leaderboard_path
 lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
 all_model_outputs alpaca_eval_all_outputs.json \ --reference_outputs  ```
-Please submit a PR with the eval set json and corresponding leaderboard csv.  #
-Limitations The AlpacaEval evaluation pipeline, like other current evaluators
-have important limitations and should therefore not be used as replacement for
-human evaluation in important settings, such as to decide whether a model is
-ready to be deployed. Those can broadly be clustered into 3 categories: 1.
-**Instructions might not be representative of real-usage**: the AlpacaEval set
-contains examples from a variety of datasets ([self-instruct](https://
-github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
-datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
-[vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
-github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
-datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
-representative of real-usage and advanced applications of better models like
-GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
-seem more similar to the open models than what they are. Indeed, those closed
-models seem to be pretrained/finetuned on much more diverse data. See for
-example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
-more complex instructions. Note, however, that in [AlpacaFarm](https://
-arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
-highly correlated (0.97 R2) with win-rates on instructions from user
-interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
-shows larger gap between the open models and OpenAI models than other
-leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
-**Biases of automatic annotators**: the automatic annotators seem to have
-implicit biases. In particular, we found that they tend to prefer longer
-outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
-and 0.62 / 0.58 for `claude`). Although we found that humans have similar
-biases (0.64 / 0.61), we believe that this could be more of a limitation of
-human annotation pipeline we used rather than a true human bias. More
-generally, through qualitative analysis, we found that automatic annotators
-give more importance to the style of the output than its content (e.g.
-factuality). Finally, we found that automatic evaluators tend to prefer outputs
-from models that are similar (likely trained on the same data) as suggested by
-the big difference between ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s
-leaderboard. 3. **Lack of safety evaluation**: importantly, AlpacaEval only
-evaluates the instruction-following capabilities of models rather than the harm
-that they could cause (e.g. toxic behavior or bias). As a result the small gap
-between current ChatGPT and the best open source models **should not** be
-interpreted as if that the latter are ready to be deployed. Beyond those
-limitations about the evaluation pipelines, there are also limitations about
-our validation of the evaluators and our [proposed approach](#analyzing-an-
-eval-set) to selecting evaluation sets.  Limitations about our validation
-pipeline
+Please submit a PR with the eval set json and corresponding leaderboard csv.
+***** Contributing a completion function *****
+Currently, we allow different completion functions, e.g., `openai`,
+`anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to
+contribute a new completion function / API with which to perform inference then
+follow those steps: 1. add a file .py with a function `_completions(prompts :
+Sequence[str], model_name :str, ... )` in the [decoder folder](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This
+function should take as argument the prompts + kwargs and return the
+completions. Please look at other completion functions in the directory for
+templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/
+alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or
+[anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+decoders/anthropic.py). 2. add `_completions` and dependencies in [__init__]
+(https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/
+__init__.py) . Again you can follow the example of
+[huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/
+main/src/alpaca_eval/decoders/__init__.py#L30) 3. update optional dependencies
+in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py) 4.
+add a model you want to evaluate in the [models configs](https://github.com/
+tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) 5. evaluate
+your model using `alpaca_eval evaluate_from_model --model_configs ''` 6.
+(optional) push the results from the previous model on AlpacaEval leaderboard
+following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/
+main#contributing-a-model) Feel free to start a PR early, we'll be able to
+provide some help in the process!  # Limitations The AlpacaEval evaluation
+pipeline, like other current evaluators have important limitations and should
+therefore not be used as replacement for human evaluation in important
+settings, such as to decide whether a model is ready to be deployed. Those can
+broadly be clustered into 3 categories: 1. **Instructions might not be
+representative of real-usage**: the AlpacaEval set contains examples from a
+variety of datasets ([self-instruct](https://github.com/yizhongw/self-
+instruct), [open-assistant](https://huggingface.co/datasets/OpenAssistant/
+oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/
+blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-
+test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/
+Anthropic--hh-rlhf/test)) which might not be representative of real-usage and
+advanced applications of better models like GPT4. This likely makes the best
+closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open
+models than what they are. Indeed, those closed models seem to be pretrained/
+finetuned on much more diverse data. See for example [this blog](https://
+medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-
+harder-tasks-aa0395c31610) for preliminary results on more complex
+instructions. Note, however, that in [AlpacaFarm](https://arxiv.org/abs/
+2305.14387) we showed that win-rates on our evaluation set are highly
+correlated (0.97 R2) with win-rates on instructions from user interactions with
+the Alpaca Demo. Furthermore, the AlpacaEval leaderboard shows larger gap
+between the open models and OpenAI models than other leaderboards ( e.g.
+[lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2. **Biases of automatic
+annotators**: the automatic annotators seem to have implicit biases. In
+particular, we found that they tend to prefer longer outputs and outputs that
+contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4` and 0.62 / 0.58 for
+`claude`). Although we found that humans have similar biases (0.64 / 0.61), we
+believe that this could be more of a limitation of human annotation pipeline we
+used rather than a true human bias. More generally, through qualitative
+analysis, we found that automatic annotators give more importance to the style
+of the output than its content (e.g. factuality). Finally, we found that
+automatic evaluators tend to prefer outputs from models that are similar
+(likely trained on the same data) as suggested by the big difference between
+ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s leaderboard. 3. **Lack of
+safety evaluation**: importantly, AlpacaEval only evaluates the instruction-
+following capabilities of models rather than the harm that they could cause
+(e.g. toxic behavior or bias). As a result the small gap between current
+ChatGPT and the best open source models **should not** be interpreted as if
+that the latter are ready to be deployed. Beyond those limitations about the
+evaluation pipelines, there are also limitations about our validation of the
+evaluators and our [proposed approach](#analyzing-an-eval-set) to selecting
+evaluation sets.  Limitations about our validation pipeline
  First, our validation of evaluators based on human cross-annotations suffers
 from the following limitations: (1) we qualitatively found that our crowd-
 workers tend to also favor style such as length and presence of lists over
 factuality; (2) this does not validate whether win-rates against a reference
 model is a good evaluation strategy in the first place; (3) preferences from 16
 crowd-workers are not representative of preferences of all humans. Second, our
 suggested approach to selecting evaluation sets based on statistical power
```

### Comparing `alpaca_eval-0.2.7/example/outputs.json` & `alpaca_eval-0.2.8/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/setup.py` & `alpaca_eval-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.8/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.8/src/alpaca_eval/annotators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,18 +518,22 @@
         self.batch_size = batch_size
         self.annotation_column = annotation_column
         self.completion_column = "raw_completion" if is_store_raw_completions else None
 
         self.is_add_default_processors = is_add_default_processors
         self.processors = []
         processors_to_kwargs = processors_to_kwargs or {}
-        if batch_size > 1 and self.is_add_default_processors:
+        if (
+            batch_size > 1
+            and self.is_add_default_processors
+            and "PaddingForBatchesProcessor" not in processors_to_kwargs
+        ):
             processors_to_kwargs["PaddingForBatchesProcessor"] = {
                 "batch_size": batch_size,
-                "padding_example": DUMMY_EXAMPLE,
+                "padding_example": utils.DUMMY_EXAMPLE,
             }
         for processor, processor_kwargs in processors_to_kwargs.items():
             processor_kwargs["seed"] = self.seed
             Processor = self._search_processor(processor)
             self.processors += [Processor(**processor_kwargs)]
 
     ### Public methods ###
@@ -577,17 +581,21 @@
     ######################
 
     ### Private methods ###
     def _search_fn_completion_parser(self, name: str) -> Callable:
         """Search for a completion parser by name."""
         return utils.get_module_attribute(completion_parsers, name)
 
-    def _search_processor(self, name: str) -> Type["processors.BaseProcessor"]:
+    def _search_processor(self, name: Union[str, Type["processors.BaseProcessor"]]) -> Type["processors.BaseProcessor"]:
         """Search for a Processor class by name."""
-        return utils.get_module_attribute(processors, name)
+        if isinstance(name, str):
+            return utils.get_module_attribute(processors, name)
+        else:
+            assert issubclass(name, processors.BaseProcessor)
+            return name
 
     def _get_prompt_template(self, prompt_template: utils.AnyPath):
         return utils.read_or_return(self.base_dir / prompt_template)
 
     def _make_prompts(
         self, df_to_annotate: pd.DataFrame, prompt_template: Optional[str] = None
     ) -> tuple[list[str], pd.DataFrame]:
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.8/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.8/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.8/src/alpaca_eval/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,51 +60,51 @@
 
 
 def ALPACAEVAL_REFERENCE_OUTPUTS():
     dataset = datasets.load_dataset(
         "tatsu-lab/alpaca_eval",
         "alpaca_eval",
         cache_dir=DEFAULT_CACHE_DIR,
-        use_auth_token=DATASETS_TOKEN,
+        token=DATASETS_TOKEN,
         download_mode="force_redownload" if DATASETS_FORCE_DOWNLOAD else None,
     )["eval"]
     return dataset
 
 
 def ALPACAFARM_ALL_OUTPUTS():
     return datasets.load_dataset(
         "tatsu-lab/alpaca_eval",
         "alpaca_eval_all_outputs",
         cache_dir=DEFAULT_CACHE_DIR,
-        use_auth_token=DATASETS_TOKEN,
+        token=DATASETS_TOKEN,
         download_mode="force_redownload" if DATASETS_FORCE_DOWNLOAD else None,
     )["eval"]
 
 
 def ALPACAFARM_GOLD_CROSSANNOTATIONS():
     df = datasets.load_dataset(
         "tatsu-lab/alpaca_eval",
         "alpaca_farm_human_crossannotations",
         cache_dir=DEFAULT_CACHE_DIR,
-        use_auth_token=DATASETS_TOKEN,
+        token=DATASETS_TOKEN,
         download_mode="force_redownload" if DATASETS_FORCE_DOWNLOAD else None,
     )["validation"].to_pandas()
 
     # turkers took around 9 min for 15 examples in AlpacaFarm
     df["time_per_example"] = 9.2 * 60 / 15
     df["price_per_example"] = 0.3  # price we paid for each example
     return df
 
 
 def ALPACAFARM_GOLD_ANNOTATIONS():
     df = datasets.load_dataset(
         "tatsu-lab/alpaca_eval",
         "alpaca_farm_human_annotations",
         cache_dir=DEFAULT_CACHE_DIR,
-        use_auth_token=DATASETS_TOKEN,
+        token=DATASETS_TOKEN,
         download_mode="force_redownload" if DATASETS_FORCE_DOWNLOAD else None,
     )["validation"].to_pandas()
 
     # turkers took around 9 min for 15 examples in AlpacaFarm
     df["time_per_example"] = 9.2 * 60 / 15
     df["price_per_example"] = 0.3  # price we paid for each example
     return df
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     model_name : str, optional
         Name of the model to use for decoding.
 
     num_procs : int, optional
         Number of parallel processes to use for decoding.
 
     decoding_kwargs :
-        Additional kwargs to pass to `anthropic.Client.completion`.
+        Additional kwargs to pass to `anthropic.Anthropic.create`.
     """
 
     n_examples = len(prompts)
     if n_examples == 0:
         logging.info("No samples to annotate.")
         return []
     else:
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/decoders/replicate.py` & `alpaca_eval-0.2.8/src/alpaca_eval/decoders/replicate.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 claude-2,91.35572139303484,0.9897323784630048,734,69,1,804,minimal,1069
 openchat-v3.1-13b,89.49004975124379,1.076875474505156,718,83,3,804,community,1484
 chatgpt,89.36567164179104,1.0789487022114888,716,83,5,804,minimal,827
 wizardlm-13b-v1.2,89.1656288916563,1.0904254662753898,714,85,4,803,community,1635
 vicuna-33b-v1.3,88.99253731343283,1.095692216068168,713,86,5,804,verified,1479
 claude,88.38509316770187,1.1144875403283188,707,89,9,805,minimal,1082
 openchat-v2-w-13b,87.1268656716418,1.1769197439396015,699,102,3,804,community,1566
+openbuddy-llama-65b-v8,86.53366583541147,1.2029182403474274,693,107,2,802,community,1162
 wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,692,108,4,804,community,1525
 openchat-v2-13b,84.96894409937889,1.2572979835605944,683,120,2,805,community,1564
 vicuna-13b-v1.3,82.11180124223603,1.348769957803504,660,143,2,805,verified,1132
+openbuddy-llama-30b-v7.1,81.54613466334165,1.370658000946423,654,148,0,802,community,968
 llama-2-13b-chat-hf,81.09452736318407,1.3817573087734825,652,152,0,804,minimal,1513
 openchat-13b,80.8695652173913,1.3843738653129234,650,153,2,805,community,1632
+openbuddy-falcon-40b-v9,80.69738480697384,1.3908517976873223,647,154,2,803,community,1089
 ultralm-13b,80.63511830635119,1.3939556917204066,647,155,1,803,community,1087
 openchat8192-13b,79.53980099502488,1.4222439886269744,639,164,1,804,community,1664
 opencoderplus-15b,78.69565217391305,1.440029529188432,632,170,3,805,community,1628
 vicuna-7b-v1.3,76.8414481897628,1.487520320531845,614,184,3,801,verified,1110
 wizardlm-13b,75.31094527363184,1.5101858292160824,601,194,9,804,minimal,985
 airoboros-65b,73.91304347826086,1.5285333061227804,587,202,16,805,community,1512
 airoboros-33b,73.29192546583852,1.55290318216736,587,212,6,805,community,1514
 guanaco-65b,71.80124223602485,1.586912361158523,578,227,0,805,minimal,1249
 llama-2-7b-chat-hf,71.36645962732919,1.593038654706019,574,230,1,805,minimal,1479
 vicuna-13b,70.43478260869566,1.6069688407799696,566,237,2,805,minimal,1037
+openbuddy-falcon-7b-v6,70.36114570361146,1.612538056786233,565,238,0,803,community,1152
 baize-v2-13b,66.95652173913044,1.6565358231309506,538,265,2,805,community,930
 oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,534,268,3,805,minimal,1079
 minotaur-13b,66.02484472049689,1.6645545328264226,529,271,5,805,community,881
 guanaco-33b,65.96273291925466,1.67108537053247,531,274,0,805,verified,1311
 nous-hermes-13b,65.46583850931677,1.669962276077284,524,275,6,805,verified,844
 vicuna-7b,64.40993788819875,1.6851107260487883,517,285,3,805,verified,1044
 baize-v2-7b,63.85093167701863,1.6945981855442178,514,291,0,805,community,1127
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.8/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/main.py` & `alpaca_eval-0.2.8/src/alpaca_eval/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,19 @@
                 old_output_path=output_path / "reference_outputs.json",
             )
 
         if output_path is not None:
             model_outputs.to_json(output_path / "model_outputs.json", orient="records", indent=2)
             reference_outputs.to_json(output_path / "reference_outputs.json", orient="records", indent=2)
 
+    if reference_model_configs is None:
+        # using a default reference outputs => uses the right leaderboard
+        if evaluation_dataset in [constants.ALPACAEVAL_REFERENCE_OUTPUTS]:
+            reference_outputs = evaluation_dataset
+
     return evaluate(
         model_outputs=model_outputs,
         reference_outputs=reference_outputs,
         annotators_config=annotators_config,
         output_path=output_path,
         max_instances=max_instances,
         **kwargs,
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.8/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt` & `alpaca_eval-0.2.8/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.8/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/processors.py` & `alpaca_eval-0.2.8/src/alpaca_eval/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Optional, Sequence
 
 import numpy as np
 import pandas as pd
 
 from . import utils
 
-DUMMY_EXAMPLE = dict(instruction="1+1=", output_1="2", input="", output_2="3")
 __all__ = ["RandomSwitchTwoColumnsProcessor", "PaddingForBatchesProcessor"]
 
 
 class BaseProcessor(abc.ABC):
     """Base class for a processor."""
 
     def __init__(self, seed: int = 123):
@@ -186,8 +185,8 @@
         padding = pd.DataFrame([self.padding_example] * n_to_pad)
         padding["is_padding"] = True
         df_out = pd.concat([df_to_annotate, padding], axis=0, ignore_index=True)
         df_out["is_padding"] = df_out["is_padding"].fillna(False)
         return df_out
 
     def postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
-        return df_annotated[~df_annotated["is_padding"]].drop(columns=["is_padding"]).copy()
+        return df_annotated[~df_annotated["is_padding"].astype(bool)].drop(columns=["is_padding"]).copy()
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.8/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.8/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.7
+Version: 0.2.8
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -81,14 +81,15 @@
 4. [Analysis](#additional-analysis-and-plots)
     - [Analyzing an evaluator](#analyzing-an-evaluator)
     - [Analyzing an eval set](#analyzing-an-eval-set)
 5. [Contributing](#contributing)
     - [Contributing a model](#contributing-a-model)
     - [Contributing an evaluator](#contributing-an-evaluator)
     - [Contributing an eval set](#contributing-an-eval-set)
+    - [Contributing a completion function](#contributing-a-completion-function)
 6. [Limitations](#limitations)
 7. [Citation](#citation)
 8. [Additional information](#additional-information)
     - [Data Release](#data-release)
     - [Differences with AlpacaFarm](#differences-with-alpacafarm)
     - [Related work](#related-work)
     - [Major updates](#major-updates)
@@ -1049,15 +1050,15 @@
 Then, please follow the steps in [Evaluating a model](#evaluating-a-model) to run inference on the model to produce
 outputs on the eval set and score the model according to one of the evaluators.
 An example command may look like:
 
 ```sh
 alpaca_eval evaluate_from_model \
   --model_configs 'falcon-7b-instruct' \
-  --annotators_config 'alpaca_eval_gpt4' 
+  --annotators_config 'alpaca_eval_gpt4'
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
@@ -1118,14 +1119,31 @@
   --reference_outputs <path_to_json_file>
 ```
 
 Please submit a PR with the eval set json and corresponding leaderboard csv.
 
 </details>
 
+
+
+<details>
+  <summary><h2 tabindex="-1" dir="auto">Contributing a completion function</h2></summary>
+
+Currently, we allow different completion functions, e.g., `openai`, `anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to contribute a new completion function / API with which to perform inference then follow those steps:
+1. add a file <name>.py with a function  `<name>_completions(prompts : Sequence[str], model_name :str, ... )`  in the [decoder folder](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This function should take as argument the prompts + kwargs and return the completions. Please look at other completion functions in the directory for templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or [anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/anthropic.py).
+2. add `<name>_completions` and dependencies in [__init__](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py) . Again you can follow the example of [huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/__init__.py#L30)
+3. update optional dependencies in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py)
+4. add a model you want to evaluate in the [models configs](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs)
+5. evaluate your model using `alpaca_eval evaluate_from_model --model_configs '<model_configs>'`
+6. (optional) push the results from the previous model on AlpacaEval leaderboard following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/main#contributing-a-model)
+
+Feel free to start a PR early, we'll be able to provide some help in the process! 
+
+</details>
+
 # Limitations
 
 The AlpacaEval evaluation pipeline, like other current evaluators have important limitations and should therefore not be
 used as replacement for human evaluation in important settings, such as to decide whether a model is ready to be
 deployed.
 Those can broadly be clustered into 3 categories:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.7 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.8 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -60,27 +60,28 @@
 them) - [Models](#models) - [Evaluators](#evaluators) 3. [Use-cases](#use-
 cases) - [Evaluating a model](#evaluating-a-model) - [Making a new leaderboard]
 (#making-a-new-leaderboard) - [Making a new evaluator](#making-a-new-evaluator)
 4. [Analysis](#additional-analysis-and-plots) - [Analyzing an evaluator]
 (#analyzing-an-evaluator) - [Analyzing an eval set](#analyzing-an-eval-set) 5.
 [Contributing](#contributing) - [Contributing a model](#contributing-a-model) -
 [Contributing an evaluator](#contributing-an-evaluator) - [Contributing an eval
-set](#contributing-an-eval-set) 6. [Limitations](#limitations) 7. [Citation]
-(#citation) 8. [Additional information](#additional-information) - [Data
-Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
-alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
-# Quick Start To install the stable release, run ```bash pip install alpaca-
-eval ``` To install the nightly version, run ```bash pip install git+https://
-github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
-export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
-this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` This will print the leaderboard to the console, and save both
-the leaderboard and the annotations to the same directory as the
-`model_outputs` file. Important parameters are the following: -
-**model_outputs** : A path to a json file for the outputs of the model to add
+set](#contributing-an-eval-set) - [Contributing a completion function]
+(#contributing-a-completion-function) 6. [Limitations](#limitations) 7.
+[Citation](#citation) 8. [Additional information](#additional-information) -
+[Data Release](#data-release) - [Differences with AlpacaFarm](#differences-
+with-alpacafarm) - [Related work](#related-work) - [Major updates](#major-
+updates)  # Quick Start To install the stable release, run ```bash pip install
+alpaca-eval ``` To install the nightly version, run ```bash pip install
+git+https://github.com/tatsu-lab/alpaca_eval ``` Then you can use it as
+follows: ```bash export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= #
+Optional; if not set, this will be your default org id. alpaca_eval --
+model_outputs 'example/outputs.json' ``` This will print the leaderboard to the
+console, and save both the leaderboard and the annotations to the same
+directory as the `model_outputs` file. Important parameters are the following:
+- **model_outputs** : A path to a json file for the outputs of the model to add
 to the leaderboard. Each dictionary should contain the keys `instruction` and
 `output`. - **annotators_config**: This is the annotator to use (e.g.,
 `alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
 has the highest agreement rate with our human annotation data. `claude` has a
 decent agreement and is free for academics. `chatgpt_fn` is the worst of the
 three, but is available to everyone, cheap, and has 2x larger context window
 (16K tokens). For a comparison of annotators see [here](#evaluators). -
@@ -655,58 +656,82 @@
 [alpaca_eval.json](https://huggingface.co/datasets/tatsu-lab/alpaca_eval/blob/
 main/alpaca_eval.json) as a guide (the `dataset` field is not necessary).
 Finally, we ask that you create a minimal leaderboard on this new evaluation
 set. You can do this with the following: ```bash alpaca_eval make_leaderboard \
 --leaderboard_path
 lpaca_eval/leaderboards/data_AlpacaEval/your_leaderboard_name.csv> \ --
 all_model_outputs alpaca_eval_all_outputs.json \ --reference_outputs  ```
-Please submit a PR with the eval set json and corresponding leaderboard csv.  #
-Limitations The AlpacaEval evaluation pipeline, like other current evaluators
-have important limitations and should therefore not be used as replacement for
-human evaluation in important settings, such as to decide whether a model is
-ready to be deployed. Those can broadly be clustered into 3 categories: 1.
-**Instructions might not be representative of real-usage**: the AlpacaEval set
-contains examples from a variety of datasets ([self-instruct](https://
-github.com/yizhongw/self-instruct), [open-assistant](https://huggingface.co/
-datasets/OpenAssistant/oasst1/viewer/OpenAssistant--oasst1/validation),
-[vicuna](https://lmsys.org/blog/2023-03-30-vicuna/), [koala](https://
-github.com/arnav-gudibande/koala-test-set), [hh-rlhf](https://huggingface.co/
-datasets/Anthropic/hh-rlhf/viewer/Anthropic--hh-rlhf/test)) which might not be
-representative of real-usage and advanced applications of better models like
-GPT4. This likely makes the best closed models (GPT4 / Claude / ChatGPT / ...)
-seem more similar to the open models than what they are. Indeed, those closed
-models seem to be pretrained/finetuned on much more diverse data. See for
-example [this blog](https://medium.com/@marcotcr/exploring-chatgpt-vs-open-
-source-models-on-slightly-harder-tasks-aa0395c31610) for preliminary results on
-more complex instructions. Note, however, that in [AlpacaFarm](https://
-arxiv.org/abs/2305.14387) we showed that win-rates on our evaluation set are
-highly correlated (0.97 R2) with win-rates on instructions from user
-interactions with the Alpaca Demo. Furthermore, the AlpacaEval leaderboard
-shows larger gap between the open models and OpenAI models than other
-leaderboards ( e.g. [lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2.
-**Biases of automatic annotators**: the automatic annotators seem to have
-implicit biases. In particular, we found that they tend to prefer longer
-outputs and outputs that contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4`
-and 0.62 / 0.58 for `claude`). Although we found that humans have similar
-biases (0.64 / 0.61), we believe that this could be more of a limitation of
-human annotation pipeline we used rather than a true human bias. More
-generally, through qualitative analysis, we found that automatic annotators
-give more importance to the style of the output than its content (e.g.
-factuality). Finally, we found that automatic evaluators tend to prefer outputs
-from models that are similar (likely trained on the same data) as suggested by
-the big difference between ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s
-leaderboard. 3. **Lack of safety evaluation**: importantly, AlpacaEval only
-evaluates the instruction-following capabilities of models rather than the harm
-that they could cause (e.g. toxic behavior or bias). As a result the small gap
-between current ChatGPT and the best open source models **should not** be
-interpreted as if that the latter are ready to be deployed. Beyond those
-limitations about the evaluation pipelines, there are also limitations about
-our validation of the evaluators and our [proposed approach](#analyzing-an-
-eval-set) to selecting evaluation sets.  Limitations about our validation
-pipeline
+Please submit a PR with the eval set json and corresponding leaderboard csv.
+***** Contributing a completion function *****
+Currently, we allow different completion functions, e.g., `openai`,
+`anthropic`, `huggingface_local`, `huggingface_hub_api` ... If you want to
+contribute a new completion function / API with which to perform inference then
+follow those steps: 1. add a file .py with a function `_completions(prompts :
+Sequence[str], model_name :str, ... )` in the [decoder folder](https://
+github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/decoders). This
+function should take as argument the prompts + kwargs and return the
+completions. Please look at other completion functions in the directory for
+templates. E.g. [huggingface_local_completions](https://github.com/tatsu-lab/
+alpaca_eval/blob/main/src/alpaca_eval/decoders/huggingface_local.py) or
+[anthropic](https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/
+decoders/anthropic.py). 2. add `_completions` and dependencies in [__init__]
+(https://github.com/tatsu-lab/alpaca_eval/blob/main/src/alpaca_eval/decoders/
+__init__.py) . Again you can follow the example of
+[huggingface_local_completions](https://github.com/tatsu-lab/alpaca_eval/blob/
+main/src/alpaca_eval/decoders/__init__.py#L30) 3. update optional dependencies
+in [setup.py](https://github.com/tatsu-lab/alpaca_eval/blob/main/setup.py) 4.
+add a model you want to evaluate in the [models configs](https://github.com/
+tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/models_configs) 5. evaluate
+your model using `alpaca_eval evaluate_from_model --model_configs ''` 6.
+(optional) push the results from the previous model on AlpacaEval leaderboard
+following [those steps](https://github.com/tatsu-lab/alpaca_eval/tree/
+main#contributing-a-model) Feel free to start a PR early, we'll be able to
+provide some help in the process!  # Limitations The AlpacaEval evaluation
+pipeline, like other current evaluators have important limitations and should
+therefore not be used as replacement for human evaluation in important
+settings, such as to decide whether a model is ready to be deployed. Those can
+broadly be clustered into 3 categories: 1. **Instructions might not be
+representative of real-usage**: the AlpacaEval set contains examples from a
+variety of datasets ([self-instruct](https://github.com/yizhongw/self-
+instruct), [open-assistant](https://huggingface.co/datasets/OpenAssistant/
+oasst1/viewer/OpenAssistant--oasst1/validation), [vicuna](https://lmsys.org/
+blog/2023-03-30-vicuna/), [koala](https://github.com/arnav-gudibande/koala-
+test-set), [hh-rlhf](https://huggingface.co/datasets/Anthropic/hh-rlhf/viewer/
+Anthropic--hh-rlhf/test)) which might not be representative of real-usage and
+advanced applications of better models like GPT4. This likely makes the best
+closed models (GPT4 / Claude / ChatGPT / ...) seem more similar to the open
+models than what they are. Indeed, those closed models seem to be pretrained/
+finetuned on much more diverse data. See for example [this blog](https://
+medium.com/@marcotcr/exploring-chatgpt-vs-open-source-models-on-slightly-
+harder-tasks-aa0395c31610) for preliminary results on more complex
+instructions. Note, however, that in [AlpacaFarm](https://arxiv.org/abs/
+2305.14387) we showed that win-rates on our evaluation set are highly
+correlated (0.97 R2) with win-rates on instructions from user interactions with
+the Alpaca Demo. Furthermore, the AlpacaEval leaderboard shows larger gap
+between the open models and OpenAI models than other leaderboards ( e.g.
+[lmsys](https://lmsys.org/blog/2023-03-30-vicuna/)). 2. **Biases of automatic
+annotators**: the automatic annotators seem to have implicit biases. In
+particular, we found that they tend to prefer longer outputs and outputs that
+contain lists (e.g. 0.68 / 0.69 for `alpaca_eval_gpt4` and 0.62 / 0.58 for
+`claude`). Although we found that humans have similar biases (0.64 / 0.61), we
+believe that this could be more of a limitation of human annotation pipeline we
+used rather than a true human bias. More generally, through qualitative
+analysis, we found that automatic annotators give more importance to the style
+of the output than its content (e.g. factuality). Finally, we found that
+automatic evaluators tend to prefer outputs from models that are similar
+(likely trained on the same data) as suggested by the big difference between
+ChatGPT/GPT4 on `claude`'s and `alpaca_eval_gpt4`'s leaderboard. 3. **Lack of
+safety evaluation**: importantly, AlpacaEval only evaluates the instruction-
+following capabilities of models rather than the harm that they could cause
+(e.g. toxic behavior or bias). As a result the small gap between current
+ChatGPT and the best open source models **should not** be interpreted as if
+that the latter are ready to be deployed. Beyond those limitations about the
+evaluation pipelines, there are also limitations about our validation of the
+evaluators and our [proposed approach](#analyzing-an-eval-set) to selecting
+evaluation sets.  Limitations about our validation pipeline
  First, our validation of evaluators based on human cross-annotations suffers
 from the following limitations: (1) we qualitatively found that our crowd-
 workers tend to also favor style such as length and presence of lists over
 factuality; (2) this does not validate whether win-rates against a reference
 model is a good evaluation strategy in the first place; (3) preferences from 16
 crowd-workers are not representative of preferences of all humans. Second, our
 suggested approach to selecting evaluation sets based on statistical power
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.8/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,22 @@
 src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
 src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
 src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/configs.yaml
+src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt
+src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/configs.yaml
+src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt
+src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/configs.yaml
+src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt
+src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/configs.yaml
+src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt
 src/alpaca_eval/models_configs/openchat-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat-13b/prompt.txt
 src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
 src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
 src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
```

### Comparing `alpaca_eval-0.2.7/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.8/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/tests/test_analyze.py` & `alpaca_eval-0.2.8/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/tests/test_decoders_unit.py` & `alpaca_eval-0.2.8/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/tests/test_main.py` & `alpaca_eval-0.2.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.7/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.8/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

