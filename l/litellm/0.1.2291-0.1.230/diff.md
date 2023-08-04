# Comparing `tmp/litellm-0.1.2291.tar.gz` & `tmp/litellm-0.1.230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.2291.tar", last modified: Thu Aug  3 21:04:36 2023, max compression
+gzip compressed data, was "litellm-0.1.230.tar", last modified: Thu Aug  3 22:06:55 2023, max compression
```

## Comparing `litellm-0.1.2291.tar` & `litellm-0.1.230.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.333102 litellm-0.1.2291/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.2291/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      152 2023-08-03 21:04:36.332961 litellm-0.1.2291/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.2291/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.331304 litellm-0.1.2291/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1201 2023-08-03 21:03:40.000000 litellm-0.1.2291/litellm/__init__.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.332623 litellm-0.1.2291/litellm/integrations/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.2291/litellm/integrations/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.2291/litellm/integrations/helicone.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    12068 2023-08-03 21:04:08.000000 litellm-0.1.2291/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2893 2023-08-03 16:40:54.000000 litellm-0.1.2291/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    15221 2023-08-03 17:14:57.000000 litellm-0.1.2291/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-03 21:04:36.332194 litellm-0.1.2291/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      152 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       80 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-03 21:04:36.000000 litellm-0.1.2291/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.2291/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-03 21:04:36.333147 litellm-0.1.2291/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      547 2023-08-03 21:04:34.000000 litellm-0.1.2291/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.077892 litellm-0.1.230/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-03 22:06:43.000000 litellm-0.1.230/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 22:06:55.073892 litellm-0.1.230/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-03 22:06:43.000000 litellm-0.1.230/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/integrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/integrations/helicone.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-03 22:06:43.000000 litellm-0.1.230/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 22:06:55.077892 litellm-0.1.230/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-03 22:06:43.000000 litellm-0.1.230/setup.py
```

### Comparing `litellm-0.1.2291/LICENSE` & `litellm-0.1.230/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2291/README.md` & `litellm-0.1.230/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2291/litellm/__init__.py` & `litellm-0.1.230/litellm/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 success_callback = []
 failure_callback = []
 set_verbose=False
 telemetry=True
 max_tokens = 256 # OpenAI Defaults
 retry = True # control tenacity retries. 
+openai_key = None 
+azure_key = None 
+anthropic_key = None 
+replicate_key = None 
+cohere_key = None 
 ####### PROXY PARAMS ################### configurable params if you use proxy models like Helicone
 api_base = None
 headers = None
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   "gpt-4",
   "gpt-4-0613",
@@ -31,15 +36,19 @@
 ]
 
 anthropic_models = [
   "claude-2", 
   "claude-instant-1"
 ]
 
-model_list = open_ai_chat_completion_models + open_ai_text_completion_models + cohere_models + anthropic_models
+replicate_models = [
+    "replicate/"
+] # placeholder, to make sure we accept any replicate model in our model_list 
+
+model_list = open_ai_chat_completion_models + open_ai_text_completion_models + cohere_models + anthropic_models + replicate_models
 
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 from .timeout import timeout
 from .utils import client, logging, exception_type  # Import all the symbols from main.py
```

### Comparing `litellm-0.1.2291/litellm/integrations/helicone.py` & `litellm-0.1.230/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2291/litellm/main.py` & `litellm-0.1.230/litellm/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 import traceback
 from functools import partial
 import dotenv
 import traceback
 import litellm
-from litellm import client, logging, exception_type, timeout, success_callback, failure_callback
+from litellm import client, logging, exception_type, timeout
 import random
 import asyncio
 from tenacity import (
     retry,
     stop_after_attempt,
     wait_random_exponential,
 )  # for exponential backoff
@@ -93,15 +93,20 @@
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
       openai.api_base = litellm.api_base if litellm.api_base is not None else os.environ.get("AZURE_API_BASE")
       openai.api_version = os.environ.get("AZURE_API_VERSION")
-      openai.api_key = api_key if api_key is not None else os.environ.get("AZURE_API_KEY")
+      if api_key:
+          openai.api_key = api_key
+      elif litellm.azure_key:
+          openai.api_key = litellm.azure_key
+      else:
+          openai.api_key = os.environ.get("AZURE_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
          response = openai.ChatCompletion.create(
             engine=model,
             messages = messages,
@@ -114,15 +119,20 @@
           messages = messages,
           **optional_params
         )
     elif model in litellm.open_ai_chat_completion_models:
       openai.api_type = "openai"
       openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
-      openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
+      if api_key:
+          openai.api_key = api_key
+      elif litellm.openai_key:
+          openai.api_key = litellm.openai_key
+      else:
+          openai.api_key = os.environ.get("OPENAI_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
          response = openai.ChatCompletion.create(
           model=model,
           messages = messages,
@@ -135,15 +145,20 @@
           messages = messages,
           **optional_params
         )
     elif model in litellm.open_ai_text_completion_models:
       openai.api_type = "openai"
       openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
-      openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
+      if api_key:
+          openai.api_key = api_key
+      elif litellm.openai_key:
+          openai.api_key = litellm.openai_key
+      else:
+          openai.api_key = os.environ.get("OPENAI_API_KEY")
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
         response = openai.Completion.create(
           model=model,
@@ -159,14 +174,17 @@
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       elif api_key:
          os.environ["REPLICATE_API_TOKEN"] = api_key
+      elif litellm.replicate_key:
+         os.environ["REPLICATE_API_TOKEN"] = litellm.replicate_key
+
       prompt = " ".join([message["content"] for message in messages])
       input = {"prompt": prompt}
       if max_tokens != float('inf'):
         input["max_length"] = max_tokens # for t5 models 
         input["max_new_tokens"] = max_tokens # for llama2 models 
       ## LOGGING
       logging(model=model, input=input, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
@@ -190,14 +208,16 @@
         ]
       }
       response = new_response
     elif model in litellm.anthropic_models:
       #anthropic defaults to os.environ.get("ANTHROPIC_API_KEY")
       if api_key:
          os.environ["ANTHROPIC_API_KEY"] = api_key
+      elif litellm.anthropic_key:
+         os.environ["ANTHROPIC_API_TOKEN"] = litellm.anthropic_key
       prompt = f"{HUMAN_PROMPT}" 
       for message in messages:
         if "role" in message:
           if message["role"] == "user":
             prompt += f"{HUMAN_PROMPT}{message['content']}"
           else:
             prompt += f"{AI_PROMPT}{message['content']}"
@@ -229,15 +249,20 @@
             }
           }
         ]
       }
       print_verbose(f"new response: {new_response}")
       response = new_response
     elif model in litellm.cohere_models:
-      cohere_key = api_key if api_key is not None else os.environ.get("COHERE_API_KEY")
+      if api_key:
+        cohere_key = api_key
+      elif litellm.api_key:
+        cohere_key = litellm.api_key
+      else:
+        cohere_key = os.environ.get("COHERE_API_KEY")
       co = cohere.Client(cohere_key)
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = co.generate(  
         model=model,
```

### Comparing `litellm-0.1.2291/litellm/timeout.py` & `litellm-0.1.230/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2291/litellm/utils.py` & `litellm-0.1.230/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2291/setup.py` & `litellm-0.1.230/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.2291',
+    version='0.1.230',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
```

