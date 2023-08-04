# Comparing `tmp/log10_io-0.2.7.tar.gz` & `tmp/log10_io-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.2.7.tar", max compression
+gzip compressed data, was "log10_io-0.2.8.tar", max compression
```

## Comparing `log10_io-0.2.7.tar` & `log10_io-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-08-01 01:39:16.080544 log10_io-0.2.7/LICENSE
--rw-r--r--   0        0        0     2715 2023-08-01 01:39:16.080544 log10_io-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/__init__.py
--rw-r--r--   0        0        0     9271 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/agents/camel.py
--rw-r--r--   0        0        0      765 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     4755 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/anthropic.py
--rw-r--r--   0        0        0     2594 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/bigquery.py
--rw-r--r--   0        0        0     2684 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/evals.py
--rw-r--r--   0        0        0     9316 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/langchain.py
--rw-r--r--   0        0        0     7142 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/llm.py
--rw-r--r--   0        0        0    13442 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/load.py
--rw-r--r--   0        0        0     1909 2023-08-01 01:39:16.084544 log10_io-0.2.7/log10/openai.py
--rw-r--r--   0        0        0     1020 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2101 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/tools.py
--rw-r--r--   0        0        0     1051 2023-08-01 01:39:16.088544 log10_io-0.2.7/log10/utils.py
--rw-r--r--   0        0        0      965 2023-08-01 01:39:16.088544 log10_io-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 log10_io-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-04 15:28:53.566749 log10_io-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3772 2023-08-04 15:28:53.566749 log10_io-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/__init__.py
+-rw-r--r--   0        0        0     9271 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/agents/camel.py
+-rw-r--r--   0        0        0      765 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     4755 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/anthropic.py
+-rw-r--r--   0        0        0     2594 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/bigquery.py
+-rw-r--r--   0        0        0     2684 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/evals.py
+-rw-r--r--   0        0        0     9493 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/langchain.py
+-rw-r--r--   0        0        0     7562 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/llm.py
+-rw-r--r--   0        0        0    13442 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/load.py
+-rw-r--r--   0        0        0     1909 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/openai.py
+-rw-r--r--   0        0        0     1020 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2101 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/tools.py
+-rw-r--r--   0        0        0     1051 2023-08-04 15:28:53.570749 log10_io-0.2.8/log10/utils.py
+-rw-r--r--   0        0        0      965 2023-08-04 15:28:53.570749 log10_io-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 log10_io-0.2.8/PKG-INFO
```

### Comparing `log10_io-0.2.7/LICENSE` & `log10_io-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/README.md` & `log10_io-0.2.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,50 @@
 
 Prompt chains such as those in [Langchain](https://github.com/hwchase17/langchain) can be difficult to debug. Log10 provides prompt provenance, session tracking and call stack functionality to help debug chains.
 
 **📝📊 Logging**
 
 Log all your OpenAI calls to compare and find the best prompts, store feedback, collect latency and usage metrics, and perform analytics and compliance monitoring of LLM powered features.
 
+You can log any openai (as [shown above](#🤔-what-is-this)) or anthropic based application using the library wrappers from log10:
+
+```python
+import os
+from log10.load import log10
+import anthropic
+import os
+
+log10(anthropic)
+anthropicClient = anthropic.Client()
+# anthropic calls are now logged
+```
+
+This will log any LLM call through the process execution.
+
+If you want to log other LLMs, you can use LangChain's LLM abstraction with the log10 logger:
+
+```python
+from langchain.chat_models import ChatOpenAI
+from langchain.schema import HumanMessage
+
+from log10.langchain import Log10Callback
+from log10.llm import Log10Config
+
+log10_callback = Log10Callback(log10_config=Log10Config())
+
+messages = [
+    HumanMessage(content="You are a ping pong machine"),
+    HumanMessage(content="Ping?"),
+]
+
+llm = ChatOpenAI(model_name="gpt-3.5-turbo", callbacks=[log10_callback])
+```
+
+Read more here for options for logging using library wrapper, langchain callback logger and how to apply log10 tags [here](./logging.md).
+
 **💿🧩 Flexible data store**
 
 log10 provides a managed data store, but if you'd prefer to manage data in your own environment, you can use data stores like google big query.
 
 Install the big query client library with:
 
 `pip install log10-io[bigquery]`
@@ -65,11 +101,12 @@
 
 1. Create a free account at [log10.io](https://log10.io)
 2. Set the following environment variables:
 - `LOG10_URL=https://log10.io`
 - `LOG10_TOKEN`: From the Settings tab in log10.io
 - `LOG10_ORG_ID`: From the Organization tab in log10.io
 - `OPENAI_API_KEY`: OpenAI API key
+- `ANTHROPIC_API_KEY`: Anthropic API key
 
 ## 💬 Community
 
 We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
```

### Comparing `log10_io-0.2.7/log10/agents/camel.py` & `log10_io-0.2.8/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/agents/scrape_summarizer.py` & `log10_io-0.2.8/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/anthropic.py` & `log10_io-0.2.8/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/bigquery.py` & `log10_io-0.2.8/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/evals.py` & `log10_io-0.2.8/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/langchain.py` & `log10_io-0.2.8/log10/langchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentAction, AgentFinish, LLMResult
 from log10.llm import LLM, Kind, Message
 
 import logging
+logging.basicConfig()
+logger = logging.getLogger("log10")
 
 def kwargs_to_hparams(kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Convert kwargs to hparams."""
     hparams = {}
     if "temperature" in kwargs:
         hparams["temperature"] = kwargs["temperature"]
     if "top_p" in kwargs:
@@ -37,26 +39,31 @@
     """Callback Handler that prints to std out."""
 
     def __init__(self, log10_config: Optional[dict] = None) -> None:
         """Initialize callback handler."""
         super().__init__(log10_config=log10_config, hparams=None)
         self.runs = {}
 
+        if log10_config.DEBUG:
+            logger.setLevel(logging.DEBUG)
+        else:
+            logger.setLevel(logging.INFO)
+
     def on_llm_start(
         self,
         serialized: Dict[str, Any],
         prompts: List[str],
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
         """Print out the prompts."""
-        logging.debug(
+        logger.debug(
             f"**\n**on_llm_start**\n**\n: serialized:\n {serialized} \n\n prompts:\n {prompts} \n\n rest: {kwargs}"
         )
         kwargs = serialized.get("kwargs", {})
         hparams = kwargs_to_hparams(kwargs)
 
         model = kwargs.get("model_name", None)
         if model is None:
@@ -65,15 +72,15 @@
             raise BaseException("No model found in serialized or kwargs")
 
         if len(prompts) != 1:
             raise BaseException("Only support one prompt at a time")
 
         request = {"model": model, "prompt": prompts[0], **hparams}
 
-        logging.debug(f"request: {request}")
+        logger.debug(f"request: {request}")
 
         completion_id = self.log_start(request, Kind.text, tags)
 
         self.runs[run_id] = {
             "kind": Kind.text,
             "completion_id": completion_id,
             "start_time": time.perf_counter(),
@@ -86,15 +93,15 @@
         messages: List[List[BaseMessage]],
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
-        logging.debug(
+        logger.debug(
             f"**\n**on_chat_model_start**\n**\n: run_id:{run_id}\nserialized:\n{serialized}\n\nmessages:\n{messages}\n\nkwargs: {kwargs}"
         )
 
         #
         # Find model string
         #
         kwargs = serialized.get("kwargs", {})
@@ -103,23 +110,23 @@
             model = kwargs.get("model", None)
         if model is None:
             raise BaseException("No model found in serialized or kwargs")
 
         hparams = kwargs_to_hparams(kwargs)
         hparams["model"] = model
 
-        logging.debug(f"hparams: {hparams}")
+        logger.debug(f"hparams: {hparams}")
 
         if len(messages) != 1:
             raise BaseException("Only support one message at a time")
 
         # Convert messages to log10 format
         log10_messages = []
         for message in messages[0]:
-            logging.debug(f"message: {message}")
+            logger.debug(f"message: {message}")
             if isinstance(message, HumanMessage):
                 log10_messages.append(Message(role="user", content=message.content))
             elif isinstance(message, AIMessage):
                 log10_messages.append(
                     Message(role="assistant", content=message.content)
                 )
             elif isinstance(message, SystemMessage):
@@ -127,30 +134,30 @@
             else:
                 raise BaseException(f"Unknown message type {type(message)}")
 
         request = {
             "messages": [message.to_dict() for message in log10_messages],
             **hparams,
         }
-        logging.debug(f"request: {request}")
+        logger.debug(f"request: {request}")
 
         completion_id = self.log_start(
             request,
             Kind.chat,
             tags,
         )
 
         self.runs[run_id] = {
             "kind": Kind.chat,
             "completion_id": completion_id,
             "start_time": time.perf_counter(),
             "model": model,
         }
 
-        logging.debug(f"logged start with completion_id: {completion_id}")
+        logger.debug(f"logged start with completion_id: {completion_id}")
 
     def on_llm_end(
         self,
         response: LLMResult,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
@@ -201,35 +208,35 @@
                         "logprobs": None,
                         "finish_reason": "stop",
                     }
                 ],
             }
 
         # Determine if we can provide usage metrics (token count).
-        logging.debug(f"**** response: {response}")
+        logger.debug(f"**** response: {response}")
         if response.llm_output is not None:
             token_usage = response.llm_output.get("token_usage")
             if token_usage is not None:
                 log10response["usage"] = token_usage
-                logging.debug(f"usage: {log10response['usage']}")
+                logger.debug(f"usage: {log10response['usage']}")
 
-        logging.debug(
+        logger.debug(
             f"**\n**on_llm_end**\n**\n: response:\n {log10response} \n\n rest: {kwargs}"
         )
         self.log_end(run["completion_id"], log10response, duration)
 
     def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Do nothing."""
-        logging.debug(f"token:\n {token} \n\n rest: {kwargs}")
+        logger.debug(f"token:\n {token} \n\n rest: {kwargs}")
 
     def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         """Do nothing."""
-        logging.debug(f"error:\n {error} \n\n rest: {kwargs}")
+        logger.debug(f"error:\n {error} \n\n rest: {kwargs}")
 
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> None:
         """Print out that we are entering a chain."""
         pass
```

### Comparing `log10_io-0.2.7/log10/llm.py` & `log10_io-0.2.8/log10/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 class Log10Config:
     def __init__(
         self,
         url: str = None,
         token: str = None,
         org_id: str = None,
         tags: List[str] = None,
+        DEBUG: bool = False,
     ):
         self.url = url if url else os.getenv("LOG10_URL")
         self.token = token if token else os.getenv("LOG10_TOKEN")
         self.org_id = org_id if org_id else os.getenv("LOG10_ORG_ID")
+        self.DEBUG = DEBUG
 
         # Get tags from env, if not set, use empty list
         if tags:
             self.tags = tags
         elif os.getenv("LOG10_TAGS") is not None:
             self.tags = os.getenv("LOG10_TAGS").split(",")
         else:
@@ -96,14 +98,16 @@
         self.completion_id = completion_id
 
     def text(self) -> str:
         return self._text
 
 
 class LLM(ABC):
+    last_completion_response = None
+
     def __init__(self, hparams: dict = None, log10_config: Log10Config = None):
         self.log10_config = log10_config
         self.hparams = hparams
 
         # Start session
         if self.log10_config:
             session_url = self.log10_config.url + "/api/sessions"
@@ -121,14 +125,20 @@
                 self.session_id = response["sessionID"]
             except Exception as e:
                 logging.warning(
                     f"Failed to start session with {session_url} using token {self.log10_config.token}. Won't be able to log. {e}"
                 )
                 self.log10_config = None
 
+    def last_completion_url(self):
+        if self.last_completion_response is None:
+            return None
+
+        return self.log10_config.url + '/app/' + self.last_completion_response['organizationSlug'] + '/completions/' + self.last_completion_response['completionID']
+
     def text(self, prompt: str, hparams: dict = None) -> TextCompletion:
         raise Exception("Not implemented")
 
     def text_request(self, prompt: str, hparams: dict = None) -> dict:
         raise Exception("Not implemented")
 
     def chat(self, messages: List[Message], hparams: dict = None) -> ChatCompletion:
@@ -152,14 +162,15 @@
     def log_start(self, request, kind: Kind, tags: Optional[List[str]] = None):
         if not self.log10_config:
             return None
 
         res = self.api_request(
             "/api/completions", "POST", {"organization_id": self.log10_config.org_id}
         )
+        self.last_completion_response = res.json()
         completion_id = res.json()["completionID"]
 
         # merge tags
         if tags:
             tags = list(set(tags + self.log10_config.tags))
         else:
             tags = self.log10_config.tags
```

### Comparing `log10_io-0.2.7/log10/load.py` & `log10_io-0.2.8/log10/load.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/openai.py` & `log10_io-0.2.8/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/schemas/bigquery.json` & `log10_io-0.2.8/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/tools.py` & `log10_io-0.2.8/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/log10/utils.py` & `log10_io-0.2.8/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.7/pyproject.toml` & `log10_io-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.2.7"
+version = "0.2.8"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.2.7/PKG-INFO` & `log10_io-0.2.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.2.7
+Version: 0.2.8
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -57,14 +57,50 @@
 
 Prompt chains such as those in [Langchain](https://github.com/hwchase17/langchain) can be difficult to debug. Log10 provides prompt provenance, session tracking and call stack functionality to help debug chains.
 
 **📝📊 Logging**
 
 Log all your OpenAI calls to compare and find the best prompts, store feedback, collect latency and usage metrics, and perform analytics and compliance monitoring of LLM powered features.
 
+You can log any openai (as [shown above](#🤔-what-is-this)) or anthropic based application using the library wrappers from log10:
+
+```python
+import os
+from log10.load import log10
+import anthropic
+import os
+
+log10(anthropic)
+anthropicClient = anthropic.Client()
+# anthropic calls are now logged
+```
+
+This will log any LLM call through the process execution.
+
+If you want to log other LLMs, you can use LangChain's LLM abstraction with the log10 logger:
+
+```python
+from langchain.chat_models import ChatOpenAI
+from langchain.schema import HumanMessage
+
+from log10.langchain import Log10Callback
+from log10.llm import Log10Config
+
+log10_callback = Log10Callback(log10_config=Log10Config())
+
+messages = [
+    HumanMessage(content="You are a ping pong machine"),
+    HumanMessage(content="Ping?"),
+]
+
+llm = ChatOpenAI(model_name="gpt-3.5-turbo", callbacks=[log10_callback])
+```
+
+Read more here for options for logging using library wrapper, langchain callback logger and how to apply log10 tags [here](./logging.md).
+
 **💿🧩 Flexible data store**
 
 log10 provides a managed data store, but if you'd prefer to manage data in your own environment, you can use data stores like google big query.
 
 Install the big query client library with:
 
 `pip install log10-io[bigquery]`
@@ -92,12 +128,13 @@
 
 1. Create a free account at [log10.io](https://log10.io)
 2. Set the following environment variables:
 - `LOG10_URL=https://log10.io`
 - `LOG10_TOKEN`: From the Settings tab in log10.io
 - `LOG10_ORG_ID`: From the Organization tab in log10.io
 - `OPENAI_API_KEY`: OpenAI API key
+- `ANTHROPIC_API_KEY`: Anthropic API key
 
 ## 💬 Community
 
 We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
```

