# Comparing `tmp/eyeball_pp-0.0.6.tar.gz` & `tmp/eyeball_pp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.6.tar", last modified: Tue Aug  1 20:05:20 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.7.tar", last modified: Fri Aug  4 00:07:51 2023, max compression
```

## Comparing `eyeball_pp-0.0.6.tar` & `eyeball_pp-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.752260 eyeball_pp-0.0.6/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.6/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     8982 2023-08-01 20:05:20.752408 eyeball_pp-0.0.6/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8599 2023-07-31 17:27:10.000000 eyeball_pp-0.0.6/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.742570 eyeball_pp-0.0.6/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.6/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.6/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.6/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.6/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    40161 2023-08-01 20:04:24.000000 eyeball_pp-0.0.6/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    36960 2023-07-28 05:50:48.000000 eyeball_pp-0.0.6/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.6/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-01 20:05:20.751952 eyeball_pp-0.0.6/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     8982 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-01 20:05:20.000000 eyeball_pp-0.0.6/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-01 20:05:20.753051 eyeball_pp-0.0.6/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.6/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.601343 eyeball_pp-0.0.7/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.7/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 00:07:51.601463 eyeball_pp-0.0.7/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8639 2023-08-03 04:44:59.000000 eyeball_pp-0.0.7/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.599155 eyeball_pp-0.0.7/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      881 2023-08-02 22:46:42.000000 eyeball_pp-0.0.7/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     3661 2023-08-03 23:07:44.000000 eyeball_pp-0.0.7/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     5419 2023-08-03 23:07:38.000000 eyeball_pp-0.0.7/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.7/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    46600 2023-08-04 00:07:30.000000 eyeball_pp-0.0.7/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    40035 2023-08-04 00:07:30.000000 eyeball_pp-0.0.7/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)     3879 2023-08-03 20:00:41.000000 eyeball_pp-0.0.7/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.601139 eyeball_pp-0.0.7/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-04 00:07:51.602076 eyeball_pp-0.0.7/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.7/setup.py
```

### Comparing `eyeball_pp-0.0.6/LICENSE` & `eyeball_pp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.6/PKG-INFO` & `eyeball_pp-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 eyeball_pp is a framework to evaluate and benchmark tasks which use llms.
 
 This framework helps you answer questions like: "Which llm is the best for my specific task?" or "This prompt change looks good on the example I just tested, does it work with all the other things I've tested?"
 
 Your task can be arbitrary, the framework only cares about initial inputs and final outputs.
 
-If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
+If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner WITHOUT you having to become methodical.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Example
```

### Comparing `eyeball_pp-0.0.6/README.md` & `eyeball_pp-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 eyeball_pp is a framework to evaluate and benchmark tasks which use llms.
 
 This framework helps you answer questions like: "Which llm is the best for my specific task?" or "This prompt change looks good on the example I just tested, does it work with all the other things I've tested?"
 
 Your task can be arbitrary, the framework only cares about initial inputs and final outputs.
 
-If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
+If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner WITHOUT you having to become methodical.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Example
```

### Comparing `eyeball_pp-0.0.6/eyeball_pp/__init__.py` & `eyeball_pp-0.0.7/eyeball_pp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .eval import (
     rerun_recorded_examples,
     set_config,
     record_task,
     record_output,
     record_input,
+    record_intermediary_state,
     get_eval_param,
     rate_recorded_examples,
     compare_recorded_checkpoints,
     delete_checkpoints_for_input_vars,
+    calculate_system_health,
     Evaluator,
 )
 
 from .classes import (
     FeedbackResult,
     OutputFeedback,
     OutputComparator,
@@ -31,8 +33,10 @@
     "delete_checkpoints_for_input_vars",
     "Evaluator",
     "FeedbackResult",
     "OutputFeedback",
     "OutputComparator",
     "OutputScorer",
     "OutputScore",
+    "calculate_system_health",
+    "record_intermediary_state",
 ]
```

### Comparing `eyeball_pp-0.0.6/eyeball_pp/eval.py` & `eyeball_pp-0.0.7/eyeball_pp/eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import json
 import os
 import types
 from .recorders import (
     ApiClientRecorder,
     Checkpoint,
     ComparisonResult,
-    DiskRecorder,
     FileRecorder,
     MemoryRecorder,
     EvalRecorder,
     get_input_hash,
 )
 from .comparators import model_graded_comparator, output_feedback_from_scores
 from .classes import (
     FeedbackResult,
+    MultiOutputFeedback,
     OutputComparator,
     OutputScore,
     OutputScorer,
     OutputFeedback,
+    TASK_OUTPUT_KEY,
 )
 
 import random
 import threading
 from typing import (
     Callable,
     Iterable,
@@ -36,18 +37,15 @@
     Any,
     runtime_checkable,
 )
 from functools import wraps
 from dataclasses import dataclass
 import dataclasses
 import datetime
-from .utils import get_user_input
-from .classes import FeedbackResult
-from rich.console import Console
-from rich.table import Table
+from .utils import get_score_map, get_user_input, output_table
 
 GREEN = "\x1b[32m"
 ORANGE = "\x1b[33m"
 RED = "\x1b[31m"
 BOLD = "\x1b[1m"
 UNDERLINE = "\x1b[4m"
 ITALIC = "\x1b[3m"
@@ -71,14 +69,15 @@
 
 @dataclass
 class EvaluatorConfig:
     sample_rate: float = 1.0
     dir_path: str = "."
     api_key: Optional[str] = None
     api_url: Optional[str] = None
+    record_in_memory: bool = False
 
     @staticmethod
     def _merge(original_config: "EvaluatorConfig", **kwargs) -> "EvaluatorConfig":
         """Kwargs should be a subset of the fields of the original config."""
         if len(kwargs) == 0:
             return original_config
 
