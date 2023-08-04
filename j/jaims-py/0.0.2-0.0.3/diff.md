# Comparing `tmp/jaims-py-0.0.2.tar.gz` & `tmp/jaims-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims-py-0.0.2.tar", last modified: Thu Jul 20 18:35:34 2023, max compression
+gzip compressed data, was "jaims-py-0.0.3.tar", last modified: Fri Aug  4 13:53:00 2023, max compression
```

## Comparing `jaims-py-0.0.2.tar` & `jaims-py-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.767037 jaims-py-0.0.2/
--rw-r--r--   0 mush       (501) staff       (20)     4181 2023-07-20 18:35:34.766901 jaims-py-0.0.2/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     3851 2023-07-20 18:35:26.000000 jaims-py-0.0.2/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.765982 jaims-py-0.0.2/jaims/
--rw-r--r--   0 mush       (501) staff       (20)      169 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    11006 2023-07-20 18:35:26.000000 jaims-py-0.0.2/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     1134 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/exceptions.py
--rw-r--r--   0 mush       (501) staff       (20)     7636 2023-07-20 18:35:26.000000 jaims-py-0.0.2/jaims/function_handler.py
--rw-r--r--   0 mush       (501) staff       (20)     7698 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/histroy_manager.py
--rw-r--r--   0 mush       (501) staff       (20)     3512 2023-07-20 08:54:39.000000 jaims-py-0.0.2/jaims/openai_wrappers.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-07-20 18:35:34.766616 jaims-py-0.0.2/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     4181 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      306 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       31 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2023-07-20 18:35:34.000000 jaims-py-0.0.2/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2023-07-20 18:35:34.767105 jaims-py-0.0.2/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)      606 2023-07-20 18:35:26.000000 jaims-py-0.0.2/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-04 13:53:00.086020 jaims-py-0.0.3/
+-rw-r--r--   0 mush       (501) staff       (20)     4222 2023-08-04 13:53:00.085898 jaims-py-0.0.3/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     3892 2023-07-21 09:49:32.000000 jaims-py-0.0.3/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-04 13:53:00.084876 jaims-py-0.0.3/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)      191 2023-07-26 10:58:46.000000 jaims-py-0.0.3/jaims/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    11756 2023-07-27 12:27:20.000000 jaims-py-0.0.3/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     1134 2023-07-31 14:08:28.000000 jaims-py-0.0.3/jaims/exceptions.py
+-rw-r--r--   0 mush       (501) staff       (20)     7636 2023-07-27 12:09:18.000000 jaims-py-0.0.3/jaims/function_handler.py
+-rw-r--r--   0 mush       (501) staff       (20)     7877 2023-07-27 10:34:32.000000 jaims-py-0.0.3/jaims/histroy_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)     5388 2023-07-31 13:42:32.000000 jaims-py-0.0.3/jaims/openai_wrappers.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-08-04 13:53:00.085669 jaims-py-0.0.3/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     4222 2023-08-04 13:53:00.000000 jaims-py-0.0.3/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      306 2023-08-04 13:53:00.000000 jaims-py-0.0.3/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2023-08-04 13:53:00.000000 jaims-py-0.0.3/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       31 2023-08-04 13:53:00.000000 jaims-py-0.0.3/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2023-08-04 13:53:00.000000 jaims-py-0.0.3/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2023-08-04 13:53:00.086070 jaims-py-0.0.3/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)      606 2023-08-04 13:52:04.000000 jaims-py-0.0.3/setup.py
```

### Comparing `jaims-py-0.0.2/PKG-INFO` & `jaims-py-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+<p align="center">
+    <img width="300" src="https://github.com/dev-mush/jaims-py/assets/669003/5c53381f-25b5-4141-bcd2-7457863eafb9" >
+</p>
 
