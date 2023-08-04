# Comparing `tmp/kscope-0.7.0.tar.gz` & `tmp/kscope-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscope-0.7.0.tar", last modified: Tue Jul 11 17:27:38 2023, max compression
+gzip compressed data, was "kscope-0.8.0.tar", last modified: Fri Aug  4 18:13:28 2023, max compression
```

## Comparing `kscope-0.7.0.tar` & `kscope-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-06-12 17:08:10.000000 kscope-0.7.0/LICENSE
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-07-11 17:27:38.794690 kscope-0.7.0/PKG-INFO
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     4960 2023-07-11 17:26:29.000000 kscope-0.7.0/README.md
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/kscope/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      226 2023-07-11 17:26:29.000000 kscope-0.7.0/kscope/__init__.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-06-12 17:08:10.000000 kscope-0.7.0/kscope/hooks.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)    10703 2023-07-11 17:26:29.000000 kscope-0.7.0/kscope/kaleidoscope_sdk.py
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1643 2023-06-12 17:08:10.000000 kscope-0.7.0/kscope/utils.py
-drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-07-11 17:27:38.794690 kscope-0.7.0/kscope.egg-info/
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/PKG-INFO
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/SOURCES.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/dependency_links.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/requires.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-07-11 17:27:38.000000 kscope-0.7.0/kscope.egg-info/top_level.txt
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-07-11 17:27:38.794690 kscope-0.7.0/setup.cfg
--rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-07-11 17:26:29.000000 kscope-0.7.0/setup.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-08-04 18:13:28.379080 kscope-0.8.0/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1073 2023-06-12 17:08:10.000000 kscope-0.8.0/LICENSE
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-08-04 18:13:28.379080 kscope-0.8.0/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     4960 2023-07-11 17:26:29.000000 kscope-0.8.0/README.md
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-08-04 18:13:28.379080 kscope-0.8.0/kscope/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      226 2023-08-04 18:13:17.000000 kscope-0.8.0/kscope/__init__.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      513 2023-06-12 17:08:10.000000 kscope-0.8.0/kscope/hooks.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)    10668 2023-08-04 18:13:17.000000 kscope-0.8.0/kscope/kaleidoscope_sdk.py
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1874 2023-08-04 18:13:17.000000 kscope-0.8.0/kscope/utils.py
+drwxrwxr-x   0 coatsworth  (1000) coatsworth  (1000)        0 2023-08-04 18:13:28.379080 kscope-0.8.0/kscope.egg-info/
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     5909 2023-08-04 18:13:28.000000 kscope-0.8.0/kscope.egg-info/PKG-INFO
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      253 2023-08-04 18:13:28.000000 kscope-0.8.0/kscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        1 2023-08-04 18:13:28.000000 kscope-0.8.0/kscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)      134 2023-08-04 18:13:28.000000 kscope-0.8.0/kscope.egg-info/requires.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)        7 2023-08-04 18:13:28.000000 kscope-0.8.0/kscope.egg-info/top_level.txt
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)       38 2023-08-04 18:13:28.379080 kscope-0.8.0/setup.cfg
+-rw-rw-r--   0 coatsworth  (1000) coatsworth  (1000)     1427 2023-08-04 18:13:17.000000 kscope-0.8.0/setup.py
```

### Comparing `kscope-0.7.0/LICENSE` & `kscope-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kscope-0.7.0/PKG-INFO` & `kscope-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.7.0
+Version: 0.8.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kscope-0.7.0/README.md` & `kscope-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `kscope-0.7.0/kscope/hooks.py` & `kscope-0.8.0/kscope/hooks.py`

 * *Files identical despite different names*

