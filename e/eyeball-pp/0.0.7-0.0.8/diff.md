# Comparing `tmp/eyeball_pp-0.0.7.tar.gz` & `tmp/eyeball_pp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.7.tar", last modified: Fri Aug  4 00:07:51 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.8.tar", last modified: Fri Aug  4 02:32:18 2023, max compression
```

## Comparing `eyeball_pp-0.0.7.tar` & `eyeball_pp-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.601343 eyeball_pp-0.0.7/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.7/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 00:07:51.601463 eyeball_pp-0.0.7/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8639 2023-08-03 04:44:59.000000 eyeball_pp-0.0.7/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.599155 eyeball_pp-0.0.7/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      881 2023-08-02 22:46:42.000000 eyeball_pp-0.0.7/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     3661 2023-08-03 23:07:44.000000 eyeball_pp-0.0.7/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     5419 2023-08-03 23:07:38.000000 eyeball_pp-0.0.7/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.7/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    46600 2023-08-04 00:07:30.000000 eyeball_pp-0.0.7/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    40035 2023-08-04 00:07:30.000000 eyeball_pp-0.0.7/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)     3879 2023-08-03 20:00:41.000000 eyeball_pp-0.0.7/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 00:07:51.601139 eyeball_pp-0.0.7/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-04 00:07:51.000000 eyeball_pp-0.0.7/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-04 00:07:51.602076 eyeball_pp-0.0.7/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.7/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.285427 eyeball_pp-0.0.8/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.8/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 02:32:18.285586 eyeball_pp-0.0.8/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8639 2023-08-03 04:44:59.000000 eyeball_pp-0.0.8/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.283359 eyeball_pp-0.0.8/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      881 2023-08-02 22:46:42.000000 eyeball_pp-0.0.8/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     3661 2023-08-03 23:07:44.000000 eyeball_pp-0.0.8/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     5419 2023-08-03 23:07:38.000000 eyeball_pp-0.0.8/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.8/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    46598 2023-08-04 01:55:30.000000 eyeball_pp-0.0.8/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    42067 2023-08-04 01:49:39.000000 eyeball_pp-0.0.8/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)     3879 2023-08-03 20:00:41.000000 eyeball_pp-0.0.8/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.285070 eyeball_pp-0.0.8/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-04 02:32:18.286470 eyeball_pp-0.0.8/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.8/setup.py
```

### Comparing `eyeball_pp-0.0.7/LICENSE` & `eyeball_pp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/PKG-INFO` & `eyeball_pp-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `eyeball_pp-0.0.7/README.md` & `eyeball_pp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/eyeball_pp/__init__.py` & `eyeball_pp-0.0.8/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/eyeball_pp/classes.py` & `eyeball_pp-0.0.8/eyeball_pp/classes.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/eyeball_pp/comparators.py` & `eyeball_pp-0.0.8/eyeball_pp/comparators.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/eyeball_pp/eval.py` & `eyeball_pp-0.0.8/eyeball_pp/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -972,18 +972,16 @@
                 comparison_results += (
                     self.recorder.get_comparison_results_for_input_hash(
                         task_name=task_name,
                         input_hash=input_hash,
                         num_results=num_samples,
                     )
                 )
-
             for cr in comparison_results:
                 output_names_to_score |= set(cr.feedback.keys())
-
             for output_name in output_names_to_score:
                 edges: dict[str, dict[str, float]] = defaultdict(lambda: dict())
                 for comparison_result in comparison_results:
                     feedback = comparison_result.feedback.get(output_name)
                     if feedback is None:
                         continue
```

### Comparing `eyeball_pp-0.0.7/eyeball_pp/recorders.py` & `eyeball_pp-0.0.8/eyeball_pp/recorders.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,22 @@
     def as_dict(self):
         return {
             "older_checkpoint_id": self.older_checkpoint_id,
             "newer_checkpoint_id": self.newer_checkpoint_id,
             "feedback": self.feedback.as_dict(),
         }
 
+    @staticmethod
+    def from_dict(data):
+        return ComparisonResult(
+            older_checkpoint_id=data["older_checkpoint_id"],
+            newer_checkpoint_id=data["newer_checkpoint_id"],
+            feedback=MultiOutputFeedback.from_dict(data["feedback"]),
+        )
+
 
 def get_input_hash(input_variables: dict[str, str]) -> str:
     sorted_input_vars = sorted(
         [
             (str(var_name), str(var_val))
             for var_name, var_val in input_variables.items()
         ],
@@ -256,14 +264,15 @@
         self.api_key = api_key
         if api_url is None:
             self.url = "https://eyeball-dot-robust-ai.uc.r.appspot.com"
         else:
             self.url = api_url
         self.checkpoint_dicts: LruCache = LruCache(max_size=100)
         self.comparison_results_dict: LruCache = LruCache(max_size=100)
+
         self.pool = ThreadPoolExecutor(max_workers=1)
 
     def _get_headers(self) -> dict[str, str]:
         return {
             "Authorization": f"Bearer {self.api_key}",
         }
 
@@ -366,23 +375,28 @@
                 name="rerun_metadata",
                 value=rerun_metadata,
             )
 
     def record_comparison_result(
         self, task_name: str, input_hash: str, result: ComparisonResult
     ) -> None:
