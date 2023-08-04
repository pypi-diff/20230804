# Comparing `tmp/mutual-0.3.3.tar.gz` & `tmp/mutual-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.3.3.tar", last modified: Mon Jul 31 05:48:30 2023, max compression
+gzip compressed data, was "mutual-0.3.4.tar", last modified: Fri Aug  4 07:47:28 2023, max compression
```

## Comparing `mutual-0.3.3.tar` & `mutual-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.909247 mutual-0.3.3/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.3/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-31 05:48:30.908999 mutual-0.3.3/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.3/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.907767 mutual-0.3.3/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.3/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    13069 2023-07-31 05:46:52.000000 mutual-0.3.3/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4980 2023-07-31 05:47:35.000000 mutual-0.3.3/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.3/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.3/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.3/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.3/mutual/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.3/mutual/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.3/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-31 05:05:14.000000 mutual-0.3.3/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.908772 mutual-0.3.3/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-31 05:48:30.909299 mutual-0.3.3/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-31 05:48:17.000000 mutual-0.3.3/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.636569 mutual-0.3.4/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.4/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-08-04 07:47:28.636284 mutual-0.3.4/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.4/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.631289 mutual-0.3.4/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4340 2023-08-04 07:44:12.000000 mutual-0.3.4/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.635807 mutual-0.3.4/mutual/api_resources/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-08-02 06:46:48.000000 mutual-0.3.4/mutual/api_resources/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    13226 2023-08-04 07:25:46.000000 mutual-0.3.4/mutual/api_resources/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4988 2023-08-04 07:23:14.000000 mutual-0.3.4/mutual/api_resources/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.4/mutual/api_resources/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.4/mutual/api_resources/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.4/mutual/api_resources/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.4/mutual/api_resources/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.4/mutual/api_resources/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.4/mutual/api_resources/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      358 2023-08-04 02:43:31.000000 mutual-0.3.4/mutual/api_resources/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.632469 mutual-0.3.4/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      509 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-08-04 07:47:28.636623 mutual-0.3.4/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-08-04 07:45:56.000000 mutual-0.3.4/setup.py
```

### Comparing `mutual-0.3.3/LICENSE.txt` & `mutual-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/PKG-INFO` & `mutual-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.3.3/README.md` & `mutual-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/APIKey.py` & `mutual-0.3.4/mutual/api_resources/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/Bot.py` & `mutual-0.3.4/mutual/api_resources/Bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 import mutual
 import io
-from typing import List, Union, Any, Tuple
+from typing import List, Union, Tuple
 
 bot_default_response = {
             "bot_id": None,
             "bot_name": None,
             "bot_chat_index": None,
             "prompt_id": None,
             "judge_id": None,
@@ -148,15 +148,15 @@
         if response.status_code < 300:
             return response.json()
         else:
             self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             return self.default_stream_response
 
     def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, 
-            flow=False, error_logs=False, stream=True, judge=True):
+            flow=False, error_logs=False, stream=True, judge=True, recommendations=False):
         
         url = f"{mutual.endpoint}/chat"
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
@@ -168,58 +168,58 @@
             "username": username,
             "prompt_id": self.prompt_id,
             "judge_id": self.judge_id,
             "judge_message_id": self.judge_message_id,
             "material_id": self.material_id,
             "multiplayer": multiplayer_memory,
             "context_window": context_window,
+            "recommendations": recommendations,
             "stream": stream,
             "judge": judge,
         }
         
         if flow or stream:
             return self._chat_stream(content=content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory,
                                      context_window=context_window,flow=flow,error_logs=error_logs,
-                                     url=url, headers=headers, data=data, stream = stream)
+                                     url=url, headers=headers, data=data, stream = stream, recommendations=recommendations)
         else:
             return self._chat_response(content=content, flow=flow, url=url, headers=headers, data=data)
         
     def _chat_stream(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, 
-            flow=False, error_logs=False, url = None, headers = None, data = None, stream= True):
+            flow=False, error_logs=False, url = None, headers = None, data = None, stream= True, recommendations=False):
         
         if not content:
             print("Please add a message to the content.")
             print("\n\n", end="", flush=True)
             if flow or self.flow:
                 new_content = input("Please enter a new response or type exit to exit: ")
                 if new_content.strip().lower() == "exit":
                     return
                 for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory,