### Comparing `kscope-0.7.0/kscope/kaleidoscope_sdk.py` & `kscope-0.8.0/kscope/kaleidoscope_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,25 +173,25 @@
 
         return response
 
     def get_activations(
         self,
         model_instance_id: str,
         prompts: List[str],
-        module_names: List[str],
+        modules: List[str],
         generation_config: Dict,
     ):
         """Gets activations from the model instance"""
 
         url = self.create_addr(
-            f"models/instances/{model_instance_id}/generate_activations"
+            f"models/instances/{model_instance_id}/get_activations"
         )
         body = {
             "prompts": prompts,
-            "module_names": module_names,
+            "modules": modules,
             "generation_config": generation_config,
         }
 
         response = post(url, body, auth_key=self.auth_key)
 
         return response
 
@@ -261,26 +261,26 @@
         Generation = namedtuple("Generation", generation_response.keys())
 
         return Generation(**generation_response)
 
     def get_activations(
         self,
         prompts: Union[str, List[str]],
-        module_names: List[str],
+        modules: List[str],
         generation_config: Dict = {},
     ):
         """Gets activations from the model instance
         :param prompts: (str or List[str]) Single prompt or list of prompts to generate from.
         Supports upto 8 prompts in a single request.
-        :param module_names: (List[str]) The layer to get activations from
+        :param modules: (List[str]) The layer to get activations from
         """
         if isinstance(prompts, str):
             prompts = [prompts]
         activations_response = self._session.get_activations(
-            self.id, prompts, module_names, generation_config
+            self.id, prompts, modules, generation_config
         )
         for idx in range(len(activations_response["activations"])):
             for elm in activations_response["activations"][idx]:
                 activations_response["activations"][idx][elm] = decode_str(
                     activations_response["activations"][idx][elm]
                 )
         Activations = namedtuple("Activations", activations_response.keys())
```

### Comparing `kscope-0.7.0/kscope/utils.py` & `kscope-0.8.0/kscope/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,27 +20,29 @@
     return codecs.encode(cloudpickle.dumps(obj), "base64").decode("utf-8")
 
 
 def check_response(resp):
     if not resp.ok:
         if resp.status_code == 422:
             raise ValueError(
-                "Request to {} not sucessful, Error Code: {}, please check your auth key".format(
+                "Request to {} not sucessful, Error Code: {}, your JWT token is invalid or incorrect, \
+                please delete the previous token at ~/.kaleidoscope.jwt and generate a new one".format(
                     resp.url, resp.status_code
                 )
             )
-        elif resp.status_code == 400:
+        elif resp.status_code == 401:
             raise ValueError(
-                "Request to {} not sucessful, Error Code: {}, please check your request body".format(
+                "Request to {} not sucessful, Error Code: {}, your JWT token is expired, please \
+                    delete the previous token at ~/.kaleidoscope.jwt and generate a new one".format(
                     resp.url, resp.status_code
                 )
             )
         raise ValueError(
-            "Request to {} not sucessful, Error Code: {}".format(
-                resp.url, resp.status_code
+            "Request to {} not sucessful, Error Code: {}, {}".format(
+                resp.url, resp.status_code, resp.json()["msg"]
             )
         )
     logger.debug("addr %s response code %s", resp.url, resp.status_code)
 
 
 def get(addr, auth_key=None, headers={}):
```

### Comparing `kscope-0.7.0/kscope.egg-info/PKG-INFO` & `kscope-0.8.0/kscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscope
-Version: 0.7.0
+Version: 0.8.0
 Summary: A user toolkit for analyzing and interfacing with Large Language Models (LLMs)
 Home-page: https://github.com/VectorInstitute/kaleidoscope-sdk
 Author: ['Vector AI Engineering']
 Author-email: ai_engineering@vectorinstitute.ai
 License: MIT
 Keywords: python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kscope-0.7.0/setup.py` & `kscope-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="kscope",
-    version="0.7.0",
+    version="0.8.0",
     description="A user toolkit for analyzing and interfacing with Large Language Models (LLMs)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="python nlp machine-learning deep-learning distributed-computing neural-networks tensor llm",
     requires_python=">=3.7",
     url="https://github.com/VectorInstitute/kaleidoscope-sdk",
     author=["Vector AI Engineering"],
```

