# Comparing `tmp/burla-0.1.5.tar.gz` & `tmp/burla-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.1.5.tar", max compression
+gzip compressed data, was "burla-0.1.6.tar", max compression
```

## Comparing `burla-0.1.5.tar` & `burla-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      535 2023-07-27 00:30:39.176725 burla-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      177 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/__init__.py
--rw-r--r--   0        0        0      907 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_config.py
--rw-r--r--   0        0        0     1352 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_logstream.py
--rw-r--r--   0        0        0     5353 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_remote_parallel_map.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      535 2023-08-04 16:41:29.800188 burla-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-08-04 16:41:29.800188 burla-0.1.6/src/burla/__init__.py
+-rw-r--r--   0        0        0      907 2023-08-04 16:41:29.800188 burla-0.1.6/src/burla/_config.py
+-rw-r--r--   0        0        0     1352 2023-08-04 16:41:29.800188 burla-0.1.6/src/burla/_logstream.py
+-rw-r--r--   0        0        0     5116 2023-08-04 16:41:29.800188 burla-0.1.6/src/burla/_remote_parallel_map.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.6/PKG-INFO
```

### Comparing `burla-0.1.5/pyproject.toml` & `burla-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burla"
-version = "0.1.5"
+version = "0.1.6"
 description = "Scale your program across 1000s of computers with one line of code."
 authors = ["Jake Zuliani <jake@burla.dev>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dill = "^0.3.6"
```

### Comparing `burla-0.1.5/src/burla/_config.py` & `burla-0.1.6/src/burla/_config.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.5/src/burla/_logstream.py` & `burla-0.1.6/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.5/src/burla/_remote_parallel_map.py` & `burla-0.1.6/src/burla/_remote_parallel_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
 from burla._config import load_api_key_from_local_config
 
 pickling_support.install()
 
-BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"
+BURLA_SERVICE_URL = "https://burla-webservice-0-1-6-zqhes3whbq-uc.a.run.app"
 JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
 
-MAX_CONCURRENCY = 100  # If your snooping on my code and want to increase this, don't, it wont work.
+MAX_CONCURRENCY = 500  # If your snooping on my code and want to increase this, don't, it wont work
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
     def __init__(self, job_id, timeout):
         super().__init__(f"Burla job with id: '{job_id}' timed out after {timeout} seconds.")
@@ -45,21 +45,14 @@
             )
             sleep(2)
             return _get_job_info(job_id, epoch, headers, attempt=attempt + 1)
         else:
             raise e
 
 
-def start_job(function_: Callable, inputs: list, image: str, job_id: str, headers: dict):
-    function_pkl_hex = dill.dumps(function_).hex()
-    data = {"function_pkl_hex": function_pkl_hex, "inputs": inputs, "image": image}
-    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data, headers=headers)
-    response.raise_for_status()
-
-
 def remote_parallel_map(
     function_: Callable,
     inputs: list,
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
     n_batches = math.ceil(len(inputs) / MAX_CONCURRENCY)
@@ -72,42 +65,48 @@
             )
         )
     outputs = []
     input_batches = [
         inputs[i : i + MAX_CONCURRENCY] for i in range(0, len(inputs), MAX_CONCURRENCY)
     ]
     for input_batch in input_batches:
-        outputs.extend(remote_parallel_map_single_batch(function_, input_batch, image, api_key))
+        outputs.extend(_remote_parallel_map_single_batch(function_, input_batch, image, api_key))
 
     all_outputs_are_none = all(item is None for item in outputs)
     if not all_outputs_are_none:
         return outputs
 
 
-def remote_parallel_map_single_batch(
+def _remote_parallel_map_single_batch(
     function_: Callable,
     inputs: list,
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
     # https://www.rfc-editor.org/rfc/rfc7235 <- specifies "correct" api key location
     headers = {"Authorization": f"Bearer {api_key or load_api_key_from_local_config()}"}
 
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={}, headers=headers)
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
-    user_python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
-    default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env:latest"
-    image = image or default_docker_image  # sets image to default_docker_image if image is None
+    if sys.version_info.minor < 8:
+        python_version = f"{sys.version_info.major}.8"
+    else:
+        python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
+
+    data = {
+        "function_pkl_hex": dill.dumps(function_, recurse=True).hex(),
+        "inputs": [dill.dumps(input_).hex() for input_ in inputs],
+        "image": image or f"{JOB_ENV_REPO}/python{python_version}/burla_job_env:latest",
+    }
 
-    # This is on a separate thread so we can print logs before all sub_jobs are running.
-    start_job_thread = Thread(target=start_job, args=(function_, inputs, image, job_id, headers))
     job_started_at_epoch = int(time())
-    start_job_thread.start()
+    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data, headers=headers)
+    response.raise_for_status()
 
     last_epoch = job_started_at_epoch
     epoch = last_epoch
     job_is_running = True
     job_timed_out = False
 
     # Start printing logs generated by this job using a separate thread.
@@ -131,17 +130,17 @@
         last_epoch = epoch
         job_is_running = job["job_is_done"] == False
         job_failed = job.get("error") is not None
         job_timed_out = (time() - job_started_at_epoch) > (TIMEOUT_MIN * 60)
 
     stop_event.set()
     log_thread.join()
-    start_job_thread.join()
 
     if job_failed:
         error = pickle.loads(bytes.fromhex(job.get("error")))
         reraise(*error)
 
     if job_timed_out:
         raise JobTimeoutError(job_id=job_id, timeout=TIMEOUT_MIN)
 
-    return job["return_values"]
+    outputs = [dill.loads(bytes.fromhex(output)) for output in job["return_values"]]
+    return outputs
```

### Comparing `burla-0.1.5/PKG-INFO` & `burla-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.1.5
+Version: 0.1.6
 Summary: Scale your program across 1000s of computers with one line of code.
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