-                                    context_window=context_window, flow=flow, stream=stream):
+                                    context_window=context_window, flow=flow, stream=stream, recommendations=recommendations):
                     yield msg
             return self.default_stream_response
         
         data['stream'] = True
         response = requests.post(url, data=json.dumps(data), headers=headers, stream=stream)
 
         if response.status_code < 300:
             # add the newly created bot to the bot class
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     yield line
-                    yield "\n"
             
             if flow or self.flow:
                 print("\n\n", end="", flush=True)
                 new_content = input("Please enter a new response or type exit to exit: ")
                 if new_content.strip().lower() == "exit":
                     return
                 for msg in self.chat(content=new_content, username=username, prompt=prompt, 
                                      multiplayer_memory=multiplayer_memory, context_window=context_window, 
-                                     flow=flow, stream=stream):
+                                     flow=flow, stream=stream, recommendations=recommendations):
                     yield msg
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
 
     def _chat_response(self, content=None, flow=False, url = None, headers = None, data = None):
```

### Comparing `mutual-0.3.3/mutual/Chat.py` & `mutual-0.3.4/mutual/api_resources/Chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                             }
                         },
                     }
 
 def create(content, bot_name=None, username=None, prompt=None, bot_id=None, prompt_id=None,
             judge_id=None, judge_message_id=None, material_id=None,
             error_logs=False, multiplayer_memory = True, judge = False, stream = True,
+            recommendations=False,
             context_window = 2):
     
     if bot_id is None:
         bot_id = mutual.bot_id
     if bot_id is None and bot_name is None:
         raise ValueError("bot_id or bot_name must be provided either as argument or set in config")
 
@@ -67,15 +68,14 @@
 def _create_stream(url=None, data=None, headers=None, error_logs = False):
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
         for line in response.iter_lines():
             if line:  # filter out keep-alive new lines
                 yield line
-                yield "\n"
     else:
         # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
         default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_stream_response
     
 def _create_response(url=None, data=None, headers=None):
     response = requests.post(url, data=json.dumps(data), headers=headers)
```

### Comparing `mutual-0.3.3/mutual/Dev.py` & `mutual-0.3.4/mutual/api_resources/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/Judge.py` & `mutual-0.3.4/mutual/api_resources/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/JudgeMessage.py` & `mutual-0.3.4/mutual/api_resources/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/Material.py` & `mutual-0.3.4/mutual/api_resources/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/Memory.py` & `mutual-0.3.4/mutual/api_resources/Memory.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/Prompt.py` & `mutual-0.3.4/mutual/api_resources/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.3/mutual/__init__.py` & `mutual-0.3.4/mutual/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # __init__.py
-from . import Bot, Chat, Prompt, Judge, JudgeMessage, APIKey, Dev, Material, Memory
+from mutual.api_resources import (
+    Bot, 
+    Chat, 
+    Prompt, 
+    Judge, 
+    JudgeMessage, 
+    APIKey, 
+    Dev, 
+    Material, 
+    Memory
+)
 
 api_key = None
 bot_id = None
 
 # production
 endpoint = "https://api-agent.mutuai.io/api"
 # development
@@ -83,7 +93,10 @@
                                material_id or response['material_id'] or "default")
     
     print(f"Successfully Fetched and Generated Bot named {response['bot_name']} with an id: {response['bot_id']}")
     print("\n", end="", flush=True)
 
     bot_id = response['bot_id']
     return new_bot_instance
+
+
+__all__ = ['api_key', 'bot_id', 'endpoint']
```

### Comparing `mutual-0.3.3/mutual.egg-info/PKG-INFO` & `mutual-0.3.4/mutual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.3.3/setup.py` & `mutual-0.3.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.3.3',  # beta
+    version='0.3.4',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

