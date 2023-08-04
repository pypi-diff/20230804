# Comparing `tmp/declarai-0.1.1.tar.gz` & `tmp/declarai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declarai-0.1.1.tar", max compression
+gzip compressed data, was "declarai-0.1.2.tar", max compression
```

## Comparing `declarai-0.1.1.tar` & `declarai-0.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1065 2023-08-03 16:51:13.176588 declarai-0.1.1/LICENSE
--rw-r--r--   0        0        0     4169 2023-08-03 16:51:13.176588 declarai-0.1.1/README.md
--rw-r--r--   0        0        0      646 2023-08-03 16:51:13.188588 declarai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/core/__init__.py
--rw-r--r--   0        0        0      279 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/core/core_settings.py
--rw-r--r--   0        0        0     1567 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/declarai.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/__init__.py
--rw-r--r--   0        0        0      983 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/base.py
--rw-r--r--   0        0        0     1496 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/chat_decorator.py
--rw-r--r--   0        0        0      645 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/magic.py
--rw-r--r--   0        0        0      569 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/decorators/task_decorator.py
--rw-r--r--   0        0        0     6647 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/README.md
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/__init__.py
--rw-r--r--   0        0        0     5989 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/evaluator.py
--rw-r--r--   0        0        0      422 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/__init__.py
--rw-r--r--   0        0        0      486 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/multiple_value.py
--rw-r--r--   0        0        0      682 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/multiple_value_multi_types.py
--rw-r--r--   0        0        0      427 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/single_value.py
--rw-r--r--   0        0        0      631 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/extraction/single_value_multi_types.py
--rw-r--r--   0        0        0      484 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/__init__.py
--rw-r--r--   0        0        0      693 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/structured_open_ended.py
--rw-r--r--   0        0        0     1224 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/structured_strict_complex.py
--rw-r--r--   0        0        0      270 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/unstructured_long_form.py
--rw-r--r--   0        0        0      251 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/generation/unstructured_short_form.py
--rw-r--r--   0        0        0       64 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/logical_tasks/__init__.py
--rw-r--r--   0        0        0     2082 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/logical_tasks/sequence.py
--rw-r--r--   0        0        0       86 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/manipulation/__init__.py
--rw-r--r--   0        0        0      586 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/manipulation/data_manipulation_structured.py
--rw-r--r--   0        0        0      393 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/metadata_significance/__init__.py
--rw-r--r--   0        0        0     1550 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/metadata_significance/simple_task_significance.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/providers/__init__.py
--rw-r--r--   0        0        0      549 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/providers/openai.py
--rw-r--r--   0        0        0     3763 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/evals/runner.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/middlewares/__init__.py
--rw-r--r--   0        0        0      610 2023-08-03 16:51:13.188588 declarai-0.1.1/src/declarai/middlewares/base.py
--rw-r--r--   0        0        0       46 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/declarai/__init__.py
--rw-r--r--   0        0        0     1177 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/declarai/log_middleware.py
--rw-r--r--   0        0        0       48 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/third_party/__init__.py
--rw-r--r--   0        0        0     2947 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/middlewares/third_party/wandb_monitor.py
--rw-r--r--   0        0        0     1345 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/__init__.py
--rw-r--r--   0        0        0     1845 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/llm_settings.py
--rw-r--r--   0        0        0       98 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/__init__.py
--rw-r--r--   0        0        0      721 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/llm.py
--rw-r--r--   0        0        0      510 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/message.py
--rw-r--r--   0        0        0      701 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/base/types/operator.py
--rw-r--r--   0        0        0       46 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/__init__.py
--rw-r--r--   0        0        0     2796 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/chat_operator.py
--rw-r--r--   0        0        0       34 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/__init__.py
--rw-r--r--   0        0        0     1840 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/openai_llm.py
--rw-r--r--   0        0        0      298 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/settings.py
--rw-r--r--   0        0        0     3916 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/openai_operators/task_operator.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/__init__.py
--rw-r--r--   0        0        0     1709 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/output_prompt.py
--rw-r--r--   0        0        0      215 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/__init__.py
--rw-r--r--   0        0        0      189 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/chain_of_thought.py
--rw-r--r--   0        0        0       75 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/instruct_function.py
--rw-r--r--   0        0        0      371 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/operators/shared/templates/output_structure.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/__init__.py
--rw-r--r--   0        0        0     2559 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/chat_orchestrator.py
--rw-r--r--   0        0        0      745 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/future_llm_task.py
--rw-r--r--   0        0        0     2822 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/sequence.py
--rw-r--r--   0        0        0     2821 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/task_orchestrator.py
--rw-r--r--   0        0        0      124 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/orchestrator/types.py
--rw-r--r--   0        0        0       38 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/annotations/__init__.py
--rw-r--r--   0        0        0     2433 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/annotations/type_annotation_to_schema.py
--rw-r--r--   0        0        0        0 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/__init__.py
--rw-r--r--   0        0        0       40 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/reST/__init__.py
--rw-r--r--   0        0        0     1922 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/reST/parser.py
--rw-r--r--   0        0        0      445 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/docstring_parsers/types.py
--rw-r--r--   0        0        0     1909 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/magic_parser.py
--rw-r--r--   0        0        0     4925 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/parser.py
--rw-r--r--   0        0        0      767 2023-08-03 16:51:13.192588 declarai-0.1.1/src/declarai/python_parser/types.py
--rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 declarai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-04 20:32:27.106865 declarai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4205 2023-08-04 20:32:27.106865 declarai-0.1.2/README.md
+-rw-r--r--   0        0        0      645 2023-08-04 20:32:27.114865 declarai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/core/__init__.py
+-rw-r--r--   0        0        0      279 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/core/core_settings.py
+-rw-r--r--   0        0        0     1587 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/declarai.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/decorators/__init__.py
+-rw-r--r--   0        0        0      613 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/decorators/base.py
+-rw-r--r--   0        0        0     2316 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/decorators/chat_decorator.py
+-rw-r--r--   0        0        0      645 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/decorators/magic.py
+-rw-r--r--   0        0        0     1313 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/decorators/task_decorator.py
+-rw-r--r--   0        0        0     6647 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/__init__.py
+-rw-r--r--   0        0        0     5989 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/evaluator.py
+-rw-r--r--   0        0        0      422 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/extraction/__init__.py
+-rw-r--r--   0        0        0      486 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/extraction/multiple_value.py
+-rw-r--r--   0        0        0      682 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/extraction/multiple_value_multi_types.py
+-rw-r--r--   0        0        0      427 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/extraction/single_value.py
+-rw-r--r--   0        0        0      631 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/extraction/single_value_multi_types.py
+-rw-r--r--   0        0        0      484 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/generation/__init__.py
+-rw-r--r--   0        0        0      693 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/generation/structured_open_ended.py
+-rw-r--r--   0        0        0     1224 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/generation/structured_strict_complex.py
+-rw-r--r--   0        0        0      270 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/generation/unstructured_long_form.py
+-rw-r--r--   0        0        0      251 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/generation/unstructured_short_form.py
+-rw-r--r--   0        0        0       64 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/logical_tasks/__init__.py
+-rw-r--r--   0        0        0     2082 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/logical_tasks/sequence.py
+-rw-r--r--   0        0        0       86 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/manipulation/__init__.py
+-rw-r--r--   0        0        0      586 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/manipulation/data_manipulation_structured.py
+-rw-r--r--   0        0        0      393 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/metadata_significance/__init__.py
+-rw-r--r--   0        0        0     1550 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/metadata_significance/simple_task_significance.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/providers/__init__.py
+-rw-r--r--   0        0        0      549 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/providers/openai.py
+-rw-r--r--   0        0        0     3763 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/evals/runner.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/__init__.py
+-rw-r--r--   0        0        0      610 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/base.py
+-rw-r--r--   0        0        0       46 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/declarai/__init__.py
+-rw-r--r--   0        0        0     1177 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/declarai/log_middleware.py
+-rw-r--r--   0        0        0       48 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/third_party/__init__.py
+-rw-r--r--   0        0        0     2947 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/middlewares/third_party/wandb_monitor.py
+-rw-r--r--   0        0        0     1345 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/__init__.py
+-rw-r--r--   0        0        0     1858 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/llm_settings.py
+-rw-r--r--   0        0        0       98 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/types/__init__.py
+-rw-r--r--   0        0        0      721 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/types/llm.py
+-rw-r--r--   0        0        0      510 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/types/message.py
+-rw-r--r--   0        0        0      701 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/base/types/operator.py
+-rw-r--r--   0        0        0       46 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/__init__.py
+-rw-r--r--   0        0        0     2796 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/chat_operator.py
+-rw-r--r--   0        0        0       34 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/openai_llm/__init__.py
+-rw-r--r--   0        0        0     1840 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/openai_llm/openai_llm.py
+-rw-r--r--   0        0        0      298 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/openai_llm/settings.py
+-rw-r--r--   0        0        0     3916 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/openai_operators/task_operator.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/__init__.py
+-rw-r--r--   0        0        0     1709 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/output_prompt.py
+-rw-r--r--   0        0        0      215 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/templates/__init__.py
+-rw-r--r--   0        0        0      189 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/templates/chain_of_thought.py
+-rw-r--r--   0        0        0       75 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/templates/instruct_function.py
+-rw-r--r--   0        0        0      371 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/operators/shared/templates/output_structure.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/__init__.py
+-rw-r--r--   0        0        0     2559 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/chat_orchestrator.py
+-rw-r--r--   0        0        0      745 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/future_llm_task.py
+-rw-r--r--   0        0        0     2822 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/sequence.py
+-rw-r--r--   0        0        0     2821 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/task_orchestrator.py
+-rw-r--r--   0        0        0      124 2023-08-04 20:32:27.114865 declarai-0.1.2/src/declarai/orchestrator/types.py
+-rw-r--r--   0        0        0       38 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/annotations/__init__.py
+-rw-r--r--   0        0        0     2433 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/annotations/type_annotation_to_schema.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/docstring_parsers/__init__.py
+-rw-r--r--   0        0        0       40 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/docstring_parsers/reST/__init__.py
+-rw-r--r--   0        0        0     1922 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/docstring_parsers/reST/parser.py
+-rw-r--r--   0        0        0      445 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/docstring_parsers/types.py
+-rw-r--r--   0        0        0     1909 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/magic_parser.py
+-rw-r--r--   0        0        0     4925 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/parser.py
+-rw-r--r--   0        0        0      767 2023-08-04 20:32:27.118865 declarai-0.1.2/src/declarai/python_parser/types.py
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 declarai-0.1.2/PKG-INFO
```

### Comparing `declarai-0.1.1/LICENSE` & `declarai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/README.md` & `declarai-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,8 +142,8 @@
 #> 2
 ```
 
 To read more about what you can do with Declarai, 
 please visit our documentation site: [docs](https://vendi-ai.github.io/declarai/)
 
 ## Contributing
-We welcome contributions to Declarai! Please read our [contributing guide](CONTRIBUTING.md) to get started.
+We welcome contributions to Declarai! Please read our [contributing guide](https://vendi-ai.github.io/declarai/src/contribute/) to get started.
```