@@ -115,19 +114,22 @@
 
     def _get_config(self, **override_config_kwargs) -> EvaluatorConfig:
         return EvaluatorConfig._merge(self.config, **override_config_kwargs)
 
     def set_config(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig._merge(self.config, **config_kwargs)
         self.data_dir = os.path.join(self.config.dir_path, "eyeball_data")
-        if self.config.api_key is not None:
-            self.recorder: EvalRecorder = ApiClientRecorder(
+
+        if self.config.record_in_memory:
+            self.recorder: EvalRecorder = MemoryRecorder()
+        elif self.config.api_key is not None:
+            self.recorder = ApiClientRecorder(
                 api_key=self.config.api_key, api_url=self.config.api_url
             )
-        elif self.running_in_notebook or not self.config.sample_rate:
+        elif self.running_in_notebook or self.config.sample_rate == 0:
             self.recorder = MemoryRecorder()
         else:
             self.recorder = FileRecorder(self.data_dir)
 
     @contextmanager
     def start_recording_session(
         self,
@@ -189,14 +191,34 @@
             self.recorder.record_input_variable(
                 task_name=task_name,
                 checkpoint_id=checkpoint_id,
                 variable_name=variable_name,
                 value=serialized_value,
             )
 
+    def record_intermediary_state(
+        self,
+        state_name: str,
+        state_value: str,
+        task_name: Optional[str] = None,
+        checkpoint_id: Optional[str] = None,
+        **config_kwargs,
+    ) -> None:
+        if self._should_record(**config_kwargs):
+            task_name, checkpoint_id = self._get_recorder_state(
+                task_name, checkpoint_id
+            )
+
+            self.recorder.record_intermediary_state(
+                task_name=task_name,
+                checkpoint_id=checkpoint_id,
+                state_name=state_name,
+                state_value=state_value,
+            )
+
     def record_output(
         self,
         value: Any,
         task_name: Optional[str] = None,
         checkpoint_id: Optional[str] = None,
         **config_kwargs,
     ) -> None:
@@ -249,14 +271,30 @@
         if recorder_checkpoint_id is None:
             raise ValueError(
                 "Must provide a checkpoint id or start a recording session to record a variable"
             )
 
         return task_name, recorder_checkpoint_id
 
+    def _get_recorded_task_name(self, task_name: Optional[str]) -> str:
+        if task_name is not None:
+            return task_name
+        if hasattr(self.current_recorder_state, "task_name"):
+            return self.current_recorder_state.task_name
+
+        task_names = self.recorder.get_task_names()
+        if len(task_names) == 0:
+            raise ValueError("No task names found")
+        elif len(task_names) == 1:
+            return task_names[0]
+        else:
+            raise ValueError(
+                f"Must provide a task_name as you have multiple tasks recorded -- Found: {task_names}"
+            )
+
     def get_eval_params(
         self,
         task_name: Optional[str] = None,
         checkpoint_id: Optional[str] = None,
     ) -> Optional[dict[str, Any]]:
         task_name, checkpoint_id = self._get_recorder_state(task_name, checkpoint_id)
 
@@ -428,37 +466,48 @@
         details = get_user_input(
             "Any details about your feedback (optional)\n", choices=None
         )
 
         output_feedback = OutputFeedback(result=feedback_result, message=details)
 
         self.recorder.record_output_feedback(
-            task_name=task_name, checkpoint_id=checkpoint_id, feedback=output_feedback
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            feedback=MultiOutputFeedback({TASK_OUTPUT_KEY: output_feedback}),
         )
         return output_feedback
 
     def rerun_recorded_examples(
         self,
         *eval_params_list: dict[str, Any],
         task_name: Optional[str] = None,
         input_hashes: Optional[list[str]] = None,
+        limit: Optional[int] = None,
+        randomize: Optional[bool] = False,
     ) -> Iterable[dict[str, Any]]:
         if task_name is None:
             task_names = self.recorder.get_task_names()
             if len(task_names) == 0:
                 raise ValueError("No task names found")
             elif len(task_names) == 1:
                 task_name = task_names[0]
             else:
                 raise ValueError(
                     f"Must provide a task_name as you have multiple tasks recorded -- Found: {task_names}"
                 )
 
         if input_hashes is None or len(input_hashes) == 0:
             input_hashes = self.recorder.get_input_hashes(task_name=task_name)
+            print(f"Input hashes {input_hashes}")
+
+        if randomize and input_hashes:
+            random.shuffle(input_hashes)
+
+        if limit is not None:
+            input_hashes = input_hashes[:limit]
 
         try:
             self.mode = EvaluatorMode.RERUN_EXAMPLES
             rerun_metadata = {
                 "id": datetime.datetime.utcnow().isoformat(),
             }
 
@@ -537,58 +586,68 @@
 
         if len(input_hashes_lst) == 0:
             input_hashes_lst = self.recorder.get_input_hashes(task_name=task_name)
 
         try:
             self.mode = EvaluatorMode.RATE_EXAMPLES
             for input_hash in input_hashes_lst:
-                already_seen_outputs_to_feedback: dict[str:OutputFeedback] = {}
+                already_seen_outputs_to_feedback: dict[str, MultiOutputFeedback] = {}
                 checkpoints = self.recorder.get_latest_checkpoints(
                     task_name, input_hash, num_checkpoints=4
                 )
 
                 if len(checkpoints) == 0:
                     continue
 
-                print(f"For the inputs:\n{checkpoints[0].get_input_var_str()}")
+                print(f"\nFor inputs:\n{checkpoints[0].get_input_var_str()}")
                 for checkpoint in checkpoints:
-                    if checkpoint.output_feedback is None:
+                    if checkpoint.output is None:
+                        continue
+
+                    if not checkpoint.feedback:
                         if feedback := already_seen_outputs_to_feedback.get(
                             checkpoint.output
                         ):
                             self.recorder.record_output_feedback(
                                 task_name=task_name,
                                 checkpoint_id=checkpoint.checkpoint_id,
                                 feedback=feedback,
                             )
                         else:
-                            feedback = self.request_user_feedback(
+                            output_feedback = self.request_user_feedback(
                                 checkpoint.output or "",
                                 task_name=task_name,
                                 checkpoint_id=checkpoint.checkpoint_id,
                             )
-                            if feedback is not None:
+                            if output_feedback is not None:
                                 already_seen_outputs_to_feedback[
                                     checkpoint.output
-                                ] = feedback
+                                ] = MultiOutputFeedback(
+                                    {TASK_OUTPUT_KEY: output_feedback}
+                                )
                     elif new_feedback := already_seen_outputs_to_feedback.get(
                         checkpoint.output
                     ):
-                        if new_feedback.result != checkpoint.output_feedback.result:
+                        if (
+                            new_feedback[TASK_OUTPUT_KEY].result
+                            != checkpoint.feedback[TASK_OUTPUT_KEY].result
+                        ):
                             print(
-                                f"For output: {checkpoint.output}\nOld feedback {checkpoint.output_feedback} is different from new feedback {new_feedback}"
+                                f"For output: {checkpoint.output}\nOld feedback {checkpoint.feedback[TASK_OUTPUT_KEY]} is different from new feedback {new_feedback[TASK_OUTPUT_KEY]}"
                             )
                             print(f"Updating feedback to {new_feedback}")
                             self.recorder.record_output_feedback(
                                 task_name=task_name,
                                 checkpoint_id=checkpoint.checkpoint_id,
                                 feedback=new_feedback,
                             )
                     else:
-                        print(f"Already has feedback: {checkpoint.output_feedback}")
+                        print(
+                            f"Output: {checkpoint.output[:140]} already has feedback: {checkpoint.feedback.get(TASK_OUTPUT_KEY)}"
+                        )
         finally:
             self.mode = EvaluatorMode.RECORD
 
     def record_human_feedback(
         self,
         feedback: OutputFeedback,
         details: Optional[str] = None,
@@ -614,135 +673,27 @@
                     f"Must provide a task_name as you have multiple tasks recorded -- Found: {task_names}"
                 )
         input_hash = get_input_hash(
             {k: self._serialize(v) for k, v in input_vars.items()}
         )
         self.recorder.delete_checkpoints_for_input_hash(task_name, input_hash)
 
-    def compute_latest_comparison_results(self, task_name: str) -> None:
-        input_names: set[str] = set()
-        rows: list[dict[str, str]] = []
-        comparison_column_names = [
-            "latest_checkpoint",
-            "previous_checkpoint",
-            "the_checkpoint_before",
-        ]
-
-        for input_hash in self.recorder.get_input_hashes(task_name):
-            # TODO: this is a slow operation
-            checkpoints = self.recorder.get_latest_checkpoints(
-                task_name, input_hash, num_checkpoints=len(comparison_column_names)
-            )
-            if len(checkpoints) == 0:
-                continue
-
-            checkpoint = checkpoints[0]
-            if checkpoint is None:
-                continue
-
-            row_data = {}
-            input_names.update(checkpoint.input_variables.keys())
-            for input_name, input_value in checkpoint.input_variables.items():
-                row_data[input_name] = input_value
-
-            # TODO: this is a slow operation, we should probably load all checkpoints and comparison results for an input hash in one iteration
-            comparison_results = self.recorder.get_comparison_results_for_input_hash(
-                task_name=task_name,
-                input_hash=input_hash,
-                num_results=len(comparison_column_names),
-            )
-            sorted_comparison_results = sorted(
-                comparison_results,
-                key=lambda x: x.newer_checkpoint_id,
-                reverse=True,
-            )
-            for idx, comparison_result in enumerate(sorted_comparison_results):
-                msg = str(comparison_result.output_feedback.result)
-                new_checkpoint = self.recorder.get_checkpoint(
-                    task_name=task_name,
-                    checkpoint_id=comparison_result.newer_checkpoint_id,
-                )
-                if new_checkpoint is not None:
-                    if new_checkpoint.output_score is not None:
-                        msg += f" (score: {new_checkpoint.output_score})"
-                    eval_params_str = ", ".join(
-                        f"{k}={v}" for k, v in new_checkpoint.eval_params.items()
-                    )
-                    if eval_params_str:
-                        msg += f" ({eval_params_str})"
-                row_data[comparison_column_names[idx]] = msg
-
-            for idx in range(len(comparison_column_names)):
-                if (
-                    comparison_column_names[idx] not in row_data
-                    and idx < len(checkpoints)
-                    and (checkpoint := checkpoints[idx]).output_score is not None
-                ):
-                    msg = f"score: **{checkpoint.output_score.score: .2f}**, {checkpoint.output_score.message}"
-                    eval_params_str = ", ".join(
-                        f"{k}={v}" for k, v in checkpoint.eval_params.items()
-                    )
-                    if eval_params_str:
-                        msg += f" ({eval_params_str})"
-                    row_data[comparison_column_names[idx]] = msg
-
-            rows.append(row_data)
-
-        md_data = []
-        table = Table(title="Comparison Results")
-
-        if len(rows) > 0:
-            column_names = sorted(list(input_names)) + comparison_column_names
-            for column_name in column_names:
-                table.add_column(column_name, justify="left")
-
-            md_data.append("| " + " | ".join(column_names) + " |")
-            md_data.append("| " + " | ".join(["---"] * len(column_names)) + " |")
-
-            for row in rows:
-                row_tuple = tuple(
-                    row.get(column_name, "") for column_name in column_names
-                )
-                table.add_row(*row_tuple)
-                md_data.append("| " + " | ".join(row_tuple) + " |")
-
-            task_data_dir = os.path.join(self.data_dir, task_name)
-            if not os.path.exists(task_data_dir):
-                os.makedirs(task_data_dir)
-
-            with open(
-                os.path.join(task_data_dir, "benchmark.md"),
-                "w+",
-            ) as f:
-                f.write("\n".join(md_data))
-
-            console = Console()
-            console.print(table)
-
     def compare_recorded_checkpoints(
         self,
         task_name: Optional[str] = None,
         num_input_hashes: int = 5,
         num_checkpoints_per_input_hash: int = 3,
         task_objective: Optional[str] = None,
         output_comparator: Optional[OutputComparator] = None,
         output_scorer: Optional[OutputScorer] = None,
+        intermediate_objectives: Optional[dict[str, str]] = None,
         use_cached_scores: bool = True,
         use_cached_comparisons: bool = True,
     ) -> None:
-        if task_name is None:
-            task_names = self.recorder.get_task_names()
-            if len(task_names) == 0:
-                raise ValueError("No task names found")
-            elif len(task_names) == 1:
-                task_name = task_names[0]
-            else:
-                raise ValueError(
-                    f"Must provide a task_name as you have multiple tasks recorded -- Found: {task_names}"
-                )
+        task_name = self._get_recorded_task_name(task_name)
 
         if output_comparator is None and output_scorer is None:
             output_comparator = model_graded_comparator
             assert (
                 task_objective is not None
             ), "Must provide an objective to compare or an output comparator"
 
@@ -773,42 +724,38 @@
                     and c.output != "None"
                 }
                 checkpoint_ids = sorted(checkpoints.keys(), reverse=True)
 
                 if len(checkpoint_ids) == 0:
                     continue
 
-                scores: dict[str, OutputScore] = {}
                 if output_scorer is not None:
+                    # TODO: change output scorer to score multiple output types
                     print(f"\nInput #{idx} - Scoring {len(checkpoint_ids)} checkpoints")
                     for checkpoint_id in checkpoint_ids:
                         checkpoint_to_score = checkpoints[checkpoint_id]
-                        if (
-                            use_cached_scores
-                            and checkpoint_to_score.output_score is not None
-                        ):
+                        if use_cached_scores and checkpoint_to_score.scores:
                             print(
-                                f"Using cached score for {checkpoint_id}: {checkpoint_to_score.output_score}"
+                                f"Using cached score for {checkpoint_id}: {checkpoint_to_score.scores}"
                             )
-                            scores[checkpoint_id] = checkpoint_to_score.output_score
-                            continue
 
                         assert checkpoint_to_score.output is not None
-                        score = output_scorer(
+                        multi_output_scores = output_scorer(
                             task_objective or "",
                             checkpoint_to_score.get_input_variables(),
                             checkpoint_to_score.output,
+                            checkpoint_to_score.intermediary_state,
                         )
-                        self.recorder.record_output_score(
+                        self.recorder.record_output_scores(
                             task_name=task_name,
                             checkpoint_id=checkpoint_id,
-                            score=score,
+                            scores=multi_output_scores,
                         )
-                        scores[checkpoint_id] = score
-                        print(f"Scored {checkpoint_id}: {score}")
+                        checkpoint_to_score.scores = multi_output_scores
+                        print(f"Scored {checkpoint_id}: {multi_output_scores}")
 
                 if len(checkpoint_ids) < 2:
                     continue
 
                 # Newer checkpoints are at the start of the list so for every comparison
                 # we compare the newer_checkpoint_id with the older_checkpoint_id
                 to_compare = [
@@ -846,26 +793,29 @@
                             task_name=task_name,
                             older_checkpoint_id=older_checkpoint_id,
                             newer_checkpoint_id=newer_checkpoint_id,
                         )
                     ):
                         print(f"Using cached comparison result for {input_hash}")
                         should_record_comparison = False
-                        output_comparison_feedback = comparator_result.output_feedback
+                        comparison_feedback = comparator_result.feedback
                     elif output_comparator is not None:
-                        output_comparison_feedback = output_comparator(
-                            objective=task_objective or "",
+                        comparison_feedback = output_comparator(
                             input_variables=newer_checkpoint.get_input_variables(),
                             older_checkpoint_output=older_checkpoint_output,
                             newer_checkpoint_output=newer_checkpoint_output,
+                            task_objective=task_objective or "",
+                            objectives_intermediary_state=intermediate_objectives,
+                            older_checkpoint_intermediary_state=older_checkpoint.intermediary_state,
+                            newer_checkpoint_intermediary_state=newer_checkpoint.intermediary_state,
                         )
                     elif output_scorer is not None:
-                        output_comparison_feedback = output_feedback_from_scores(
-                            older_score=scores[older_checkpoint_id],
-                            newer_score=scores[newer_checkpoint_id],
+                        comparison_feedback = output_feedback_from_scores(
+                            older_scores=older_checkpoint.scores,
+                            newer_scores=newer_checkpoint.scores,
                         )
                     else:
                         raise ValueError(
                             "Should not happen. We need an output comparator or output scorer"
                         )
 
                     new_unique_params = []
@@ -909,14 +859,15 @@
                         older_checkpoint.rerun_metadata.get("id")
                         if older_checkpoint.rerun_metadata is not None
                         else None
                     )
 
                     num_comparisons += 1
 
+                    output_comparison_feedback = comparison_feedback[TASK_OUTPUT_KEY]
                     if output_comparison_feedback.result == FeedbackResult.NEUTRAL:
                         print(
                             f"{ORANGE}[neutral] task output is the same between checkpoints {older_checkpoint_id} {old_unique_params_str} & {newer_checkpoint_id} {new_unique_params_str} {END_CLR}"
                         )
                         params_to_succesful_examples[new_params_str] += 1
                         params_to_succesful_examples[old_params_str] += 1
                         if rerun_id_new is not None:
@@ -940,15 +891,15 @@
                     if should_record_comparison:
                         self.recorder.record_comparison_result(
                             task_name=task_name,
                             input_hash=input_hash,
                             result=ComparisonResult(
                                 older_checkpoint_id=older_checkpoint_id,
                                 newer_checkpoint_id=newer_checkpoint_id,
-                                output_feedback=output_comparison_feedback,
+                                feedback=comparison_feedback,
                             ),
                         )
 
             print("\nSummary:")
             print("---------")
             if len(rerun_to_succesful_examples) > 0:
                 print("Your most sucessful re-runs:")
@@ -965,26 +916,213 @@
             for params, num_successes in sorted(
                 params_to_succesful_examples.items(), key=lambda x: x[1], reverse=True
             ):
                 if params == "":
                     params = "default"
                 print(f"{params}: {num_successes}/{num_comparisons} successes")
 
-            self.compute_latest_comparison_results(task_name)
+            self.calculate_system_health(task_name=task_name)
 
         finally:
             self.mode = EvaluatorMode.RECORD
 
+    def calculate_system_health(
+        self,
+        num_samples: int = 10,
+        plotting_frequency_in_days: int = 1,
+        task_name: Optional[str] = None,
+    ) -> None:
+        task_name = self._get_recorded_task_name(task_name=task_name)
+        output_names_to_score: set[str] = set()
+
+        # calculate rolling average if we have output scores for the last num_samples checkpoints
+        input_hashes = self.recorder.get_input_hashes(task_name=task_name)
+        if len(input_hashes) == 0:
+            print("No input hashes exist for this task")
+
+        all_checkpoints: list[Checkpoint] = []
+        input_hash_to_checkpoints: dict[str, list[Checkpoint]] = {}
+        for input_hash in input_hashes:
+            checkpoints = self.recorder.get_latest_checkpoints(
+                task_name=task_name,
+                input_hash=input_hash,
+                num_checkpoints=num_samples,
+            )
+            input_hash_to_checkpoints[input_hash] = checkpoints
+            all_checkpoints += checkpoints
+
+        all_checkpoints_dict: dict[str, Checkpoint] = {
+            c.checkpoint_id: c for c in all_checkpoints
+        }
+
+        if len(all_checkpoints) == 0:
+            return
+
+        # If the outputs have scores, we can calculate a rolling average
+        scored_checkpoints: list[Checkpoint] = []
+        for c in all_checkpoints:
+            scored_outputs = set(c.scores.keys())
+            if len(scored_outputs) > 0:
+                scored_checkpoints.append(c)
+                output_names_to_score |= scored_outputs
+
+        if len(scored_checkpoints) == 0:
+            # If the outputs don't have scores, we can give the better output a score of 1 and the worse output a score of 0.5 and propagate that score to the older checkpoints
+            comparison_results: list[ComparisonResult] = []
+            for input_hash in input_hashes:
+                comparison_results += (
+                    self.recorder.get_comparison_results_for_input_hash(
+                        task_name=task_name,
+                        input_hash=input_hash,
+                        num_results=num_samples,
+                    )
+                )
+
+            for cr in comparison_results:
+                output_names_to_score |= set(cr.feedback.keys())
+
+            for output_name in output_names_to_score:
+                edges: dict[str, dict[str, float]] = defaultdict(lambda: dict())
+                for comparison_result in comparison_results:
+                    feedback = comparison_result.feedback.get(output_name)
+                    if feedback is None:
+                        continue
+
+                    if feedback.result == FeedbackResult.POSITIVE:
+                        edges[comparison_result.older_checkpoint_id][
+                            comparison_result.newer_checkpoint_id
+                        ] = 1.0
+                    elif feedback.result == FeedbackResult.NEGATIVE:
+                        edges[comparison_result.newer_checkpoint_id][
+                            comparison_result.older_checkpoint_id
+                        ] = 1.0
+                    else:
+                        edges[comparison_result.newer_checkpoint_id][
+                            comparison_result.older_checkpoint_id
+                        ] = 0.0
+                        edges[comparison_result.older_checkpoint_id][
+                            comparison_result.newer_checkpoint_id
+                        ] = 0.0
+                scores = get_score_map(edges)
+                denom = max(scores.values()) if len(scores) > 0 else 0.0
+                for checkpoint_id, score in scores.items():
+                    # TODO: fetch checkpoint if it doesn't exist
+                    # TODO: change input hash to checkpoints dict too
+                    if checkpoint := all_checkpoints_dict.get(checkpoint_id):
+                        checkpoint.scores[output_name] = OutputScore(
+                            score=(score / denom) if denom > 0 else 0.0,
+                            message="",
+                        )
+
+        scored_checkpoints = [c for c in all_checkpoints if len(c.scores) > 0]
+
+        if len(scored_checkpoints) == 0:
+            print(f"Not enough checkpoints with comparisons to calculate system health")
+            return
+
+        rolling_averages: list[dict[str, Any]] = []
+
+        date_to_use = datetime.datetime.utcnow().date()
+        scored_checkpoints.sort(key=lambda x: x.checkpoint_id, reverse=True)
+
+        for output_name in sorted(output_names_to_score):
+            output_display_name = (
+                output_name if output_name != TASK_OUTPUT_KEY else "Task output"
+            )
+            while scored_checkpoints[-1].created_at.date() <= date_to_use:
+                total_score = 0.0
+                num_checkpoints_used = 0
+                input_hash_set = set()
+                for checkpoint in scored_checkpoints:
+                    if num_checkpoints_used >= num_samples:
+                        break
+
+                    if checkpoint.created_at.date() <= date_to_use:
+                        if checkpoint.scores is not None:
+                            total_score += checkpoint.scores[output_name].score
+                            num_checkpoints_used += 1
+                            input_hash_set.add(checkpoint.get_input_hash())
+
+                rolling_averages.append(
+                    {
+                        "date": date_to_use.isoformat(),
+                        "rolling_average": total_score / float(num_checkpoints_used),
+                        "num_checkpoints_used": num_checkpoints_used,
+                        "input_diversity": len(input_hash_set),
+                    }
+                )
+                date_to_use -= datetime.timedelta(days=plotting_frequency_in_days)
+
+            output_table(
+                rolling_averages,
+                title=f"{output_name} system health (Rolling average of scores for the last {num_samples} checkpoints)",
+                column_names=[
+                    "date",
+                    "rolling_average",
+                    "num_checkpoints_used",
+                    "input_diversity",
+                ],
+                markdown_file=os.path.join(
+                    self.data_dir, task_name, "system_health.md"
+                ),
+            )
+
+            input_specific_rows: list[dict[str, str]] = []
+            for input_hash, checkpoints in input_hash_to_checkpoints.items():
+                best_checkpoint: Optional[Checkpoint] = None
+                most_recent_checkpoint: Optional[Checkpoint] = None
+                worst_checkpoint: Optional[Checkpoint] = None
+
+                for checkpoint in checkpoints:
+                    if output_name not in checkpoint.scores:
+                        continue
+
+                    if (
+                        best_checkpoint is None
+                        or checkpoint.scores[output_name].score
+                        > best_checkpoint.scores[output_name].score
+                    ):
+                        best_checkpoint = checkpoint
+                    if (
+                        most_recent_checkpoint is None
+                        or checkpoint.created_at > most_recent_checkpoint.created_at
+                    ):
+                        most_recent_checkpoint = checkpoint
+                    if (
+                        worst_checkpoint is None
+                        or checkpoint.scores[output_name].score
+                        < worst_checkpoint.scores[output_name].score
+                    ):
+                        worst_checkpoint = checkpoint
+
+                row_data = dict(checkpoint.input_variables)
+                if best_checkpoint is not None:
+                    row_data["best_checkpoint"] = best_checkpoint.output_score_repr(
+                        output_name=output_name
+                    )
+                if most_recent_checkpoint is not None:
+                    row_data[
+                        "most_recent_checkpoint"
+                    ] = most_recent_checkpoint.output_score_repr(output_name)
+                if worst_checkpoint is not None:
+                    row_data["worst_checkpoint"] = worst_checkpoint.output_score_repr(
+                        output_name=output_name
+                    )
+                input_specific_rows.append(row_data)
+            output_table(input_specific_rows, title=f"{output_name} per input stats")
+
 
 _default_evaluator = Evaluator()
 
 
 set_config = _default_evaluator.set_config
 record_task = _default_evaluator.record_task
 record_output = _default_evaluator.record_output
 record_input = _default_evaluator.record_input
 get_eval_param = _default_evaluator.get_eval_param
 get_eval_params = _default_evaluator.get_eval_params
 rerun_recorded_examples = _default_evaluator.rerun_recorded_examples
 rate_recorded_examples = _default_evaluator.rate_recorded_examples
 compare_recorded_checkpoints = _default_evaluator.compare_recorded_checkpoints
 delete_checkpoints_for_input_vars = _default_evaluator.delete_checkpoints_for_input_vars
+calculate_system_health = _default_evaluator.calculate_system_health
+record_intermediary_state = _default_evaluator.record_intermediary_state
```

### Comparing `eyeball_pp-0.0.6/eyeball_pp/recorders.py` & `eyeball_pp-0.0.7/eyeball_pp/recorders.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from concurrent.futures import ThreadPoolExecutor
+from datetime import datetime
 import hashlib
 import json
 import pkg_resources
 import yaml
 import os
 import pickle
 from typing import Any, Optional, Protocol
 from dataclasses import dataclass
 import dataclasses
 import requests
 
 from .utils import LruCache
-from .classes import OutputFeedback, OutputScore
+from .classes import MultiOutputFeedback, OutputFeedback, OutputScore, MultiOutputScores
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ComparisonResult:
     older_checkpoint_id: str
     newer_checkpoint_id: str
-    output_feedback: OutputFeedback
+    feedback: MultiOutputFeedback
 
     def as_dict(self):
         return {
             "older_checkpoint_id": self.older_checkpoint_id,
             "newer_checkpoint_id": self.newer_checkpoint_id,
-            "output_feedback": self.output_feedback.as_dict(),
+            "feedback": self.feedback.as_dict(),
         }
 
 
 def get_input_hash(input_variables: dict[str, str]) -> str:
     sorted_input_vars = sorted(
         [
             (str(var_name), str(var_val))
@@ -44,17 +45,20 @@
 
 
 @dataclass
 class Checkpoint:
     checkpoint_id: str
     input_variables: dict[str, str] = dataclasses.field(default_factory=dict)
     eval_params: dict[str, Any] = dataclasses.field(default_factory=dict)
+    intermediary_state: dict[str, str] = dataclasses.field(default_factory=dict)
     output: Optional[str] = None
-    output_feedback: Optional[OutputFeedback] = None
-    output_score: Optional[OutputScore] = None
+    feedback: MultiOutputFeedback = dataclasses.field(
+        default_factory=MultiOutputFeedback
+    )
+    scores: MultiOutputScores = dataclasses.field(default_factory=MultiOutputScores)
     rerun_metadata: dict[str, str] = dataclasses.field(default_factory=dict)
 
     def get_input_variables(self) -> dict[str, str]:
         return dict(self.input_variables)
 
     def get_input_hash(self) -> str:
         return get_input_hash(self.input_variables)
@@ -79,41 +83,75 @@
 
     def as_dict(self) -> dict[str, Any]:
         checkpoint_dict = {
             "checkpoint_id": self.checkpoint_id,
             "input_variables": self.input_variables,
             "output": self.output,
         }
+        if self.intermediary_state:
+            checkpoint_dict["intermediary_state"] = self.intermediary_state
         if self.eval_params:
             checkpoint_dict["eval_params"] = self.eval_params
-        if self.output_feedback is not None:
-            checkpoint_dict["output_feedback"] = self.output_feedback.as_dict()
-        if self.output_score is not None:
-            checkpoint_dict["output_score"] = self.output_score.as_dict()
+        if self.feedback is not None:
+            checkpoint_dict["feedback"] = self.feedback
+        if self.scores is not None:
+            checkpoint_dict["score"] = self.scores
         if self.rerun_metadata:
             checkpoint_dict["rerun_metadata"] = self.rerun_metadata
 
         return checkpoint_dict
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> "Checkpoint":
         return cls(
             checkpoint_id=data["checkpoint_id"],
             input_variables=data["input_variables"],
             eval_params=data.get("eval_params") or {},
             output=data["output"],
-            output_feedback=OutputFeedback.from_dict(data["output_feedback"])
-            if data.get("output_feedback") is not None
-            else None,
-            output_score=OutputScore.from_dict(data["output_score"])
-            if data.get("output_score") is not None
-            else None,
+            feedback=MultiOutputFeedback.from_dict(data["feedback"])
+            if data.get("feedback") is not None
+            else {},
+            scores=MultiOutputScores.from_dict(data.get("score"))
+            if data.get("score") is not None
+            else {},
             rerun_metadata=data.get("rerun_metadata") or {},
+            intermediary_state=data.get("intermediary_state") or {},
         )
 
+    @property
+    def created_at(self) -> datetime:
+        return datetime.fromisoformat(self.checkpoint_id)
+
+    def output_score_repr(self, output_name: str) -> str:
+        time_ago = datetime.now() - self.created_at
+        if time_ago.days > 0:
+            msg = f"@ {time_ago.days} days ago"
+        elif time_ago.seconds > 3600:
+            msg = f"@ {time_ago.seconds // 3600} hours ago"
+        elif time_ago.seconds > 60:
+            msg = f"@ {time_ago.seconds // 60} minutes ago"
+        else:
+            msg = f"@ {time_ago.seconds} seconds ago"
+        msg += "\n"
+
+        if output_name in self.scores:
+            output_score = self.scores[output_name]
+            msg += f"score: {output_score.score:.2f}"
+            if output_score.message:
+                msg += f" ({output_score.message})"
+            msg += "\n"
+
+        params_str = ", ".join(f"{k}={v}" for k, v in self.eval_params.items())
+        if params_str:
+            msg += f"({params_str})\n"
+
+        if self.output is not None:
+            msg += self.output[:140]
+        return msg
+
 
 class EvalRecorder(Protocol):
     def record_input_variable(
         self,
         task_name: str,
         checkpoint_id: str,
         variable_name: str,
@@ -125,36 +163,45 @@
         self,
         task_name: str,
         checkpoint_id: str,
         output: str,
     ) -> None:
         ...
 
+    def record_intermediary_state(
+        self,
+        task_name: str,
+        checkpoint_id: str,
+        state_name: str,
+        state_value: str,
+    ) -> None:
+        ...
+
     def record_eval_params(
         self,
         task_name: str,
         checkpoint_id: str,
         eval_params: dict[str, Any],
         rerun_metadata: Optional[dict[str, Any]] = None,
     ) -> None:
         ...
 
     def record_output_feedback(
         self,
         task_name: str,
         checkpoint_id: str,
-        feedback: OutputFeedback,
+        feedback: MultiOutputFeedback,
     ) -> None:
         ...
 
-    def record_output_score(
+    def record_output_scores(
         self,
         task_name: str,
         checkpoint_id: str,
-        score: OutputScore,
+        scores: MultiOutputScores,
     ) -> None:
         ...
 
     def get_checkpoint(
         self, task_name: str, checkpoint_id: str
     ) -> Optional[Checkpoint]:
         ...
@@ -204,18 +251,19 @@
         ...
 
 
 class ApiClientRecorder(EvalRecorder):
     def __init__(self, api_key: str, api_url: Optional[str] = None) -> None:
         self.api_key = api_key
         if api_url is None:
-            self.url = "https://eyeball.tark.ai/"
+            self.url = "https://eyeball-dot-robust-ai.uc.r.appspot.com"
         else:
             self.url = api_url
         self.checkpoint_dicts: LruCache = LruCache(max_size=100)
+        self.comparison_results_dict: LruCache = LruCache(max_size=100)
         self.pool = ThreadPoolExecutor(max_workers=1)
 
     def _get_headers(self) -> dict[str, str]:
         return {
             "Authorization": f"Bearer {self.api_key}",
         }
 
@@ -281,20 +329,31 @@
             checkpoint_id=checkpoint_id,
             prefixes=[],
             name="output",
             value=output,
             flush=True,
         )
 
+    def record_intermediary_state(
+        self, task_name: str, checkpoint_id: str, state_name: str, state_value: str
+    ) -> None:
+        self._record_checkpoint(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            prefixes=["intermediary_state"],
+            name=state_name,
+            value=state_value,
+        )
+
     def record_eval_params(
         self,
         task_name: str,
         checkpoint_id: str,
         eval_params: dict[str, Any],
-        rerun_metadata: dict[str, Any] | None = None,
+        rerun_metadata: Optional[dict[str, Any]] = None,
     ) -> None:
         self._record_checkpoint(
             task_name=task_name,
             checkpoint_id=checkpoint_id,
             prefixes=[],
             name="eval_params",
             value=eval_params,
@@ -317,29 +376,29 @@
                 "task_name": task_name,
                 "input_hash": input_hash,
                 "result": result.as_dict(),
             },
             headers=self._get_headers(),
         )
 
-    def record_output_score(
-        self, task_name: str, checkpoint_id: str, score: OutputScore
+    def record_output_scores(
+        self, task_name: str, checkpoint_id: str, scores: dict[str, OutputScore]
     ) -> None:
         requests.post(
-            f"{self.url}/record_output_score",
+            f"{self.url}/record_output_scores",
             json={
                 "task_name": task_name,
                 "checkpoint_id": checkpoint_id,
-                "score": score.as_dict(),
+                "scores": scores,
             },
             headers=self._get_headers(),
         )
 
     def record_output_feedback(
-        self, task_name: str, checkpoint_id: str, feedback: OutputFeedback
+        self, task_name: str, checkpoint_id: str, feedback: MultiOutputFeedback
     ) -> None:
         requests.post(
             f"{self.url}/record_output_feedback",
             json={
                 "task_name": task_name,
                 "checkpoint_id": checkpoint_id,
                 "feedback": feedback.as_dict(),
@@ -348,63 +407,63 @@
         )
 
     def delete_checkpoints_for_input_hash(
         self, task_name: str, input_hash: str
     ) -> None:
         ...
 
-    def get_checkpoint(self, task_name: str, checkpoint_id: str) -> Checkpoint | None:
+    def get_checkpoint(self, task_name: str, checkpoint_id: str) -> Checkpoint:
         dict_key = f"{task_name},{checkpoint_id}"
         if dict_key in self.checkpoint_dicts:
             return Checkpoint(**(self.checkpoint_dicts[dict_key]))
 
         response = requests.get(
             f"{self.url}/get_checkpoint",
-            json={
+            params={
                 "task_name": task_name,
                 "checkpoint_id": checkpoint_id,
             },
             headers=self._get_headers(),
         )
         if response.status_code != 200:
             logger.debug(
                 f"Failed to get checkpoint - {checkpoint_id}: {response.status_code}"
             )
             return None
         return Checkpoint(**response.json())
 
     def get_comparison_result(
         self, task_name: str, older_checkpoint_id: str, newer_checkpoint_id: str
-    ) -> ComparisonResult | None:
+    ) -> ComparisonResult:
         ...
 
     def get_comparison_results_for_input_hash(
         self, task_name: str, input_hash: str, num_results: int = 3
     ) -> list[ComparisonResult]:
         return []
 
     def get_input_hashes(self, task_name: str) -> list[str]:
         response = requests.get(
             f"{self.url}/get_input_hashes",
-            json={
+            params={
                 "task_name": task_name,
             },
             headers=self._get_headers(),
         )
         if response.status_code != 200:
             logger.debug(f"Failed to get input hashes: {response.status_code}")
             return []
         return response.json()["input_hashes"]
 
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
     ) -> list[Checkpoint]:
         response = requests.get(
             f"{self.url}/get_latest_checkpoints",
-            json={
+            params={
                 "task_name": task_name,
                 "input_hash": input_hash,
                 "num_checkpoints": num_checkpoints,
             },
             headers=self._get_headers(),
         )
         if response.status_code != 200:
@@ -501,14 +560,22 @@
 
     def record_output(self, task_name: str, checkpoint_id: str, output: str) -> None:
         checkpoint = self._fetch_or_create_checkpoint(
             task_name=task_name, checkpoint_id=checkpoint_id
         )
         checkpoint.output = output
 
+    def record_intermediary_state(
+        self, task_name: str, checkpoint_id: str, state_name: str, state_value: str
+    ) -> None:
+        checkpoint = self._fetch_or_create_checkpoint(
+            task_name=task_name, checkpoint_id=checkpoint_id
+        )
+        checkpoint.intermediary_state[state_name] = state_value
+
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
     ) -> list[Checkpoint]:
         if task_name not in self.tasks:
             return []
         task = self.tasks[task_name]
         if input_hash not in task.input_hashes:
@@ -562,20 +629,20 @@
         if rerun_metadata is not None:
             checkpoint.rerun_metadata = rerun_metadata
 
     def record_output_feedback(
         self,
         task_name: str,
         checkpoint_id: str,
-        feedback: OutputFeedback,
+        feedback: MultiOutputFeedback,
     ) -> None:
         checkpoint = self._fetch_or_create_checkpoint(
             task_name=task_name, checkpoint_id=checkpoint_id
         )
-        checkpoint.output_feedback = feedback
+        checkpoint.feedback = feedback
 
     def get_task_names(self) -> list[str]:
         return list(self.tasks.keys())
 
     def record_comparison_result(
         self,
         task_name: str,
@@ -586,24 +653,24 @@
         key = f"{result.older_checkpoint_id},{result.newer_checkpoint_id}"
         task.comparison_results[key] = result
 
         if input_hash not in task.input_hash_to_comparison_results:
             task.input_hash_to_comparison_results[input_hash] = set()
         task.input_hash_to_comparison_results[input_hash].add(key)
 
-    def record_output_score(
+    def record_output_scores(
         self,
         task_name: str,
         checkpoint_id: str,
-        score: OutputScore,
+        scores: MultiOutputScores,
     ) -> None:
         checkpoint = self._fetch_or_create_checkpoint(
             task_name=task_name, checkpoint_id=checkpoint_id
         )
-        checkpoint.output_score = score
+        checkpoint.scores = scores
 
     def get_comparison_result(
         self,
         task_name: str,
         older_checkpoint_id: str,
         newer_checkpoint_id: str,
     ) -> Optional[ComparisonResult]:
@@ -763,14 +830,29 @@
             checkpoint_id=checkpoint_id,
             prefixes=[],
             name="input_hash",
             value=input_hash,
             flush=True,
         )
 
+    def record_intermediary_state(
+        self,
+        task_name: str,
+        checkpoint_id: str,
+        state_name: str,
+        state_value: str,
+    ) -> None:
+        self._record_checkpoint(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            prefixes=["intermediary_state"],
+            name=state_name,
+            value=state_value,
+        )
+
     def record_eval_params(
         self,
         task_name: str,
         checkpoint_id: str,
         eval_params: dict[str, Any],
         rerun_metadata: Optional[dict[str, Any]] = None,
     ) -> None:
@@ -790,55 +872,52 @@
                 value=rerun_metadata,
             )
 
     def record_output_feedback(
         self,
         task_name: str,
         checkpoint_id: str,
-        feedback: OutputFeedback,
+        feedback: MultiOutputFeedback,
     ) -> None:
         self._record_checkpoint(
             task_name=task_name,
             checkpoint_id=checkpoint_id,
             prefixes=[],
-            name="output_feedback",
+            name="feedback",
             value=feedback.as_dict(),
             flush=True,
         )
 
-    def record_output_score(
-        self,
-        task_name: str,
-        checkpoint_id: str,
-        score: OutputScore,
+    def record_output_scores(
+        self, task_name: str, checkpoint_id: str, scores: MultiOutputScores
     ) -> None:
         self._record_checkpoint(
             task_name=task_name,
             checkpoint_id=checkpoint_id,
             prefixes=[],
-            name="output_score",
-            value=score.as_dict(),
+            name="score",
+            value=scores.as_dict(),
             flush=True,
         )
 
     def _checkpoint_from_yaml_dict(
         self, yaml_dict: dict[str, Any], checkpoint_id: str
     ) -> Checkpoint:
         checkpoint = Checkpoint(checkpoint_id=checkpoint_id)
         checkpoint.input_variables = yaml_dict.get("input_variables", {})
         checkpoint.eval_params = yaml_dict.get("eval_params", {})
         checkpoint.output = yaml_dict.get("output")
-        checkpoint.output_feedback = (
-            OutputFeedback.from_dict(yaml_dict.get("output_feedback"))
-            if "output_feedback" in yaml_dict
+        checkpoint.feedback = (
+            MultiOutputFeedback.from_dict(yaml_dict.get("feedback"))
+            if "feedback" in yaml_dict
             else None
         )
-        checkpoint.output_score = (
-            OutputScore.from_dict(yaml_dict.get("output_score"))
-            if "output_score" in yaml_dict
+        checkpoint.scores = (
+            MultiOutputScores.from_dict(yaml_dict.get("scores"))
+            if "scores" in yaml_dict
             else None
         )
         checkpoint.rerun_metadata = yaml_dict.get("rerun_metadata") or {}
         return checkpoint
 
     def get_checkpoint(
         self, task_name: str, checkpoint_id: str
@@ -904,15 +983,15 @@
         comparison_dir = os.path.join(self.dir_path, task_name, "comparison_results")
         if not os.path.exists(comparison_dir):
             os.makedirs(comparison_dir)
 
         file_name = f"{input_hash}_{result.older_checkpoint_id}_{result.newer_checkpoint_id}.yaml"
         file_path = os.path.join(comparison_dir, file_name)
         yaml.dump(
-            result.output_feedback.as_dict(),
+            result.feedback.as_dict(),
             open(file_path, "w+"),
         )
 
     def get_comparison_result(
         self,
         task_name: str,
         older_checkpoint_id: str,
@@ -935,15 +1014,15 @@
 
             if file_name.endswith(".yaml"):
                 file_path = os.path.join(comparison_dir, file_name)
                 yaml_dict = yaml.load(open(file_path, "r"), Loader=yaml.FullLoader)
                 return ComparisonResult(
                     older_checkpoint_id=older_checkpoint_id,
                     newer_checkpoint_id=newer_checkpoint_id,
-                    output_feedback=OutputFeedback.from_dict(yaml_dict),
+                    feedback=MultiOutputFeedback.from_dict(yaml_dict),
                 )
         return None
 
     def get_comparison_results_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
@@ -965,15 +1044,15 @@
             if file_name.endswith(".yaml"):
                 file_path = os.path.join(comparison_dir, file_name)
                 yaml_dict = yaml.load(open(file_path, "r"), Loader=yaml.FullLoader)
                 results.append(
                     ComparisonResult(
                         older_checkpoint_id=splits[1],
                         newer_checkpoint_id=splits[2],
-                        output_feedback=OutputFeedback.from_dict(yaml_dict),
+                        feedback=MultiOutputFeedback.from_dict(yaml_dict),
                     )
                 )
         return sorted(results, key=lambda x: x.newer_checkpoint_id, reverse=True)[
             :num_results
         ]
 
     def delete_checkpoints_for_input_hash(
@@ -1004,14 +1083,29 @@
             task_name=task_name,
             checkpoint_id=checkpoint_id,
             variable_name=variable_name,
             value=value,
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
 
+    def record_intermediary_state(
+        self,
+        task_name: str,
+        checkpoint_id: str,
+        state_name: str,
+        state_value: str,
+    ) -> None:
+        self.memory_recorder.record_intermediary_state(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            state_name=state_name,
+            state_value=state_value,
+        )
+        pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
+
     def record_eval_params(
         self,
         task_name: str,
         checkpoint_id: str,
         eval_params: dict[str, Any],
         rerun_metadata: Optional[dict[str, Any]] = None,
     ) -> None:
@@ -1023,15 +1117,15 @@
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
 
     def record_output_feedback(
         self,
         task_name: str,
         checkpoint_id: str,
-        feedback: OutputFeedback,
+        feedback: MultiOutputFeedback,
     ) -> None:
         self.memory_recorder.record_output_feedback(
             task_name=task_name,
             checkpoint_id=checkpoint_id,
             feedback=feedback,
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
@@ -1063,22 +1157,22 @@
         result: ComparisonResult,
     ) -> None:
         self.memory_recorder.record_comparison_result(
             task_name=task_name, input_hash=input_hash, result=result
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
 
-    def record_output_score(
+    def record_output_scores(
         self,
         task_name: str,
         checkpoint_id: str,
-        score: OutputScore,
+        scores: MultiOutputScores,
     ) -> None:
-        self.memory_recorder.record_output_score(
-            task_name=task_name, checkpoint_id=checkpoint_id, score=score
+        self.memory_recorder.record_output_scores(
+            task_name=task_name, checkpoint_id=checkpoint_id, scores=scores
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
 
     def get_comparison_result(
         self,
         task_name: str,
         older_checkpoint_id: str,
@@ -1118,10 +1212,7 @@
         task_name: str,
         input_hash: str,
     ) -> None:
         self.memory_recorder.delete_checkpoints_for_input_hash(
             task_name=task_name, input_hash=input_hash
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
-
-    def compute_latest_comparison_results(self, task_name: str) -> None:
-        ...
```

### Comparing `eyeball_pp-0.0.6/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.7/eyeball_pp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 eyeball_pp is a framework to evaluate and benchmark tasks which use llms.
 
 This framework helps you answer questions like: "Which llm is the best for my specific task?" or "This prompt change looks good on the example I just tested, does it work with all the other things I've tested?"
 
 Your task can be arbitrary, the framework only cares about initial inputs and final outputs.
 
-If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner.
+If you've been eyeballing how well your changes are working, this framework should fit right in and help you evaluate your task in a more methodical manner WITHOUT you having to become methodical.
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Example
```

### Comparing `eyeball_pp-0.0.6/setup.cfg` & `eyeball_pp-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eyeball_pp
-version = 0.0.6
+version = 0.0.7
 description = A python package for evaluating tasks which use llms
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Revant
 author_email = revant.kapoor@gmail.com
 url = https://github.com/revantk/eyeball-plus-plus
 license_files = LICENSE
```