-![jaims_logo](https://github.com/dev-mush/jaims/assets/669003/ac429608-6c49-4e41-a361-50da9569bfec)
 
 # jAIms 
 
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
```

### Comparing `jaims-py-0.0.2/README.md` & `jaims-py-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+<p align="center">
+    <img width="300" src="https://github.com/dev-mush/jaims-py/assets/669003/5c53381f-25b5-4141-bcd2-7457863eafb9" >
+</p>
 
-![jaims_logo](https://github.com/dev-mush/jaims/assets/669003/ac429608-6c49-4e41-a361-50da9569bfec)
 
 # jAIms 
 
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
```

### Comparing `jaims-py-0.0.2/jaims/agent.py` & `jaims-py-0.0.3/jaims/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
+import logging
 import os
 from typing import Any, Dict, Generator, List, Optional, Union
 
 import openai
 
 from jaims.openai_wrappers import (
     DEFAULT_MAX_TOKENS,
     MAX_CONSECUTIVE_CALLS,
     JAImsGPTModel,
-    JaimsTokensExpense,
+    JAImsTokensExpense,
     estimate_token_count,
+    get_openai_response,
 )
 from jaims.exceptions import (
     JAImsMissingOpenaiAPIKeyException,
-    JAImsOpenAIErrorException,
     JAImsMaxConsecutiveFunctionCallsExceeded,
 )
 from jaims.function_handler import (
     JAImsFuncWrapper,
     JAImsFunctionHandler,
     parse_functions_to_json,
 )
@@ -57,74 +58,80 @@
 
     Methods
     -------
         run(messages, stream: bool optional) -> JAImsResponse
             performs the call to OpenAI and returns the response
         clear_history()
             clears the agent history
+        get_history(optimized: bool) -> List[dict]
+            returns the current history of the agent, if optimized is passed to True, it will return the
+            optimized version, otherwise the full history since the beginning of this agent session
         get_expenses() -> List[JaimsTokensExpense]
             returns the currently spent tokens for this agent session, one for each model used
 
+
     Raises
     ------
         MissingOpenaiAPIKeyException
             if the OPENAI_API_KEY environment variable is not set and no api key is provided
 
     Private Members
     ---------------
         __history_manager : HistoryManager
             the history manager
     """
 
     def __init__(
         self,
         model=JAImsGPTModel.GPT_3_5_TURBO,
-        functions: List[JAImsFuncWrapper] = [],
-        initial_prompts: Optional[List[Dict]] = [],
+        functions: Optional[List[JAImsFuncWrapper]] = None,
+        initial_prompts: Optional[List[Dict]] = None,
         max_consecutive_calls=MAX_CONSECUTIVE_CALLS,
         optimize_context=True,
         openai_api_key: Optional[str] = None,
     ):
         openai_api_key = openai_api_key or os.getenv("OPENAI_API_KEY")
         if not openai_api_key:
             raise JAImsMissingOpenaiAPIKeyException()
         openai.api_key = openai_api_key
 
         self.model = model
-        self.functions = functions
-        self.initial_prompts = initial_prompts
+        self.functions = functions or []
+        self.initial_prompts = initial_prompts or []
         self.max_consecutive_calls = max_consecutive_calls
         self.__expense = {
-            JAImsGPTModel.GPT_3_5_TURBO.string: JaimsTokensExpense(
+            JAImsGPTModel.GPT_3_5_TURBO.string: JAImsTokensExpense(
                 gpt_model=JAImsGPTModel.GPT_3_5_TURBO
             ),
-            JAImsGPTModel.GPT_3_5_TURBO_16K.string: JaimsTokensExpense(
+            JAImsGPTModel.GPT_3_5_TURBO_16K.string: JAImsTokensExpense(
                 gpt_model=JAImsGPTModel.GPT_3_5_TURBO_16K
             ),
-            JAImsGPTModel.GPT_4.string: JaimsTokensExpense(
+            JAImsGPTModel.GPT_4.string: JAImsTokensExpense(
                 gpt_model=JAImsGPTModel.GPT_4
             ),
         }
         self.__function_handler = JAImsFunctionHandler(self.functions)
         self.__history_manager = HistoryManager(
             model=self.model,
             functions=self.functions,
             mandatory_context=self.initial_prompts,
             optimize_history=optimize_context,
         )
 
     def run(
         self,
-        messages: List[dict] = [],
+        messages: Optional[List[dict]] = None,
         max_tokens: int = DEFAULT_MAX_TOKENS,
         stream: bool = False,
         temperature: float = 0.0,
         top_p: Optional[int] = None,
         n: int = 1,
-        function_call: str = "auto",
+        function_call: Union[str, Dict] = "auto",
+        max_retries: int = 15,
+        delay: int = 10,
     ) -> Union[str, Generator[str, None, None]]:
         """
         Calls OpenAI with the passed parameters and returns or streams the response.
 
         Parameters
         ----------
             messages : list
@@ -141,30 +148,38 @@
                 the top_p to be used to generate the answer
                 defaults to None
             n : int (optional)
                 the number of answers to be generated
                 defaults to 1
             function_call : str (optional)
                 the function call to be used, defaults to "auto"
+            max_retries : int
+                the maximum number of retries to be used when calling OpenAI in case of error
+                defaults to 15
+            delay : int
+                the delay in seconds to be used between retries
+                defaults to 10
 
         Returns
         -------
             JAImsResponse
                 the response object
         """
 
-        self.__history_manager.add_messages(messages)
+        self.__history_manager.add_messages(messages or [])
 
         kwargs = {
-            "model": self.model.string,
+            "model": self.model,
             "temperature": temperature,
             "top_p": top_p,
             "stream": stream,
             "max_tokens": max_tokens,
             "n": n,
+            "max_retries": max_retries,
+            "delay": delay,
         }
 
         if self.functions:
             kwargs["function_call"] = function_call
             kwargs["functions"] = parse_functions_to_json(self.functions)
 
         call_context = OpenaiCallContext(kwargs)
@@ -182,27 +197,20 @@
 
         messages = self.__history_manager.get_messages(
             agent_max_tokens=call_context.call_kwargs["max_tokens"],
         )
 
         call_context.call_kwargs["messages"] = messages
 
-        try:
-            response: Any = openai.ChatCompletion.create(**call_context.call_kwargs)
+        response = get_openai_response(**call_context.call_kwargs)
 
-            if call_context.call_kwargs["stream"]:
-                return self.__process_openai_stream_response(response, call_context)
-            else:
-                return self.__process_openai_response(response, call_context)
-        except openai.OpenAIError as e:
-            raise JAImsOpenAIErrorException(
-                f"Failed to communicate with the OpenAI API: {str(e)}", e
-            ) from e
-        except Exception as e:
-            raise Exception(f"An unexpected error occurred: {str(e)}") from e
+        if call_context.call_kwargs["stream"]:
+            return self.__process_openai_stream_response(response, call_context)
+        else:
+            return self.__process_openai_response(response, call_context)
 
     def __process_openai_stream_response(
         self, response: Any, call_context: OpenaiCallContext
     ) -> Generator[str, None, None]:
         message = {}
         for response_delta in response:
             if len(response_delta["choices"]) > 0:
@@ -218,15 +226,15 @@
                     prompt_tokens = estimate_token_count(
                         json.dumps(sent_messages), model=self.model
                     )
                     completion_tokens = estimate_token_count(
                         json.dumps(message), model=self.model
                     )
                     total_tokens = prompt_tokens + completion_tokens
-                    rough_expense = JaimsTokensExpense(
+                    rough_expense = JAImsTokensExpense(
                         gpt_model=self.model,
                         prompt_tokens=prompt_tokens,
                         completion_tokens=completion_tokens,
                         total_tokens=total_tokens,
                         rough_estimate=True,
                     )
                     self.__log_new_expense(rough_expense)
@@ -237,48 +245,57 @@
                     yield response_delta["choices"][0]["delta"]["content"]
 
     def __process_openai_response(self, response: Any, call_context: OpenaiCallContext):
         if len(response["choices"]) == 0:
             return ""
 
         # log token expense
-        expense = JaimsTokensExpense.from_openai_usage_dictionary(
+        expense = JAImsTokensExpense.from_openai_usage_dictionary(
             self.model, response["usage"]
         )
         self.__log_new_expense(expense)
 
         message = response["choices"][0]["message"]
         return self.__handle_response_message(message, call_context)
 
     def __handle_response_message(self, message, call_context):
         self.__history_manager.add_messages([message])
+        logger = logging.getLogger(__name__)
+        logger.debug(f"OpenAI response:\n{message}")
 
         if "function_call" in message:
             result_message = self.__function_handler.handle_from_message(
                 message=message
             )
-            self.__history_manager.add_messages([result_message])
-            return self.__call_openai(call_context)
+            if call_context.call_kwargs["function_call"] == "auto":
+                self.__history_manager.add_messages([result_message])
+                return self.__call_openai(call_context)
 
         if call_context.call_kwargs["stream"]:
             return ""
 
         return message["content"]
 
-    def __log_new_expense(self, expense: JaimsTokensExpense):
+    def __log_new_expense(self, expense: JAImsTokensExpense):
         self.__expense[expense.gpt_model.string].add_from(expense)
 
     def get_expenses(self):
         """
         Returns the tokens spent in the current session in an array, one for each model.
         """
         return [
             expense for expense in self.__expense.values() if expense.total_tokens > 0
         ]
 
+    def get_history(self, optimized: bool = False):
+        """
+        Returns the current history of the agent.
+        """
+        return self.__history_manager.get_history(optimized=optimized)
+
     @staticmethod
     def __merge_message_deltas(current: dict, delta: dict) -> dict:
         """Merges new delta into the accumulated one."""
         for key, value in delta.items():
             if key in current:
                 if isinstance(value, str):
                     current[key] += value
```

### Comparing `jaims-py-0.0.2/jaims/exceptions.py` & `jaims-py-0.0.3/jaims/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaims-py-0.0.2/jaims/function_handler.py` & `jaims-py-0.0.3/jaims/function_handler.py`

 * *Files identical despite different names*

### Comparing `jaims-py-0.0.2/jaims/histroy_manager.py` & `jaims-py-0.0.3/jaims/histroy_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from jaims.openai_wrappers import (
     DEFAULT_MAX_TOKENS,
     JAImsGPTModel,
     estimate_token_count,
 )
 
 from jaims.exceptions import JAImsTokensLimitExceeded
-import tiktoken
 import json
 
 from jaims.function_handler import JAImsFuncWrapper, parse_functions_to_json
 
 
 class HistoryManager:
     """
@@ -41,24 +40,25 @@
         __history : list
             holds the current openai messages history. It's meant to be
             manipulated only by the methods of this class.
     """
 
     def __init__(
         self,
-        history: List = [],
+        history: Optional[List] = None,
         model: JAImsGPTModel = JAImsGPTModel.GPT_3_5_TURBO,
         mandatory_context: Optional[List] = None,
         functions: Optional[List[JAImsFuncWrapper]] = None,
         optimize_history: bool = True,
     ):
-        self.__history = history
+        self.__history = history or []
         self.model = model
         self.mandatory_context = mandatory_context or []
-        self.json_functions = parse_functions_to_json(functions or [])
+        funcs_to_parse = functions or []
+        self.json_functions = parse_functions_to_json(funcs_to_parse)
         self.optimize_history = optimize_history
 
     def add_messages(self, messages: List):
         """
         Pushes new messages in the history.
 
         Parameters
@@ -193,10 +193,16 @@
 
     def clear_history(self):
         """
         Clears the history.
         """
         self.__history = []
 
+    def get_history(self, optimized=False):
+        if optimized:
+            return self.get_messages()
+
+        return self.__history
+
     def __tokens_from_messages(self, messages: List):
         """Returns the number of tokens used by a list of messages."""
         return estimate_token_count(json.dumps(messages), self.model)
```

### Comparing `jaims-py-0.0.2/jaims_py.egg-info/PKG-INFO` & `jaims-py-0.0.3/jaims_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+<p align="center">
+    <img width="300" src="https://github.com/dev-mush/jaims-py/assets/669003/5c53381f-25b5-4141-bcd2-7457863eafb9" >
+</p>
 
-![jaims_logo](https://github.com/dev-mush/jaims/assets/669003/ac429608-6c49-4e41-a361-50da9569bfec)
 
 # jAIms 
 
 _My name is Bot, jAIMs Bot._ 🕶️
 
 jAIms is a lightweight Python framework built on top of the OpenAI library that lets you create powerful LLM agents.
 It is designed with simplicity and ease of use in mind and only depends on `openai` and `tiktoken`.
```

### Comparing `jaims-py-0.0.2/setup.py` & `jaims-py-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements.txt
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