### Comparing `declarai-0.1.1/pyproject.toml` & `declarai-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "declarai"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Aviv Almashanu <avivex1000@gmail.com>"]
 readme = "README.md"
 packages = [{include = "declarai", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 openai = "^0.27.8"
 pydantic = "^1.8.2"
 jsonref = "^1.1.0"
-wandb = {version = "^0.10.32", optional = true}
+wandb = {version = "^0.15.8", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.13.9"
 black = "^23.3.0"
 isort = "^5.11.5"
 pytest = "^7.4.0"
```

### Comparing `declarai-0.1.1/src/declarai/declarai.py` & `declarai-0.1.2/src/declarai/declarai.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 
     # *-------------------------------------------------------------------------- *
     # * Actual implementation of Declarai                                         *
     # *-------------------------------------------------------------------------- *
     def __init__(self, **kwargs):
         self.llm_config = LLMSettings(**kwargs)
 
-        self.task = LLMTaskDecorator(self)
+        self.task = LLMTaskDecorator(self, **kwargs)
 
         class Experimental:
-            chat = LLMChatDecorator(self)
+            chat = LLMChatDecorator(self, **kwargs)
 
         self.experimental = Experimental
```

### Comparing `declarai-0.1.1/src/declarai/decorators/base.py` & `declarai-0.1.2/src/declarai/decorators/task_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from abc import abstractmethod
-from typing import Any, List, Optional
-
+from typing import overload, Callable, Any, List, Type
+from typing_extensions import Self
+from declarai.decorators.base import LLMOrchestratorDecorator
 from declarai.middlewares.base import TaskMiddleware
+from declarai.operators import resolve_operator
+from declarai.orchestrator.task_orchestrator import LLMTaskOrchestrator
 
 
-class LLMOrchestratorDecorator:
-    def __init__(
-        self,
-        declarai_instance,
-        middlewares: Optional[List[TaskMiddleware]] = None,
-        **kwargs,
-    ):
-        self.declarai_instance = declarai_instance
-
-        self.operator = self.get_operator(**kwargs)
-        self.middlewares = middlewares or []
+class LLMTaskDecorator(LLMOrchestratorDecorator):
+    @overload
+    def __call__(self, decorated: None = None, *, middlewares: List[Type[TaskMiddleware]]) -> Self:
+        ...
 
-    @abstractmethod
-    def get_operator(self, **kwargs):
+    @overload
+    def __call__(self, decorated: Callable[..., Any]) -> LLMTaskOrchestrator:
         ...
 
     def __call__(
         self,
         decorated=None,
         *,
-        middlewares: List[TaskMiddleware] = None,
+        middlewares: List[TaskMiddleware] = None
     ):
         # When arguments are passed
         if decorated is None:
             self.middlewares = middlewares
             return self
         else:
             # When no arguments are passed
             return self.return_orchestrator(decorated)
 
-    @abstractmethod
-    def return_orchestrator(self, decorated: Any) -> Any:
-        ...
+    def get_operator(self, **kwargs):
+        return resolve_operator(self.declarai_instance.llm_config, **kwargs)
+
+    def return_orchestrator(self, func):
+        llm_task = LLMTaskOrchestrator(
+            func, self.operator, middlewares=self.middlewares
+        )
+        llm_task.__name__ = func.__name__
+        return llm_task
```

### Comparing `declarai-0.1.1/src/declarai/decorators/magic.py` & `declarai-0.1.2/src/declarai/decorators/magic.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/README.md` & `declarai-0.1.2/src/declarai/evals/README.md`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/evaluator.py` & `declarai-0.1.2/src/declarai/evals/evaluator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/extraction/multiple_value_multi_types.py` & `declarai-0.1.2/src/declarai/evals/extraction/multiple_value_multi_types.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/extraction/single_value_multi_types.py` & `declarai-0.1.2/src/declarai/evals/extraction/single_value_multi_types.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/generation/structured_open_ended.py` & `declarai-0.1.2/src/declarai/evals/generation/structured_open_ended.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/generation/structured_strict_complex.py` & `declarai-0.1.2/src/declarai/evals/generation/structured_strict_complex.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/logical_tasks/sequence.py` & `declarai-0.1.2/src/declarai/evals/logical_tasks/sequence.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/manipulation/data_manipulation_structured.py` & `declarai-0.1.2/src/declarai/evals/manipulation/data_manipulation_structured.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/metadata_significance/simple_task_significance.py` & `declarai-0.1.2/src/declarai/evals/metadata_significance/simple_task_significance.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/providers/openai.py` & `declarai-0.1.2/src/declarai/evals/providers/openai.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/evals/runner.py` & `declarai-0.1.2/src/declarai/evals/runner.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/middlewares/base.py` & `declarai-0.1.2/src/declarai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/middlewares/declarai/log_middleware.py` & `declarai-0.1.2/src/declarai/middlewares/declarai/log_middleware.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/middlewares/third_party/wandb_monitor.py` & `declarai-0.1.2/src/declarai/middlewares/third_party/wandb_monitor.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/__init__.py` & `declarai-0.1.2/src/declarai/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/base/llm_settings.py` & `declarai-0.1.2/src/declarai/operators/base/llm_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 class LLMSettings:
     def __init__(
         self,
         provider: str,
         model: str,
         version: Optional[str] = None,
+        **_,
     ):
         self.provider = provider
         self._model = model
         self.version = version
 
     @property
     def model(self, delimiter: Optional[str] = "-") -> str:
```

### Comparing `declarai-0.1.1/src/declarai/operators/base/types/llm.py` & `declarai-0.1.2/src/declarai/operators/base/types/llm.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/base/types/operator.py` & `declarai-0.1.2/src/declarai/operators/base/types/operator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/openai_operators/chat_operator.py` & `declarai-0.1.2/src/declarai/operators/openai_operators/chat_operator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/openai_operators/openai_llm/openai_llm.py` & `declarai-0.1.2/src/declarai/operators/openai_operators/openai_llm/openai_llm.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/openai_operators/task_operator.py` & `declarai-0.1.2/src/declarai/operators/openai_operators/task_operator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/operators/shared/output_prompt.py` & `declarai-0.1.2/src/declarai/operators/shared/output_prompt.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/orchestrator/chat_orchestrator.py` & `declarai-0.1.2/src/declarai/orchestrator/chat_orchestrator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/orchestrator/future_llm_task.py` & `declarai-0.1.2/src/declarai/orchestrator/future_llm_task.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/orchestrator/sequence.py` & `declarai-0.1.2/src/declarai/orchestrator/sequence.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/orchestrator/task_orchestrator.py` & `declarai-0.1.2/src/declarai/orchestrator/task_orchestrator.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/python_parser/annotations/type_annotation_to_schema.py` & `declarai-0.1.2/src/declarai/python_parser/annotations/type_annotation_to_schema.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/python_parser/docstring_parsers/reST/parser.py` & `declarai-0.1.2/src/declarai/python_parser/docstring_parsers/reST/parser.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/python_parser/magic_parser.py` & `declarai-0.1.2/src/declarai/python_parser/magic_parser.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/python_parser/parser.py` & `declarai-0.1.2/src/declarai/python_parser/parser.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/src/declarai/python_parser/types.py` & `declarai-0.1.2/src/declarai/python_parser/types.py`

 * *Files identical despite different names*

### Comparing `declarai-0.1.1/PKG-INFO` & `declarai-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: declarai
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Aviv Almashanu
 Author-email: avivex1000@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: wandb
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
-Requires-Dist: wandb (>=0.10.32,<0.11.0) ; extra == "wandb"
+Requires-Dist: wandb (>=0.15.8,<0.16.0) ; extra == "wandb"
 Description-Content-Type: text/markdown
 
 # Introducing declareai
 [![versions](https://img.shields.io/pypi/pyversions/declarai.svg)](https://github.com/vendi-ai/declarai)
 [![license](https://img.shields.io/github/license/vendi-ai/declarai.svg)](https://github.com/vendi-ai/declarai/blob/main/LICENSE)
 
 ![Logo - declarai.png](assets/Logo-declarai.png)
@@ -161,9 +161,9 @@
 #> 2
 ```
 
 To read more about what you can do with Declarai, 
 please visit our documentation site: [docs](https://vendi-ai.github.io/declarai/)
 
 ## Contributing
-We welcome contributions to Declarai! Please read our [contributing guide](CONTRIBUTING.md) to get started.
+We welcome contributions to Declarai! Please read our [contributing guide](https://vendi-ai.github.io/declarai/src/contribute/) to get started.
```