-        requests.post(
-            f"{self.url}/record_comparison_result",
-            json={
-                "task_name": task_name,
-                "input_hash": input_hash,
-                "result": result.as_dict(),
-            },
-            headers=self._get_headers(),
-        )
+        def _record():
+            requests.post(
+                f"{self.url}/record_comparison_result",
+                json={
+                    "task_name": task_name,
+                    "input_hash": input_hash,
+                    **result.as_dict(),
+                },
+                headers=self._get_headers(),
+            )
+
+        self.pool.submit(_record)
+        key = f"{task_name},{result.older_checkpoint_id},{result.newer_checkpoint_id}"
+        self.comparison_results_dict[key] = result
 
     def record_output_scores(
         self, task_name: str, checkpoint_id: str, scores: dict[str, OutputScore]
     ) -> None:
         requests.post(
             f"{self.url}/record_output_scores",
             json={
@@ -407,15 +421,17 @@
         )
 
     def delete_checkpoints_for_input_hash(
         self, task_name: str, input_hash: str
     ) -> None:
         ...
 
-    def get_checkpoint(self, task_name: str, checkpoint_id: str) -> Checkpoint:
+    def get_checkpoint(
+        self, task_name: str, checkpoint_id: str
+    ) -> Optional[Checkpoint]:
         dict_key = f"{task_name},{checkpoint_id}"
         if dict_key in self.checkpoint_dicts:
             return Checkpoint(**(self.checkpoint_dicts[dict_key]))
 
         response = requests.get(
             f"{self.url}/get_checkpoint",
             params={
@@ -425,25 +441,59 @@
             headers=self._get_headers(),
         )
         if response.status_code != 200:
             logger.debug(
                 f"Failed to get checkpoint - {checkpoint_id}: {response.status_code}"
             )
             return None
-        return Checkpoint(**response.json())
+        return Checkpoint.from_dict(response.json())
 
     def get_comparison_result(
         self, task_name: str, older_checkpoint_id: str, newer_checkpoint_id: str
-    ) -> ComparisonResult:
-        ...
+    ) -> Optional[ComparisonResult]:
+        key = f"{task_name},{older_checkpoint_id},{newer_checkpoint_id}"
+        if key in self.comparison_results_dict:
+            return self.comparison_results_dict[key]
+        else:
+            response = requests.get(
+                f"{self.url}/get_comparison_result",
+                params={
+                    "task_name": task_name,
+                    "older_checkpoint_id": older_checkpoint_id,
+                    "newer_checkpoint_id": newer_checkpoint_id,
+                },
+                headers=self._get_headers(),
+            )
+            if response.status_code != 200:
+                logger.debug(f"Failed to get comparison result: {response.status_code}")
+                return None
+            response_dict = response.json()
+            if "success" in response_dict and not response_dict["success"]:
+                return None
+            return ComparisonResult.from_dict(response_dict)
 
     def get_comparison_results_for_input_hash(
         self, task_name: str, input_hash: str, num_results: int = 3
     ) -> list[ComparisonResult]:
-        return []
+        response = requests.get(
+            f"{self.url}/get_comparison_results_for_input_hash",
+            params={
+                "task_name": task_name,
+                "input_hash": input_hash,
+                "num_results": num_results,
+            },
+            headers=self._get_headers(),
+        )
+        if response.status_code != 200:
+            logger.debug(f"Failed to get comparison results: {response.status_code}")
+            return []
+        return [
+            ComparisonResult.from_dict(data)
+            for data in response.json()["comparison_results"]
+        ]
 
     def get_input_hashes(self, task_name: str) -> list[str]:
         response = requests.get(
             f"{self.url}/get_input_hashes",
             params={
                 "task_name": task_name,
             },
```

### Comparing `eyeball_pp-0.0.7/eyeball_pp/utils.py` & `eyeball_pp-0.0.8/eyeball_pp/utils.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.7/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.8/eyeball_pp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `eyeball_pp-0.0.7/setup.cfg` & `eyeball_pp-0.0.8/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eyeball_pp
-version = 0.0.7
+version = 0.0.8
 description = A python package for evaluating tasks which use llms
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Revant
 author_email = revant.kapoor@gmail.com
 url = https://github.com/revantk/eyeball-plus-plus
 license_files = LICENSE
```

