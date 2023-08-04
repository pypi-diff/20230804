# Comparing `tmp/kani-0.0.2.tar.gz` & `tmp/kani-0.0.3.tar.gz`

## Comparing `kani-0.0.2.tar` & `kani-0.0.3.tar`

### file list

```diff
@@ -1,61 +1,75 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kani-0.0.2/.gitattributes
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 kani-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 kani-0.0.2/requirements.txt
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 kani-0.0.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 kani-0.0.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 kani-0.0.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kani-0.0.2/docs/Makefile
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 kani-0.0.2/docs/advanced.rst
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kani-0.0.2/docs/api_reference.rst
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 kani-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 kani-0.0.2/docs/customization.rst
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 kani-0.0.2/docs/engine_reference.rst
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 kani-0.0.2/docs/engines.rst
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 kani-0.0.2/docs/function_calling.rst
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 kani-0.0.2/docs/index.rst
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 kani-0.0.2/docs/install.rst
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 kani-0.0.2/docs/kani.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 kani-0.0.2/docs/make.bat
--rw-r--r--   0        0        0   153203 2020-02-02 00:00:00.000000 kani-0.0.2/docs/_static/5_advanced_api.png
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 kani-0.0.2/docs/shared/engine_table.rst
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 kani-0.0.2/examples/1_quickstart.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kani-0.0.2/examples/2_function_calling_weather.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 kani-0.0.2/examples/3_customization_exception_prompt.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 kani-0.0.2/examples/3_customization_last_four.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 kani-0.0.2/examples/3_customization_track_function_calls.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 kani-0.0.2/examples/4_engines_llama.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kani-0.0.2/examples/4_engines_vicuna.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 kani-0.0.2/examples/5_advanced_api.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 kani-0.0.2/examples/5_advanced_retrieval.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 kani-0.0.2/examples/5_advanced_subkanis.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kani-0.0.2/examples/README.md
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 kani-0.0.2/examples/colab_quickstart.ipynb
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 kani-0.0.2/examples/dice.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kani-0.0.2/kani/__init__.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 kani-0.0.2/kani/ai_function.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 kani-0.0.2/kani/exceptions.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 kani-0.0.2/kani/json_schema.py
--rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 kani-0.0.2/kani/kani.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 kani-0.0.2/kani/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/__init__.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/base.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/httpclient.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/huggingface/__init__.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/huggingface/base.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/huggingface/llama2.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/huggingface/vicuna.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/openai/__init__.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/openai/client.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/openai/engine.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 kani-0.0.2/kani/engines/openai/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.2/kani/utils/__init__.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 kani-0.0.2/kani/utils/cli.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 kani-0.0.2/kani/utils/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kani-0.0.2/tests/test_type_spec.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 kani-0.0.2/tests/utils.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 kani-0.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 kani-0.0.2/LICENSE
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 kani-0.0.2/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 kani-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 kani-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kani-0.0.3/.gitattributes
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 kani-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kani-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kani-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 kani-0.0.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 kani-0.0.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 kani-0.0.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kani-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 kani-0.0.3/docs/advanced.rst
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 kani-0.0.3/docs/api_reference.rst
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 kani-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 kani-0.0.3/docs/contributing.rst
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 kani-0.0.3/docs/customization.rst
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kani-0.0.3/docs/engine_reference.rst
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 kani-0.0.3/docs/engines.rst
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 kani-0.0.3/docs/function_calling.rst
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kani-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 kani-0.0.3/docs/install.rst
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 kani-0.0.3/docs/kani.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 kani-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0   153203 2020-02-02 00:00:00.000000 kani-0.0.3/docs/_static/5_advanced_api.png
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 kani-0.0.3/docs/shared/engine_table.rst
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 kani-0.0.3/examples/1_async_entrypoints.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 kani-0.0.3/examples/1_fewshot.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 kani-0.0.3/examples/1_quickstart.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 kani-0.0.3/examples/2_function_calling_fewshot.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kani-0.0.3/examples/2_function_calling_weather.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 kani-0.0.3/examples/3_customization_exception_prompt.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 kani-0.0.3/examples/3_customization_last_four.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 kani-0.0.3/examples/3_customization_track_function_calls.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 kani-0.0.3/examples/4_engines_fp4_quant.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 kani-0.0.3/examples/4_engines_llama2.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kani-0.0.3/examples/4_engines_vicuna.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 kani-0.0.3/examples/5_advanced_api.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 kani-0.0.3/examples/5_advanced_retrieval.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 kani-0.0.3/examples/5_advanced_subkanis.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kani-0.0.3/examples/README.md
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 kani-0.0.3/examples/colab_quickstart.ipynb
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 kani-0.0.3/examples/dice.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 kani-0.0.3/kani/__init__.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 kani-0.0.3/kani/ai_function.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 kani-0.0.3/kani/exceptions.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 kani-0.0.3/kani/json_schema.py
+-rw-r--r--   0        0        0    19979 2020-02-02 00:00:00.000000 kani-0.0.3/kani/kani.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 kani-0.0.3/kani/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/__init__.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/base.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/httpclient.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/llama2_prompt.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/ctransformers/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/ctransformers/base.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/ctransformers/llama2.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/huggingface/__init__.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/huggingface/base.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/huggingface/llama2.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/huggingface/vicuna.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/openai/__init__.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/openai/client.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/openai/engine.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 kani-0.0.3/kani/engines/openai/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.3/kani/utils/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 kani-0.0.3/kani/utils/cli.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 kani-0.0.3/kani/utils/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kani-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 kani-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 kani-0.0.3/tests/engine.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 kani-0.0.3/tests/test_kani.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 kani-0.0.3/tests/test_llama.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kani-0.0.3/tests/test_type_spec.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 kani-0.0.3/tests/utils.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 kani-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 kani-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 kani-0.0.3/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 kani-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 kani-0.0.3/PKG-INFO
```

### Comparing `kani-0.0.2/.readthedocs.yaml` & `kani-0.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/docs/Makefile` & `kani-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/docs/advanced.rst` & `kani-0.0.3/docs/advanced.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 When used in conjunction with :doc:`function_calling`, kani can choose when to spawn "sub-kani" - self-contained
 "agents" capable of performing their own tasks, then reporting to the parent with their results.
 
 For example, you might have the parent kani use a cheaper, faster model - but with the tradeoff that that model has a
 smaller context length. If you need it to perform a task that requires more context, you can spawn a sub-kani using
 a more expensive, slower model with a larger context.
 
+.. caution::
+    Be careful when creating a new kani instance with an existing kani's chat history!
+    If you pass an old kani's chat history to a new kani without copying it, the same list will be mutated.
+
+    Use ``newkani = Kani(..., chat_history=oldkani.chat_history.copy())`` to pass a copy.
+
+    Index slicing (as shown in the example below) also creates a copy.
+
 .. code-block:: python
 
     class KaniWithAISummarization(Kani):
         @ai_function()
         async def summarize_conversation(self):
             """Get the summary of the conversation so far."""
             # in this AI Function, we can spawn a sub-kani with a model that can handle
@@ -117,14 +125,16 @@
     AI: The Yamanote Line is a loop service in Tokyo, Japan...
 
 .. caution::
 
     Wikipedia articles might be longer than can fit in the model's context window. Try combining this with the sub-kani
     summarization example above to build a powerful retrieval agent!
 
+    You may also use ``@ai_function(auto_truncate=...)`` if truncating the response is acceptable.
+
 Hosting kani Online
 -------------------
 What if you want to host a web service that allows its users to chat with kani? In this example, we show how you can
 allow users to connect to a kani hosted on a webserver using a WebSocket connection. Since kani supports asyncio and
 is built with parallelization in mind, you can have as many people as you want connect at once!
 
 We'll use `FastAPI <https://fastapi.tiangolo.com/>`_ to run this webserver. To connect to it, you can use any client
@@ -166,8 +176,8 @@
 
 .. image:: _static/5_advanced_api.png
     :align: center
     :width: 600
 
 .. tip::
 
-    In a real production environment, you might want to send JSON payloads over the WebSocket rather than raw strings.
+    In a real production environment, you might want to send JSON payloads over the WebSocket rather than raw strings.
```

### Comparing `kani-0.0.2/docs/api_reference.rst` & `kani-0.0.3/docs/api_reference.rst`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 Common Models
 -------------
 .. autoclass:: kani.models.ChatRole
     :members:
 
 .. autoclass:: kani.models.FunctionCall
     :members:
+    :exclude-members: model_config, model_fields
     :class-doc-from: class
 
 .. autoclass:: kani.models.ChatMessage
     :members:
+    :exclude-members: model_config, model_fields
     :class-doc-from: class
 
 Exceptions
 ----------
 .. automodule:: kani.exceptions
     :members:
```

### Comparing `kani-0.0.2/docs/conf.py` & `kani-0.0.3/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,7 +64,11 @@
     "enable": False,  # the bundled Roboto font does not support kanji
 }
 
 # sphinx_copybutton
 copybutton_exclude = ".linenos, .gp, .go"
 copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
 copybutton_prompt_is_regexp = True
+copybutton_copy_empty_lines = False
+
+# sphinxemoji.sphinxemoji
+sphinxemoji_style = "twemoji"
```

### Comparing `kani-0.0.2/docs/customization.rst` & `kani-0.0.3/docs/customization.rst`

 * *Files 5% similar despite different names*

```diff
@@ -26,37 +26,34 @@
     area of research!
 
 By default, kani includes the **system prompt** and any messages specified as **always include** (in the initializer),
 then as many messages as possible fit in the remaining token limit, prioritizing later messages.
 
 .. todo: figure demonstrating this
 
-To override this behaviour, override :meth:`.Kani.get_truncated_chat_history` in your subclass:
+To override this behaviour, override :meth:`.Kani.get_prompt` in your subclass:
 
-.. automethod:: kani.Kani.get_truncated_chat_history
+.. automethod:: kani.Kani.get_prompt
     :noindex:
 
 For example, here's how you might override the behaviour to only include the most recent 4 messages
 (omitting earlier ones to fit in the token length if necessary) and any always included messages:
 
 .. seealso::
 
     This example is available in the
     `GitHub repo <https://github.com/zhudotexe/kani/blob/main/examples/3_customization_last_four.py>`__.
 
 .. code-block:: python
 
     class LastFourKani(Kani):
-        async def get_truncated_chat_history(self):
-            # self.always_include_messages includes the system prompt
-            always_len = sum(self.message_token_len(m) for m in self.always_include_messages)
-            # the engine may need to reserve some tokens for internal mechanisms
-            always_len += self.engine.token_reserve
-            # calculate how many tokens we have remaining, accounting for the response
-            remaining = self.max_context_size - (always_len + self.desired_response_tokens)
+        async def get_prompt(self):
+            # calculate how many tokens we have for the prompt, accounting for the system prompt,
+            # always_include_messages, any tokens reserved by the engine, and the response
+            remaining = self.max_context_size - self.always_len
             # working backwards through history...
             messages = []
             for message in reversed(self.chat_history[-4:]):
                 # if the message fits in the space we have remaining...
                 message_len = self.message_token_len(message)
                 remaining -= message_len
                 if remaining > 0:
@@ -86,15 +83,15 @@
     privacy and confidentiality.
 
 .. _do_function_call:
 
 Handle a Function Call
 ----------------------
 
-.. note:: This functionality is only available when using :meth:`.Kani.full_round` and :doc:`function_calling`.
+.. note:: This functionality is only available when using :meth:`.Kani.full_round`.
 
 When a model predicts that it should use a function, it will request a :class:`.FunctionCall`. It is then kani's
 responsibility to turn the requested function call into a real call to a Python method.
 
 By default, you probably won't want to change the implementation of :meth:`.Kani.do_function_call`, which does a couple
 things:
 
@@ -163,24 +160,27 @@
     >>> ai.failed_calls
     Counter({'get_time': 1})
 
 .. _handle_function_call_exception:
 
 Handle a Function Call Exception
 --------------------------------
-.. note:: This functionality is only available when using :meth:`.Kani.full_round` and :doc:`function_calling`.
+.. note:: This functionality is only available when using :meth:`.Kani.full_round`.
 
 Above, we show how you can instrument a function call. But when a function call goes wrong, what happens?
 
 A requested function call can error out for a variety of reasons:
 
-- The requested function doesn't exist and the model hallucinated it
-- The function exists, but the model hallucinated parameters that don't exist
+- The requested function doesn't exist and the model hallucinated it (:exc:`.NoSuchFunction`)
+- The function exists, but the model hallucinated parameters that don't exist (:exc:`.WrappedCallException` around
+  :exc:`TypeError`)
 - The parameter names all exist, but the model got the data types wrong or didn't provide some
-- The Python function raised an exception
+  (:exc:`.WrappedCallException` around :exc:`TypeError` or
+  `ValidationError <https://docs.pydantic.dev/latest/errors/validation_errors/>`_)
+- The Python function raised an exception (:exc:`.WrappedCallException`)
 
 By default, kani will add a :class:`.ChatMessage` to the chat history, giving the model feedback
 on what occurred. The model can then retry the call up to *retry_attempts* times.
 
 :meth:`.Kani.handle_function_call_exception` controls this behaviour, adding the message and returning whether or not
 the model should be allowed to retry. By overriding this method, you can control the error prompt, log the error, or
 implement custom retry logic.
```

### Comparing `kani-0.0.2/docs/engine_reference.rst` & `kani-0.0.3/docs/engine_reference.rst`

 * *Files 17% similar despite different names*

```diff
@@ -30,7 +30,15 @@
     :members:
 
 .. autoclass:: kani.engines.huggingface.llama2.LlamaEngine
     :members:
 
 .. autoclass:: kani.engines.huggingface.vicuna.VicunaEngine
     :members:
+
+CTransformers
+-------------
+.. autoclass:: kani.engines.ctransformers.base.CTransformersEngine
+    :members:
+
+.. autoclass:: kani.engines.ctransformers.llama2.LlamaCTransformersEngine
+    :members:
```

### Comparing `kani-0.0.2/docs/function_calling.rst` & `kani-0.0.3/docs/function_calling.rst`

 * *Files 18% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         def get_weather(self, location, unit):
             # call some weather API...
 
     ai = MyKani(engine)
     chat_in_terminal(ai)
 
 .. note::
-
-    AI functions can be synchronous or asynchronous - kani will automatically await a coroutine as needed.
+    AI functions can be synchronous (i.e. ``def``) or asynchronous (``async def``) - kani will automatically await a
+    coroutine as needed.
 
 Step 2: Documentation
 ---------------------
 In order for a language model to effectively know what our AI functions do, we need to document them. We do this
 inline in the function: through type annotations and the docstring.
 
 The allowed types are:
@@ -89,14 +89,17 @@
         ):
             # add a triple-quoted string immediately after the def to describe the function:
             """Get the current weather in a given location."""
             # call some weather API...
 
     # ...
 
+.. note::
+    Comments (i.e. ``# ...``) aren't given to the language model at all - these are only for your own reference.
+
 Step 3: Register
 ----------------
 The final step once you've defined your method is to register it as an AI function using the ``@ai_function()``
 decorator.
 
 Here, you can set some options for how kani should expose your function by passing these keyword args:
 
@@ -130,16 +133,16 @@
 .. _next_actor:
 
 Next Actor
 ^^^^^^^^^^
 After a function call returns, kani will hand control back to the LM to generate a response by default. If instead
 control should be given to the human (i.e. return from the chat round), set ``after=ChatRole.USER``.
 
-Example
--------
+Complete Example
+----------------
 Here's the full example of how you might implement a function to get weather that we built in the last few steps:
 
 .. code-block:: python
 
     import enum
     from typing import Annotated
 
@@ -164,24 +167,83 @@
             # call some weather API, or just mock it for this example
             degrees = 72 if unit == Unit.FAHRENHEIT else 22
             return f"Weather in {location}: Sunny, {degrees} degrees {unit.value}."
 
     ai = MyKani(engine)
     chat_in_terminal(ai)
 
+Few-Shot Prompting
+------------------
+Just as in the last section, we can also few-shot prompt the model to give it examples of how it should call the
+functions we define.
+
+When a function returns a result, that result is converted to a string and saved to the chat history. To few-shot
+prompt a model, we can mock these returns in the chat history using :meth:`.ChatMessage.function`!
+
+For example, here's how you might prompt the model to give the temperature in both Fahrenheit and Celsius without
+the user having to ask:
+
+.. code-block:: python
+
+    from kani import ChatMessage, FunctionCall
+    fewshot = [
+        ChatMessage.user("What's the weather in Philadelphia?"),
+        # first, the model should ask for the weather in fahrenheit
+        ChatMessage.assistant(
+            content=None,
+            function_call=FunctionCall.with_args(
+                "get_weather", location="Philadelphia, PA", unit="fahrenheit"
+            )
+        ),
+        # and we mock the function's response to the model
+        ChatMessage.function(
+            "get_weather",
+            "Weather in Philadelphia, PA: Partly cloudy, 85 degrees fahrenheit.",
+        ),
+        # repeat in celsius
+        ChatMessage.assistant(
+            content=None,
+            function_call=FunctionCall.with_args(
+                "get_weather", location="Philadelphia, PA", unit="celsius"
+            )
+        ),
+        ChatMessage.function(
+            "get_weather",
+            "Weather in Philadelphia, PA: Partly cloudy, 29 degrees celsius.",
+        ),
+        # finally, give the result to the user
+        ChatMessage.assistant("It's currently 85F (29C) and partly cloudy in Philadelphia."),
+    ]
+    ai = MyKani(engine, chat_history=fewshot)
+
+.. code-block:: pycon
+
+    >>> chat_in_terminal(ai)
+    USER: What's the weather in San Francisco?
+    AI: Thinking (get_weather)...
+    AI: Thinking (get_weather)...
+    AI: It's currently 72F (22C) and sunny in San Francisco.
+
+Few-shot prompts combined with function calls are a powerful tool! For example, you can also specify how a model should
+retry functions, vary the parameters it gives, react to function feedback, and more.
+
 Dynamic Functions
 -----------------
 Rather than statically defining the list of functions a kani can use in a class, you can also pass a list of
 :class:`.AIFunction` when you initialize a kani.
 
 The API for the :class:`.AIFunction` class is similar to :func:`.ai_function`.
 
 .. code-block:: python
 
-    def my_cool_function(foo: str, bar: int):
+    def my_cool_function(
+        foo: str,
+        bar: Annotated[int, AIParam(desc="Some cool parameter.")],
+    ):
+        """Do some cool things."""
         ...
 
     functions = [AIFunction(my_cool_function)]
     ai = Kani(engine, functions=functions)
 
 .. _auto_retry:
```

### Comparing `kani-0.0.2/docs/index.rst` & `kani-0.0.3/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 
 kani (カニ) is a lightweight and highly hackable harness for chat-based language models with tool usage/function calling.
 
 Compared to other LM harnesses, kani is less opinionated and offers more fine-grained customizability
 over the parts of the control flow that matter, making it the perfect choice for NLP researchers, hobbyists, and
 developers alike.
 
+kani comes with support for OpenAI models and LLaMA v2 out of the box, with a model-agnostic framework to add support
+for many more.
+
 .. todo information about the paper and citations
 
 Features
 --------
 
 - **Lightweight and high-level** - kani implements common boilerplate to interface with language models without forcing
   you to use opinionated prompt frameworks or complex library-specific tooling.
+- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
+  Implement these two, and kani can run with any language model.
 - **Automatic chat memory management** - Allow chat sessions to flow without worrying about managing the number of
   tokens in the history - kani takes care of it.
 - **Function calling with model feedback and retry** - Give models access to functions in just one line of code.
   kani elegantly provides feedback about hallucinated parameters and errors and allows the model to retry calls.
-- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
-  Implement these two, and kani can run with any language model.
-- **You are in control** - You can override and provide a custom implementation for all
-  of these features, allowing you to run experiments just the way you want to. There are no hidden prompt hacks.
+- **You control the prompts** - There are no hidden prompt hacks. We will never decide for you how to format your own
+  data, unlike other popular language model libraries.
 - **Fast to iterate and intuitive to learn** - With kani, you only write Python - we handle the rest.
 - **Asynchronous design from the start** - kani can scale to run multiple chat sessions in parallel easily, without
   having to manage multiple processes or programs.
 
 Quickstart
 ----------
 kani requires Python 3.10 or above.
@@ -74,8 +77,9 @@
     kani
     function_calling
     customization
     engines
     advanced
     api_reference
     engine_reference
+    contributing
     genindex
```

### Comparing `kani-0.0.2/docs/install.rst` & `kani-0.0.3/docs/install.rst`

 * *Files 24% similar despite different names*

```diff
@@ -58,8 +58,43 @@
 
     .. code-block:: console
 
         $ python -m venv venv
         $ venv\Scripts\activate.bat
         $ pip install "kani[...]"
 
+Development Version
+-------------------
+If you'd like to install the development version of kani, you can install it from GitHub directly:
+
+.. code-block:: console
+
+    $ pip install 'kani @ git+https://github.com/zhudotexe/kani.git@main'
+
+This will install the latest version of kani.
+
+.. note::
+    You may need to use ``pip install --upgrade --no-deps --force-reinstall ...`` to force pip to re-fetch the
+    latest kani from GitHub.
+
+    To install an engine's extras, use ``pip install 'kani[...] @ git+https://github.com/zhudotexe/kani.git@main'``.
+
+.. caution::
+    Development versions of kani may be unstable! Do not use development kani in production or in final research
+    experiments; pin a released version of kani instead.
+
+Requirements File
+-----------------
+If you're running experiments using kani, we recommend pinning the version of kani to ensure your runs are reproducible.
+To do this, we recommend storing all your Python requirements in a ``requirements.txt`` file.
+
+.. code-block:: text
+
+    kani[...]==x.y.z
+    # ... other dependencies
+
+You can automatically generate this file too, by running ``pip freeze > requirements.txt``.
+
+Later, anyone else running your code can install the same dependency versions by simply running
+``pip install -r requirements.txt``.
+
 Next, we'll take a look at basic usage of kani.
```

### Comparing `kani-0.0.2/docs/kani.rst` & `kani-0.0.3/docs/engines.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-Basic Usage
-===========
-Let's take a look back at the quickstart program:
+Engines
+=======
+Engines are the means by which kani interact with language models. As you've seen, kani comes with a few engines
+included:
 
-.. code-block:: python
+.. include:: shared/engine_table.rst
 
-    from kani import Kani, chat_in_terminal
-    from kani.engines.openai import OpenAIEngine
+In this section, we'll discuss how to implement your own engine to use any language model or API you can think of.
 
-    api_key = "sk-..."
-    engine = OpenAIEngine(api_key, model="gpt-3.5-turbo")
-    ai = Kani(engine)
-    chat_in_terminal(ai)
+.. tip::
 
-kani is comprised of two main parts: the *engine*, which is the interface between kani and the language model,
-and the *kani*, which is responsible for tracking chat history, prompting the engine, and handling function calls.
+    Built an engine for a model kani doesn't support yet?
+    kani is OSS and |:heart:| PRs with engine implementations for the latest models - see :doc:`contributing`.
 
-Kani
-----
+Implementing an Engine
+----------------------
+To create your own engine, all you have to do is subclass :class:`.BaseEngine`:
 
-.. seealso::
+.. autoclass:: kani.engines.base.BaseEngine
+    :noindex:
+    :members:
 
-    The :class:`.Kani` API documentation.
+A new engine must implement at least the two abstract methods and set the abstract attribute:
 
-To initialize a kani, only the ``engine`` is required, though you can configure much more:
+- :meth:`.BaseEngine.message_len` takes a single :class:`.ChatMessage` and returns the length of that message,
+  in tokens.
+- :meth:`.BaseEngine.predict` takes a list of :class:`.ChatMessage` and :class:`.AIFunction` and returns a
+  new :class:`.BaseCompletion`.
+- :attr:`.BaseEngine.max_context_size` specifies the model's token context size.
+
+Optionally, you can also implement :meth:`.BaseEngine.close` if your engine needs to clean up resources, and
+:attr:`.BaseEngine.token_reserve` if your engine needs to reserve tokens (e.g. for a one-time prompt template).
+
+kani comes with a couple additional bases and utilities to help you build engines for models on Hugging Face or with
+an available HTTP API.
+
+HTTP Client
+-----------
+If your language model backend exposes an HTTP API, you can create a subclass of :class:`.BaseClient` to interface with
+it. Your engine should then create an instance of the new HTTP client and call it to make predictions.
 
-.. automethod:: kani.Kani.__init__
+.. seealso::
+
+    The source code of the :class:`.OpenAIClient`, which uses the HTTP client.
+
+.. autoclass:: kani.engines.httpclient.BaseClient
     :noindex:
+    :members:
 
-.. code-block:: pycon
+Hugging Face
+------------
+If your language model backend is available on Hugging Face or is compatible with ``transformers``'
+``AutoModelForCausalLM`` interface, kani includes a base engine that implements a prediction pipeline.
 
-    >>> from kani import Kani, chat_in_terminal
-    >>> from kani.engines.openai import OpenAIEngine
-    >>> api_key = "sk-..."
-    >>> engine = OpenAIEngine(api_key, model="gpt-3.5-turbo")
-    >>> ai = Kani(engine, system_prompt="You are a sarcastic assistant.")
-    >>> chat_in_terminal(ai, rounds=1)
-    USER: Hello kani!
-    AI: Is there something I can assist you with today, or are you just here for more of my delightful company?
-
-Entrypoints
-^^^^^^^^^^^
-While :func:`.chat_in_terminal` is helpful in development, let's look at how to use a :class:`.Kani` in a larger
-application.
+Instead of having to implement the prediction logic, all you have to do is subclass :class:`.HuggingEngine` and
+implement :meth:`~.HuggingEngine.build_prompt` and :meth:`~.BaseEngine.message_len`.
 
-The two standard entrypoints are :meth:`.Kani.chat_round` and :meth:`.Kani.full_round`, and their ``_str`` counterparts:
+.. seealso::
 
-.. automethod:: kani.Kani.chat_round
-    :noindex:
+    The source code of the :class:`.LlamaEngine`, which uses the HuggingEngine.
 
-.. automethod:: kani.Kani.full_round
+.. autoclass:: kani.engines.huggingface.base.HuggingEngine
     :noindex:
 
-These are asynchronous methods, which means you'll need to be in an async context.
-
-Web frameworks like FastAPI and Flask 2 allow your route methods to be async, meaning you can await a kani method
-from within your route method without having to get too in the weeds with asyncio.
+    .. automethod:: kani.engines.huggingface.base.HuggingEngine.build_prompt
+        :noindex:
 
-Otherwise, you can create an async context by defining an async function and using :func:`asyncio.run`. For example,
-here's how you might implement a simple chat:
+    .. automethod:: kani.engines.huggingface.base.HuggingEngine.message_len
+        :noindex:
 
-.. code-block:: python
+.. _4b_quant:
 
-    from kani import Kani, chat_in_terminal
-    from kani.engines.openai import OpenAIEngine
+4-bit Quantization (|:hugging:|)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+If you're running your model locally, you might run into issues because large language models are, well, *large*!
+Unless you pay for a massive compute cluster (|:money_with_wings:|) or have access to one at your institution, you
+might not be able to fit models with billions of params on your GPU. That's where model quantization comes into play.
 
-    api_key = "sk-..."
-    engine = OpenAIEngine(api_key, model="gpt-3.5-turbo")
-    ai = Kani(engine, system_prompt="You are a helpful assistant.")
-
-    async def chat_with_kani():
-        while True:
-            user_message = input("USER: ")
-            message = await ai.chat_round_str(user_message)
-            print("AI:", message)
+    Using FP4 quantization you can expect to reduce up to 8x the model size compared to its native full precision
+    version.
 
-    asyncio.run(chat_with_kani())
+In this section, we'll show how to load HuggingFace models in FP4.
 
 .. seealso::
 
-    The source code of :func:`.chat_in_terminal`.
+    We're mostly going to follow the HuggingFace documentation found here:
+    https://huggingface.co/docs/transformers/perf_infer_gpu_one
 
-Engines
-^^^^^^^
-Engines are responsible for interfacing with a language model.
+**Install Dependencies**
 
-This table lists the engines built in to kani:
+First, you'll need to install kani with the ``huggingface`` extra (and any other extras necessary for your engine;
+we'll use LLaMA v2 in this example, so you'll want ``pip install 'kani[huggingface,llama]'``\ .)
 
-.. include:: shared/engine_table.rst
+After that, you'll need to install ``bitsandbytes`` and ``accelerate``:
 
-.. seealso::
+.. code-block:: console
 
-    We won't go too far into implementation details here - if you are interested in implementing your own engine, check
-    out :doc:`engines` or the :class:`.BaseEngine` API documentation.
+    $ pip install bitsandbytes>=0.39.0 accelerate
 
-When you are finished with an engine, release its resources with :meth:`.BaseEngine.close`.
+.. caution:: The ``bitsandbytes`` library is currently only UNIX-compatible.
 
-Chat Messages
-^^^^^^^^^^^^^
-Each message contains the ``role`` (a :class:`.ChatRole`: system, assistant, user, or function) that sent the message
-and the ``content`` of the message. Optionally, a user message can also contain a ``name`` (for multi-user
-conversations), and an assistant message can contain a ``function_call`` (discussed in :doc:`function_calling`).
-
-At a high level, a :class:`.Kani` is responsible for managing a list of :class:`.ChatMessage`: the chat session associated
-with it. You can access the chat messages through the :attr:`.Kani.chat_history` attribute.
-
-You may even modify the chat history (i.e. append or delete ChatMessages) to change the prompt at any time.
-
-.. code-block:: pycon
-
-    >>> from kani import Kani, chat_in_terminal
-    >>> from kani.engines.openai import OpenAIEngine
-    >>> api_key = "sk-..."
-    >>> engine = OpenAIEngine(api_key, model="gpt-3.5-turbo")
-    >>> ai = Kani(engine, system_prompt="You are a helpful assistant.")
-    >>> chat_in_terminal(ai, rounds=1)
-    USER: Hello kani!
-    AI: Hello! How can I assist you today?
-    >>> ai.chat_history
-    [
-        ChatMessage(role=ChatRole.USER, content="Hello kani!"),
-        ChatMessage(role=ChatRole.ASSISTANT, content="Hello! How can I assist you today?"),
-    ]
-    >>> await ai.get_truncated_chat_history()
-    # The system prompt is passed to the engine, but isn't part of chat_history
-    # - this will be useful later in advanced use cases.
-    [
-        ChatMessage(role=ChatRole.SYSTEM, content="You are a helpful assistant."),
-        ChatMessage(role=ChatRole.USER, content="Hello kani!"),
-        ChatMessage(role=ChatRole.ASSISTANT, content="Hello! How can I assist you today?"),
-    ]
+**Set Load Arguments**
 
-Saving & Loading Chats
-----------------------
-You can save or load a kani's chat state using :meth:`.Kani.save` and :meth:`.Kani.load`. This will dump the state to
-a specified JSON file, which you can load into a later kani instance:
+Then, you'll need to set the ``model_load_kwargs`` when initializing your model, and use the engine as normal! This
+example shows the :class:`.LlamaEngine`, but the same arguments should apply to any subclass of the
+:class:`.HuggingEngine`.
 
-.. automethod:: kani.Kani.save
-    :noindex:
+.. code-block:: python
+    :emphasize-lines: 4-7
 
-.. automethod:: kani.Kani.load
-    :noindex:
+    engine = LlamaEngine(
+        use_auth_token=True,
+        strict=True,
+        model_load_kwargs={
+            "device_map": "auto",
+            "load_in_4bit": True,
+        },
+    )
+
+
+**Memory Usage Comparison**
+
+This table shows the effect of enabling fp4 quantization on GPU memory usage and inference speed on ``Llama-2-7b-chat``.
+
+These numbers represent the average of three runs on a consumer RTX 4070ti (12GB memory) with greedy sampling.
+
++--------------+----------------------+----------------------------------------+
+| fp4 Enabled? | Memory Usage         | Inference Time (per token)             |
++==============+======================+========================================+
+| No           | 26.6GB               | 1215.6 ms                              |
++--------------+----------------------+----------------------------------------+
+| Yes          | 5.0GB (5.32x less)   | 23.6 ms (51.5x speedup\ [#shared]_)    |
++--------------+----------------------+----------------------------------------+
+
+.. [#shared] Since the memory usage without fp4 enabled is larger than the VRAM size of my GPU, some weights were stored
+    in shared memory. This likely led to much slower inference compared to storing all weights on a GPU.
+
+CTransformers
+-------------
+If your language model backend is available with GGML, kani includes a base engine that implements 
+a prediction pipeline.
+
+Instead of having to implement the prediction logic, all you have to do is subclass :class:`.CTransformersEngine` and
+implement :meth:`~.CTransformersEngine.build_prompt` and :meth:`~.BaseEngine.message_len`.
 
-If you'd like more manual control over how you store chat state, there are two attributes you need to save:
-:attr:`.Kani.always_include_messages` and :attr:`.Kani.chat_history` (both lists of :class:`.ChatMessage`\ ).
+.. seealso::
+
+    The source code of the :class:`.LlamaCTransformersEngine`, which uses the CTransformersEngine.
 
-These are `pydantic <https://docs.pydantic.dev/latest/usage/serialization/>`_ models, which you can save and load using
-``ChatMessage.model_dump()`` and ``ChatMessage.model_validate()``.
+.. autoclass:: kani.engines.ctransformers.base.CTransformersEngine
+    :noindex:
 
-You could, for example, save the chat state to a database and load it when necessary. A common pattern is also to save
-only the ``chat_history`` and use ``always_include_messages`` as an application-specific prompt.
+    .. automethod:: kani.engines.ctransformers.base.CTransformersEngine.build_prompt
+        :noindex:
 
-Next Steps
-----------
-In the next section, we'll look at subclassing :class:`.Kani` in order to supply functions to the language model.
-Then, we'll look at how you can override and/or extend the implementations of kani methods to control each part of
-a chat round.
+    .. automethod:: kani.engines.ctransformers.base.CTransformersEngine.message_len
+        :noindex:
```

### Comparing `kani-0.0.2/docs/make.bat` & `kani-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/docs/_static/5_advanced_api.png` & `kani-0.0.3/docs/_static/5_advanced_api.png`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/1_quickstart.py` & `kani-0.0.3/examples/1_quickstart.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/2_function_calling_weather.py` & `kani-0.0.3/examples/2_function_calling_weather.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/3_customization_exception_prompt.py` & `kani-0.0.3/examples/3_customization_exception_prompt.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/3_customization_last_four.py` & `kani-0.0.3/examples/3_customization_last_four.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 from kani.engines.openai import OpenAIEngine
 
 api_key = os.getenv("OPENAI_API_KEY")
 engine = OpenAIEngine(api_key, model="gpt-3.5-turbo")
 
 
 class LastFourKani(Kani):
-    async def get_truncated_chat_history(self):
+    async def get_prompt(self):
         """
         Only include the most recent 4 messages (omitting earlier ones to fit in the token length if necessary)
         and any always included messages.
         """
-        # self.always_include_messages includes the system prompt
-        always_len = sum(self.message_token_len(m) for m in self.always_include_messages)
-        # the engine may need to reserve some tokens for internal mechanisms
-        always_len += self.engine.token_reserve
-        # calculate how many tokens we have remaining, accounting for the response
-        remaining = self.max_context_size - (always_len + self.desired_response_tokens)
+        # calculate how many tokens we have for the prompt, accounting for the system prompt, always_include_messages,
+        # any tokens reserved by the engine, and the response
+        remaining = self.max_context_size - self.always_len
         # working backwards through history...
         messages = []
         for message in reversed(self.chat_history[-4:]):
             # if the message fits in the space we have remaining...
             message_len = self.message_token_len(message)
             remaining -= message_len
             if remaining > 0:
```

### Comparing `kani-0.0.2/examples/3_customization_track_function_calls.py` & `kani-0.0.3/examples/3_customization_track_function_calls.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/4_engines_llama.py` & `kani-0.0.3/examples/4_engines_llama2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from kani import Kani, chat_in_terminal
 from kani.engines.huggingface.llama2 import LlamaEngine
 
 engine = LlamaEngine(use_auth_token=True, strict=True)
 ai = Kani(
     engine,
     system_prompt=(
-        "You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. "
+        "You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe."
         " Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content."
         " Please ensure that your responses are socially unbiased and positive in nature.\n\nIf a question does not"
         " make any sense, or is not factually coherent, explain why instead of answering something not correct. If you"
         " don't know the answer to a question, please don't share false information."
     ),
 )
+
 if __name__ == "__main__":
     chat_in_terminal(ai)
```

### Comparing `kani-0.0.2/examples/4_engines_vicuna.py` & `kani-0.0.3/examples/4_engines_vicuna.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/5_advanced_api.py` & `kani-0.0.3/examples/5_advanced_api.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/5_advanced_retrieval.py` & `kani-0.0.3/examples/5_advanced_retrieval.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/5_advanced_subkanis.py` & `kani-0.0.3/examples/5_advanced_subkanis.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/examples/colab_quickstart.ipynb` & `kani-0.0.3/examples/colab_quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/kani/ai_function.py` & `kani-0.0.3/kani/ai_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,32 +16,37 @@
         self,
         inner,
         after: ChatRole = ChatRole.ASSISTANT,
         name: str | None = None,
         desc: str | None = None,
         auto_retry: bool = True,
         json_schema: dict | None = None,
+        auto_truncate: int | None = None,
     ):
         """
         :param inner: The function implementation.
         :param after: Who should speak next after the function call completes (see :ref:`next_actor`). Defaults to the
             model.
         :param name: The name of the function (defaults to the name of the function in source code).
         :param desc: The function's description (defaults to the function's docstring).
         :param auto_retry: Whether the model should retry calling the function if it gets it wrong
             (see :ref:`auto_retry`).
         :param json_schema: A JSON Schema document describing the function's parameters. By default, kani will
             automatically generate one, but this can be helpful for overriding it in any tricky cases.
+        :param auto_truncate: If a function response is longer than this many tokens, truncate it until it is at most
+            this many tokens and add "..." to the end. By default, no responses will be truncated. This uses a smart
+            paragraph-aware truncation algorithm.
         """
         self.inner = validate_call(inner)
         self.after = after
         self.name = name or inner.__name__
         self.desc = desc or inspect.getdoc(inner)
         self.auto_retry = auto_retry
         self.json_schema = self.create_json_schema() if json_schema is None else json_schema
+        self.auto_truncate = auto_truncate
 
         # wraps() things
         self.__name__ = inner.__name__
         self.__qualname__ = inner.__qualname__
         self.__annotations__ = inner.__annotations__
         self.__module__ = inner.__module__
         self.__doc__ = inner.__doc__
@@ -88,33 +93,38 @@
     func=None,
     *,
     after: ChatRole = ChatRole.ASSISTANT,
     name: str | None = None,
     desc: str | None = None,
     auto_retry: bool = True,
     json_schema: dict | None = None,
+    auto_truncate: int | None = None,
 ):
     """Decorator to mark a method of a Kani to expose to the AI.
 
     :param after: Who should speak next after the function call completes (see :ref:`next_actor`). Defaults to the
         model.
     :param name: The name of the function (defaults to the name of the function in source code).
     :param desc: The function's description (defaults to the function's docstring).
     :param auto_retry: Whether the model should retry calling the function if it gets it wrong (see :ref:`auto_retry`).
     :param json_schema: A JSON Schema document describing the function's parameters. By default, kani will automatically
         generate one, but this can be helpful for overriding it in any tricky cases.
+    :param auto_truncate: If a function response is longer than this many tokens, truncate it until it is at most
+        this many tokens and add "..." to the end. By default, no responses will be truncated. This uses a smart
+        paragraph-aware truncation algorithm.
     """
 
     def deco(f):
         f.__ai_function__ = {
             "after": after,
             "name": name or f.__name__,
             "desc": desc or inspect.getdoc(f),
             "auto_retry": auto_retry,
             "json_schema": json_schema,
+            "auto_truncate": auto_truncate,
         }
         return f
 
     if func is not None:
         return deco(func)
     return deco
```

### Comparing `kani-0.0.2/kani/exceptions.py` & `kani-0.0.3/kani/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 class KaniException(Exception):
     """Base class for all Kani exceptions/errors."""
 
 
+class MessageTooLong(KaniException):
+    """This chat message will never fit in the context window."""
+
+
 # ==== HTTP ====
 class HTTPException(KaniException):
     """Base class for all HTTP errors (for HTTP engines)."""
 
 
 class HTTPTimeout(HTTPException):
     """Timeout occurred connecting to or waiting for a response from an HTTP request."""
```

### Comparing `kani-0.0.2/kani/json_schema.py` & `kani-0.0.3/kani/json_schema.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/kani/kani.py` & `kani-0.0.3/kani/kani.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 import inspect
 import logging
+import weakref
 from typing import AsyncIterable, Callable
 
-import cachetools
-
 from .ai_function import AIFunction
-from .engines.base import BaseEngine
-from .exceptions import NoSuchFunction, WrappedCallException, FunctionCallException
+from .engines.base import BaseEngine, BaseCompletion
+from .exceptions import NoSuchFunction, WrappedCallException, FunctionCallException, MessageTooLong
 from .models import ChatMessage, FunctionCall, ChatRole
 from .utils.typing import PathLike, SavedKani
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("kani")
+message_log = logging.getLogger("kani.messages")
 
 
 class Kani:
     """Base class for all kani.
 
     **Entrypoints**
 
@@ -67,90 +67,74 @@
             evict newer messages rather than these to manage context length). These will not be included in
             :attr:`chat_history`.
         :param desired_response_tokens: The minimum amount of space to leave in ``max context size - tokens in prompt``.
             To control the maximum number of tokens generated more precisely, you may be able to configure the engine
             (e.g. ``OpenAIEngine(..., max_tokens=250)``).
         :param chat_history: The chat history to start with (not including system prompt or always include messages),
             for advanced use cases. By default, each kani starts with a new conversation session.
+
+            .. caution::
+                If you pass another kani's chat history here without copying it, the same list will be mutated!
+                Use ``chat_history=mykani.chat_history.copy()`` to pass a copy.
         :param functions: A list of :class:`.AIFunction` to expose to the model (for dynamic function calling).
             Use :func:`.ai_function` to define static functions (see :doc:`function_calling`).
         :param retry_attempts: How many attempts the LM may take if a function call raises an exception.
         """
         self.engine = engine
         self.system_prompt = system_prompt.strip() if system_prompt else None
         self.desired_response_tokens = desired_response_tokens
         self.max_context_size = engine.max_context_size
 
         self.always_include_messages: list[ChatMessage] = (
             [ChatMessage.system(self.system_prompt)] if system_prompt else []
         ) + (always_include_messages or [])
-        """Chat messages that are always included as a prefix in the model's prompt. Includes the system message, if
-        supplied."""
+        """Chat messages that are always included as a prefix in the model's prompt.
+        Includes the system message, if supplied."""
 
         self.chat_history: list[ChatMessage] = chat_history or []
         """All messages in the current chat state, not including system or always include messages."""
 
         # async to prevent generating multiple responses missing context
         self.lock = asyncio.Lock()
 
         # function calling
         self.retry_attempts = retry_attempts
 
         # find all registered ai_functions and save them
         if functions is None:
             functions = []
-        self.functions = {f.name: f for f in functions}
+        self.functions: dict[str, AIFunction] = {f.name: f for f in functions}
         for name, member in inspect.getmembers(self, predicate=inspect.ismethod):
             if not hasattr(member, "__ai_function__"):
                 continue
             f: AIFunction = AIFunction(member, **member.__ai_function__)
             if f.name in self.functions:
                 raise ValueError(f"AIFunction {f.name!r} is already registered!")
             self.functions[f.name] = f
 
         # cache
-        self._oldest_idx = 0
-        self._message_tokens = cachetools.FIFOCache(256)
-
-    def message_token_len(self, message: ChatMessage):
-        """Returns the number of tokens used by a given message."""
-        try:
-            return self._message_tokens[message]
-        except KeyError:
-            mlen = self.engine.message_len(message)
-            if mlen > self.max_context_size:
-                log.warning(
-                    "The chat message's size is longer than the entire context window. It will never be included in a"
-                    f" prompt, nor any messages before it.\nContent: {message.content!r}"
-                )
-            self._message_tokens[message] = mlen
-            return mlen
+        self._message_tokens = weakref.WeakKeyDictionary()
 
     # === main entrypoints ===
     async def chat_round(self, query: str, **kwargs) -> ChatMessage:
         """Perform a single chat round (user -> model -> user, no functions allowed).
 
         This is slightly faster when you are chatting with a kani with no AI functions defined.
 
         :param query: The contents of the user's chat message.
         :param kwargs: Additional arguments to pass to the model engine (e.g. hyperparameters).
         :returns: The model's reply.
         """
         async with self.lock:
-            # get the user's chat input
+            # add the user's chat input to the state
             self.chat_history.append(ChatMessage.user(query.strip()))
 
-            # get the context
-            messages = await self.get_truncated_chat_history()
-
-            # get the model's output, save it to chat history
-            completion = await self.engine.predict(messages=messages, **kwargs)
-
+            # and get a completion
+            completion = await self.get_model_completion(include_functions=False, **kwargs)
             message = completion.message
-            self._message_tokens[message] = completion.completion_tokens or self.message_token_len(message)
             self.chat_history.append(message)
             return message
 
     async def chat_round_str(self, query: str, **kwargs) -> str:
         """Like :meth:`chat_round`, but only returns the content of the message."""
         msg = await self.chat_round(query, **kwargs)
         return msg.content
@@ -171,21 +155,16 @@
         retry = 0
         is_model_turn = True
         async with self.lock:
             self.chat_history.append(ChatMessage.user(query.strip()))
 
             while is_model_turn:
                 # do the model prediction
-                messages = await self.get_truncated_chat_history()
-                completion = await self.engine.predict(
-                    messages=messages, functions=list(self.functions.values()), **kwargs
-                )
-                # bookkeeping
+                completion = await self.get_model_completion(**kwargs)
                 message = completion.message
-                self._message_tokens[message] = completion.completion_tokens or self.message_token_len(message)
                 self.chat_history.append(message)
                 yield message
 
                 # if function call, do it and attempt retry if it's wrong
                 if not message.function_call:
                     return
 
@@ -193,15 +172,15 @@
                     is_model_turn = await self.do_function_call(message.function_call)
                 except FunctionCallException as e:
                     should_retry = await self.handle_function_call_exception(message.function_call, e, retry)
                     # retry if we have retry attempts left
                     retry += 1
                     if not should_retry:
                         # disable function calling on the next go
-                        kwargs = {**kwargs, "function_call": "none"}
+                        kwargs = {**kwargs, "include_functions": False}
                     continue
                 else:
                     retry = 0
 
     async def full_round_str(
         self,
         query: str,
@@ -218,46 +197,113 @@
         async for message in self.full_round(query, **kwargs):
             if text := message.content:
                 yield text
 
             if message.function_call and (fn_msg := function_call_formatter(message)):
                 yield fn_msg
 
+    # ==== helpers ====
+    @property
+    def always_len(self) -> int:
+        """Returns the number of tokens that will always be reserved.
+
+        (e.g. for system prompts, always include messages, the engine, and the response).
+        """
+        return (
+            sum(self.message_token_len(m) for m in self.always_include_messages)
+            + self.engine.token_reserve
+            + self.desired_response_tokens
+        )
+
+    def message_token_len(self, message: ChatMessage):
+        """Returns the number of tokens used by a given message."""
+        try:
+            return self._message_tokens[message]
+        except KeyError:
+            mlen = self.engine.message_len(message)
+            self._message_tokens[message] = mlen
+            return mlen
+
+    async def get_model_completion(self, include_functions: bool = True, **kwargs) -> BaseCompletion:
+        """Get the model's completion with the current chat state.
+
+        Compared to :meth:`chat_round` and :meth:`full_round`, this lower-level method does not save the model's reply
+        to the chat history or mutate the chat state; it is intended to help with logging or to repeat a call multiple
+        times.
+
+        :param include_functions: Whether to pass this kani's function definitions to the engine.
+        :param kwargs: Arguments to pass to the model engine.
+        """
+        # get the current chat state
+        messages = await self.get_prompt()
+        # log it (message_log includes the number of messages sent and the last message)
+        n_messages = len(messages)
+        if n_messages == 0:
+            message_log.debug("[0]>>> [requested completion with no prompt]")
+        else:
+            message_log.debug(f"[{n_messages}]>>> {messages[-1]}")
+
+        # get the model's completion at the given state
+        if include_functions:
+            completion = await self.engine.predict(messages=messages, functions=list(self.functions.values()), **kwargs)
+        else:
+            completion = await self.engine.predict(messages=messages, **kwargs)
+
+        # cache its length (if the completion isn't saved to state, this weakrefs and gc's later)
+        message = completion.message
+        self._message_tokens[message] = completion.completion_tokens or self.message_token_len(message)
+        # and log it too
+        message_log.debug(f"<<< {message}")
+        return completion
+
     # ==== overridable methods ====
-    async def get_truncated_chat_history(self) -> list[ChatMessage]:
+    async def get_prompt(self) -> list[ChatMessage]:
         """
         Called each time before asking the LM engine for a completion to generate the chat prompt.
         Returns a list of messages such that the total token count in the messages is less than
         ``(self.max_context_size - self.desired_response_tokens)``.
 
         Always includes the system prompt plus any always_include_messages at the start of the prompt.
 
         You may override this to get more fine-grained control over what is exposed in the model's memory at any given
         call.
         """
-        reversed_history = []
-        always_len = sum(self.message_token_len(m) for m in self.always_include_messages) + self.engine.token_reserve
-        remaining = self.max_context_size - (always_len + self.desired_response_tokens)
+        always_len = self.always_len
+        remaining = max_size = self.max_context_size - always_len
         total_tokens = 0
-        for idx in range(len(self.chat_history) - 1, self._oldest_idx - 1, -1):
-            message = self.chat_history[idx]
+        to_keep = 0  # messages to keep from the end of chat history
+        for message in reversed(self.chat_history):
+            # get and check the message's length
             message_len = self.message_token_len(message)
+            if message_len > max_size:
+                func_help = (
+                    ""
+                    if message.role != ChatRole.FUNCTION
+                    else "You may set `auto_truncate` in the @ai_function to automatically truncate long responses.\n"
+                )
+                raise MessageTooLong(
+                    "The chat message's size is longer than the allowed context window (after including system"
+                    " messages, always include messages, and desired response tokens).\n"
+                    f"{func_help}Content: {message.content[:100]}..."
+                )
+            # see if we can include it
             remaining -= message_len
-            if remaining > 0:
+            if remaining >= 0:
                 total_tokens += message_len
-                reversed_history.append(message)
+                to_keep += 1
             else:
-                self._oldest_idx = idx + 1
                 break
         log.debug(
-            f"get_truncated_chat_history() returned {always_len + total_tokens} tokens ({always_len} always) in"
-            f" {len(self.always_include_messages) + len(reversed_history)} messages"
+            f"get_prompt() returned {always_len + total_tokens} tokens ({always_len} always) in"
+            f" {len(self.always_include_messages) + to_keep} messages"
             f" ({len(self.always_include_messages)} always)"
         )
-        return self.always_include_messages + reversed_history[::-1]
+        if not to_keep:
+            return self.always_include_messages
+        return self.always_include_messages + self.chat_history[-to_keep:]
 
     async def do_function_call(self, call: FunctionCall) -> bool:
         """Resolve a single function call.
 
         By default, any exception raised from this method will be an instance of a :class:`.FunctionCallException`.
 
         You may implement an override to add instrumentation around function calls (e.g. tracking success counts
@@ -272,19 +318,30 @@
         f = self.functions.get(call.name)
         if not f:
             raise NoSuchFunction(call.name)
         # call it
         try:
             result = await f(**call.kwargs)
             result_str = str(result)
+            log.debug(f"{f.name} responded with data: {result_str!r}")
         except Exception as e:
             raise WrappedCallException(f.auto_retry, e) from e
+        msg = ChatMessage.function(f.name, result_str)
+        # if we are auto truncating, check and see if we need to
+        if f.auto_truncate is not None:
+            message_len = self.message_token_len(msg)
+            if message_len > f.auto_truncate:
+                log.warning(
+                    f"The content returned by {f.name} is too long ({message_len} > {f.auto_truncate} tokens), auto"
+                    " truncating..."
+                )
+                msg = self._auto_truncate_message(msg, max_len=f.auto_truncate)
+                log.debug(f"Auto truncate returned {self.message_token_len(msg)} tokens.")
         # save the result to the chat history
-        log.debug(f"{f.name} responded with data: {result_str!r}")
-        self.chat_history.append(ChatMessage.function(f.name, result_str))
+        self.chat_history.append(msg)
         # yield whose turn it is
         return f.after == ChatRole.ASSISTANT
 
     async def handle_function_call_exception(
         self, call: FunctionCall, err: FunctionCallException, attempt: int
     ) -> bool:
         """Called when a function call raises an exception.
@@ -333,7 +390,40 @@
         :param kwargs: Additional arguments to pass to Pydantic's ``model_validate_json``.
         """
         with open(fp) as f:
             data = f.read()
         state = SavedKani.model_validate_json(data, **kwargs)
         self.always_include_messages = state.always_include_messages
         self.chat_history = state.chat_history
+
+    # ==== internals ====
+    def _auto_truncate_message(self, msg: ChatMessage, max_len: int) -> ChatMessage:
+        """Mutate the provided message until it is less than *max_len* tokens long."""
+        full_content = msg.content
+        if not full_content:
+            return msg  # idk how this could happen
+        for chunk_divider in ("\n\n", "\n", ". ", ", ", " "):
+            # chunk the text
+            content = ""
+            last_msg = None
+            chunks = full_content.split(chunk_divider)
+            for idx, chunk in enumerate(chunks):
+                # fit in as many chunks as possible
+                if idx:
+                    content += chunk_divider
+                content += chunk
+                # when it's too long...
+                msg = ChatMessage(role=msg.role, name=msg.name, content=content + "...")
+                if self.message_token_len(msg) > max_len:
+                    # if we have some text, return it
+                    if last_msg:
+                        return last_msg
+                    # otherwise, we need to split into smaller chunks
+                    break
+                # otherwise, continue
+                last_msg = msg
+        # if we get here and have no content, chop it to the first max_len characters
+        log.warning(
+            "Auto truncate could not find an appropriate place to chunk the text. The returned value will be the first"
+            f" {max_len} characters."
+        )
+        return ChatMessage(role=msg.role, name=msg.name, content=full_content[: max_len - 3] + "...")
```

### Comparing `kani-0.0.2/kani/models.py` & `kani-0.0.3/kani/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,44 +34,49 @@
     """The arguments to call it with, encoded in JSON."""
 
     @property
     def kwargs(self) -> dict:
         """The arguments to call the function with, with JSON decoded to a Python dict."""
         return json.loads(self.arguments)
 
+    @classmethod
+    def with_args(cls, name: str, **kwargs):
+        """Create a function call with the given arguments (e.g. for few-shot prompting)."""
+        return cls(name=name, arguments=json.dumps(kwargs))
+
 
 class ChatMessage(BaseModel):
     """Represents a message in the chat context."""
 
     model_config = ConfigDict(frozen=True)
 
     role: ChatRole
     """Who said the message?"""
 
     content: str | None
-    """The content of the message. Can be None only if the message is a function call."""
+    """The content of the message. Can be None only if the message is a requested function call from the assistant."""
 
     name: str | None = None
     """The name of the user who sent the message, if set (user messages only)."""
 
     function_call: FunctionCall | None = None
-    """The function requested by the model (function messages only)."""
+    """The function requested by the model (assistant messages only)."""
 
     @classmethod
-    def system(cls, content: str):
+    def system(cls, content: str, **kwargs):
         """Create a new system message."""
-        return cls(role=ChatRole.SYSTEM, content=content)
+        return cls(role=ChatRole.SYSTEM, content=content, **kwargs)
 
     @classmethod
-    def user(cls, content: str):
+    def user(cls, content: str, **kwargs):
         """Create a new user message."""
-        return cls(role=ChatRole.USER, content=content)
+        return cls(role=ChatRole.USER, content=content, **kwargs)
 
     @classmethod
-    def assistant(cls, content: str):
+    def assistant(cls, content: str | None, **kwargs):
         """Create a new assistant message."""
-        return cls(role=ChatRole.ASSISTANT, content=content)
+        return cls(role=ChatRole.ASSISTANT, content=content, **kwargs)
 
     @classmethod
-    def function(cls, name: str, content: str):
+    def function(cls, name: str, content: str, **kwargs):
         """Create a new function message."""
-        return cls(role=ChatRole.FUNCTION, content=content, name=name)
+        return cls(role=ChatRole.FUNCTION, content=content, name=name, **kwargs)
```

### Comparing `kani-0.0.2/kani/engines/base.py` & `kani-0.0.3/kani/engines/base.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/kani/engines/httpclient.py` & `kani-0.0.3/kani/engines/httpclient.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,8 +69,11 @@
 
     async def post(self, route: str, **kwargs):
         """Convenience method; equivalent to ``self.request("POST", route, **kwargs)``."""
         return await self.request("POST", route, **kwargs)
 
     async def close(self):
         """Close the underlying aiohttp session."""
+        if self.http is None:
+            return
         await self.http.close()
+        self.http = None  # this allows us to reuse the client after it has been closed
```

### Comparing `kani-0.0.2/kani/engines/huggingface/base.py` & `kani-0.0.3/kani/engines/huggingface/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 class HuggingEngine(BaseEngine, abc.ABC):
     """Base engine for all HuggingFace text-generation models.
 
     This class implements the main decoding logic for any HuggingFace model based on a pretrained
     ``AutoModelForCausalLM``. To implement a new HuggingFace model, just implement :meth:`build_prompt` and
     :meth:`~.BaseEngine.message_len` for the specified model.
+
+    .. tip:: See :ref:`4b_quant` for information about loading a quantized model for lower memory usage.
     """
 
     def __init__(
         self,
         model_id: str,
         max_context_size: int,
         use_auth_token=None,
@@ -55,15 +57,16 @@
         self.tokenizer = AutoTokenizer.from_pretrained(model_id, **tokenizer_kwargs)
         self.model = AutoModelForCausalLM.from_pretrained(model_id, **model_load_kwargs)
         self.hyperparams = hyperparams
 
         if device is None:
             device = "cuda" if torch.has_cuda else "cpu"
         self.device = device
-        self.model.to(device)
+        if self.model.device.type != self.device:
+            self.model.to(device)
 
     @abc.abstractmethod
     def build_prompt(
         self, messages: list[ChatMessage], functions: list[AIFunction] | None = None
     ) -> str | torch.Tensor:
         """Given the list of messages from kani, build either a single string representing the prompt for the model,
         or build the token tensor."""
```

### Comparing `kani-0.0.2/kani/engines/huggingface/llama2.py` & `kani-0.0.3/kani/engines/huggingface/llama2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import warnings
 
 from kani.ai_function import AIFunction
 from kani.exceptions import MissingModelDependencies
 from kani.models import ChatMessage, ChatRole
 from .base import HuggingEngine
+from .. import llama2_prompt
+from ..llama2_prompt import B_INST, E_INST, B_SYS, E_SYS
 
 try:
     import torch
+    from torch import tensor
     import sentencepiece
 except ImportError:
     raise MissingModelDependencies(
         'The LlamaEngine requires extra dependencies. Please install kani with "pip install'
         " 'kani[huggingface,llama]'\". You will also need to install PyTorch manually."
     ) from None
 
-B_INST, E_INST = "[INST]", "[/INST]"
-B_SYS, E_SYS = "<<SYS>>\n", "\n<</SYS>>\n\n"
-
 
 class LlamaEngine(HuggingEngine):
     """Implementation of LLaMA v2 using huggingface transformers.
 
     You may also use the 13b, 70b, or other LLaMA models that use the LLaMA prompt by passing the HuggingFace model
     ID to the initializer.
 
@@ -38,14 +38,16 @@
         https://ai.meta.com/resources/models-and-libraries/llama-downloads/ and
         https://huggingface.co/meta-llama/Llama-2-7b-chat-hf to request access.
 
         Then, run ``huggingface-cli login`` to authenticate with Hugging Face.
 
     .. seealso:: https://huggingface.co/meta-llama/Llama-2-7b-chat-hf
 
+    .. tip:: See :ref:`4b_quant` for information about loading a quantized model for lower memory usage.
+
     .. code-block:: python
 
         engine = LlamaEngine("meta-llama/Llama-2-7b-chat-hf", use_auth_token=True, strict=True)
         ai = Kani(engine)
     """
 
     def __init__(self, model_id: str = "meta-llama/Llama-2-7b-chat-hf", *args, strict=False, **kwargs):
@@ -78,38 +80,31 @@
             raise ValueError("Messages after the first must alternate between user and system (LLaMA strict mode).")
         if messages[-1].role != ChatRole.USER:
             raise ValueError("The last message must be from the user (LLaMA strict mode).")
         # implementation based on llama code
         dialog = [f"{B_SYS}{messages[0].content}{E_SYS}{messages[1].content}"] + [m.content for m in messages[2:]]
         dialog_tokens = sum(
             [
-                self.tokenizer.encode(f"{B_INST} {prompt} {E_INST} {answer} </s>")
+                self.tokenizer.encode(f"{B_INST} {prompt} {E_INST} {answer}") + [self.tokenizer.eos_token_id]
                 for prompt, answer in zip(dialog[::2], dialog[1::2])
             ],
             [],
         )
         dialog_tokens += self.tokenizer.encode(f"{B_INST} {dialog[-1]} {E_INST}")
-        return torch.tensor([dialog_tokens], dtype=torch.long)
+        return torch.tensor([dialog_tokens], device=self.device)
 
     def build_prompt(self, messages: list[ChatMessage], functions: list[AIFunction] | None = None) -> torch.Tensor:
         if functions:
             warnings.warn("The LlamaEngine is conversational only and does not support function calling.")
         if self.strict:
             return self._build_prompt_strict(messages)
         # non-strict has to kind of just do its best
         # ganbatte, kani, ganbatte
-        prompt_parts = []
-        for message in messages:
-            if message.role == ChatRole.USER:
-                prompt_parts.append(f"<s> {B_INST} {message.content} {E_INST}")
-            elif message.role == ChatRole.ASSISTANT:
-                prompt_parts.append(f" {message.content} </s>")
-            else:
-                prompt_parts.append(f"{B_INST} {B_SYS}{message.content}{E_SYS} {E_INST}")
-        return self.tokenizer.encode("".join(prompt_parts), add_special_tokens=False, return_tensors="pt")
+        tokens = llama2_prompt.build(messages, tokenize=self.tokenizer.encode, eos_token_id=self.tokenizer.eos_token_id)
+        return torch.tensor([tokens], device=self.device)
 
     def message_len(self, message: ChatMessage) -> int:
         # https://github.com/facebookresearch/llama/blob/main/llama/generation.py#L212
         if message.role == ChatRole.USER:
             # <s> [INST] {} [/INST] -> 7
             return self.tokenizer(message.content, return_length=True).length[0] + 7
         elif message.role == ChatRole.ASSISTANT:
```

### Comparing `kani-0.0.2/kani/engines/huggingface/vicuna.py` & `kani-0.0.3/kani/engines/huggingface/vicuna.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     """Implementation of Vicuna (a LLaMA v1 fine-tune) using huggingface transformers.
 
     You may also use the 13b, 33b, or other LLaMA models that use the Vicuna prompt by passing the HuggingFace model
     ID to the initializer.
 
     .. seealso:: https://huggingface.co/lmsys/vicuna-7b-v1.3
 
+    .. tip:: See :ref:`4b_quant` for information about loading a quantized model for lower memory usage.
+
     .. code-block:: python
 
         engine = VicunaEngine("lmsys/vicuna-7b-v1.3")
         ai = Kani(engine)
     """
 
     # all prompts start with a hidden <s> token and ASSISTANT:
```

### Comparing `kani-0.0.2/kani/engines/openai/client.py` & `kani-0.0.3/kani/engines/openai/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,30 @@
 
 
 class OpenAIClient(BaseClient):
     """Simple HTTP client to interface with the OpenAI API."""
 
     SERVICE_BASE = "https://api.openai.com/v1"
 
-    def __init__(self, api_key: str, http: aiohttp.ClientSession = None):
+    def __init__(self, api_key: str, http: aiohttp.ClientSession = None, organization: str = None, retry: int = 5):
         super().__init__(http)
         self.api_key = api_key
+        self.organization = organization
+        self.retry = retry
 
-    async def request(self, method: str, route: str, headers=None, retry=5, **kwargs):
+    async def request(self, method: str, route: str, headers=None, retry=None, **kwargs):
         if headers is None:
             headers = {}
+        # set up auth headers
         headers["Authorization"] = f"Bearer {self.api_key}"
+        if self.organization:
+            headers["OpenAI-Organization"] = self.organization
+
+        # make the request
+        retry = retry if retry is not None else self.retry
         for i in range(retry):
             try:
                 return await super().request(method, route, headers=headers, **kwargs)
             except (HTTPStatusException, HTTPTimeout) as e:
                 if (i + 1) == retry:
                     raise
                 retry_sec = 2**i
```

### Comparing `kani-0.0.2/kani/engines/openai/engine.py` & `kani-0.0.3/kani/engines/openai/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,25 +35,30 @@
     """
 
     def __init__(
         self,
         api_key: str = None,
         model="gpt-3.5-turbo",
         max_context_size: int = None,
+        organization: str = None,
+        retry: int = 5,
         *,
         client: OpenAIClient = None,
         **hyperparams,
     ):
         """
         :param api_key: Your OpenAI API key.
         :param model: The key of the model to use.
         :param max_context_size: The maximum amount of tokens allowed in the chat prompt. If None, uses the given
             model's full context size.
+        :param organization: The OpenAI organization to use in requests (defaults to the API key's default org).
+        :param retry: How many times the engine should retry failed HTTP calls with exponential backoff (default 5).
         :param client: An instance of :class:`.OpenAIClient` (for reusing the same client in multiple engines). You must
-            specify exactly one of (api_key, client).
+            specify exactly one of (api_key, client). If this is passed the ``organization`` and ``retry`` params will
+            be ignored.
         :param hyperparams: Any additional parameters to pass to
             :meth:`.OpenAIClient.create_chat_completion`.
         """
         if (api_key is None and client is None) or (api_key and client):
             raise ValueError("You must supply exactly one of (api_key, client).")
         if max_context_size is None:
             max_context_size = next(size for prefix, size in CONTEXT_SIZES_BY_PREFIX if model.startswith(prefix))
@@ -68,15 +73,17 @@
     def _load_tokenizer(self):
         try:
             self.tokenizer = tiktoken.encoding_for_model(self.model)
         except KeyError:
             self.tokenizer = tiktoken.get_encoding("cl100k_base")
 
     def message_len(self, message: ChatMessage) -> int:
-        mlen = len(self.tokenizer.encode(message.content)) + 5  # ChatML = 4, role = 1
+        mlen = 5  # ChatML = 4, role = 1
+        if message.content:
+            mlen += len(self.tokenizer.encode(message.content))
         if message.name:
             mlen += len(self.tokenizer.encode(message.name))
         if message.function_call:
             mlen += len(self.tokenizer.encode(message.function_call.name))
             mlen += len(self.tokenizer.encode(message.function_call.arguments))
         return mlen
```

### Comparing `kani-0.0.2/kani/engines/openai/models.py` & `kani-0.0.3/kani/engines/openai/models.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/kani/utils/cli.py` & `kani-0.0.3/kani/utils/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
             if stopword and query == stopword:
                 break
             async for msg in kani.full_round_str(query, function_call_formatter=_function_formatter):
                 print(f"AI: {msg}")
     except KeyboardInterrupt:
         pass
     finally:
-        if not rounds:
-            await kani.engine.close()
+        await kani.engine.close()
 
 
 def chat_in_terminal(kani: Kani, rounds: int = 0, stopword: str = None):
     """Chat with a kani right in your terminal.
 
     Useful for playing with kani, quick prompt engineering, or demoing the library.
 
@@ -45,13 +44,17 @@
 
         This function is only a development utility and should not be used in production.
 
     :param rounds: The number of chat rounds to play (defaults to 0 for infinite).
     :param stopword: Break out of the chat loop if the user sends this message.
     """
     try:
-        asyncio.run(chat_in_terminal_async(kani, rounds=rounds, stopword=stopword))
+        asyncio.get_running_loop()
     except RuntimeError:
+        pass
+    else:
         print(
             f"WARNING: It looks like you're in an environment with a running asyncio loop (e.g. Google Colab).\nYou"
             f" should use `await chat_in_terminal_async(...)` instead."
         )
+        return
+    asyncio.run(chat_in_terminal_async(kani, rounds=rounds, stopword=stopword))
```

### Comparing `kani-0.0.2/tests/test_type_spec.py` & `kani-0.0.3/tests/test_type_spec.py`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/.gitignore` & `kani-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/LICENSE` & `kani-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kani-0.0.2/README.md` & `kani-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 
 kani (カニ) is a lightweight and highly hackable harness for chat-based language models with tool usage/function calling.
 
 Compared to other LM harnesses, kani is less opinionated and offers more fine-grained customizability
 over the parts of the control flow that matter, making it the perfect choice for NLP researchers, hobbyists, and
 developers alike.
 
+kani comes with support for OpenAI models and LLaMA v2 out of the box, with a model-agnostic framework to add support
+for many more.
+
 [Read the docs on ReadTheDocs!](http://kani.readthedocs.io/)
 
 ## Features
 
 - **Lightweight and high-level** - kani implements common boilerplate to interface with language models without forcing
   you to use opinionated prompt frameworks or complex library-specific tooling.
+- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
+  Implement these two, and kani can run with any language model.
 - **Automatic chat memory management** - Allow chat sessions to flow without worrying about managing the number of
   tokens in the history - kani takes care of it.
 - **Function calling with model feedback and retry** - Give models access to functions in just one line of code.
   kani elegantly provides feedback about hallucinated parameters and errors and allows the model to retry calls.
-- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
-  Implement these two, and kani can run with any language model.
-- **You are in control** - You can override and provide a custom implementation for all
-  of these features, allowing you to run experiments just the way you want to. There are no hidden prompt hacks.
+- **You control the prompts** - There are no hidden prompt hacks. We will never decide for you how to format your own
+  data, unlike other popular language model libraries.
 - **Fast to iterate and intuitive to learn** - With kani, you only write Python - we handle the rest.
 - **Asynchronous design from the start** - kani can scale to run multiple chat sessions in parallel easily, without
   having to manage multiple processes or programs.
 
 ## Quickstart
 
 kani requires Python 3.10 or above.
@@ -63,21 +66,32 @@
 # the docs for how to use kani programmatically.
 chat_in_terminal(ai)
 ```
 
 kani makes the time to set up a working chat model short, while offering the programmer deep customizability over
 every prompt, function call, and even the underlying language model.
 
+## Docs
+
 To learn more about how
 to [customize kani with your own prompt wrappers](https://kani.readthedocs.io/en/latest/customization.html),
 [function calling](https://kani.readthedocs.io/en/latest/function_calling.html), and
 more, [read the docs!](http://kani.readthedocs.io/)
 
 Or take a look at the hands-on examples [in this repo](https://github.com/zhudotexe/kani/tree/main/examples).
 
+## Demo
+
+Want to see kani in action? Using 4-bit quantization to shrink the model, we run LLaMA v2 as part of our test suite
+right on GitHub Actions:
+
+https://github.com/zhudotexe/kani/actions/workflows/pytest.yml?query=branch%3Amain
+
+Simply click on the latest build to see LLaMA's output!
+
 <!--
 For developers:
 
 ## Build and Publish
 
 `fastlmi` uses Hatchling to build.
```

### Comparing `kani-0.0.2/pyproject.toml` & `kani-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kani"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Andrew Zhu", email = "andrew@zhu.codes" },
 ]
 description = "kani (カニ) is a lightweight and highly hackable harness for chat-based language models with tool usage/function calling."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
@@ -19,15 +19,14 @@
     # https://pypi.org/classifiers/
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "aiohttp>=3.0.0,<4.0.0",
-    "cachetools>=5.0.0,<6.0.0",
     "pydantic>=2.0.0,<3.0.0",
 ]
 
 [project.optional-dependencies]
 huggingface = [
     "transformers>=4.0.0,<5.0.0",
 ]
@@ -36,14 +35,22 @@
     "sentencepiece~=0.1.99",
 ]
 
 openai = [
     "tiktoken~=0.4.0",
 ]
 
+ctransformers = [
+    "ctransformers~=0.2.14",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/zhudotexe/kani"
 "Bug Tracker" = "https://github.com/zhudotexe/kani/issues"
 
 [tool.black]
 line-length = 120
 preview = true
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+markers = ["llama: these tests use a real LLaMA v2 model."]
```

### Comparing `kani-0.0.2/PKG-INFO` & `kani-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kani
-Version: 0.0.2
+Version: 0.0.3
 Summary: kani (カニ) is a lightweight and highly hackable harness for chat-based language models with tool usage/function calling.
 Project-URL: Homepage, https://github.com/zhudotexe/kani
 Project-URL: Bug Tracker, https://github.com/zhudotexe/kani/issues
 Author-email: Andrew Zhu <andrew@zhu.codes>
 License: MIT License
         
         Copyright (c) 2023 Andrew Zhu
@@ -31,16 +31,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Requires-Dist: aiohttp<4.0.0,>=3.0.0
-Requires-Dist: cachetools<6.0.0,>=5.0.0
 Requires-Dist: pydantic<3.0.0,>=2.0.0
+Provides-Extra: ctransformers
+Requires-Dist: ctransformers~=0.2.14; extra == 'ctransformers'
 Provides-Extra: huggingface
 Requires-Dist: transformers<5.0.0,>=4.0.0; extra == 'huggingface'
 Provides-Extra: llama
 Requires-Dist: sentencepiece~=0.1.99; extra == 'llama'
 Provides-Extra: openai
 Requires-Dist: tiktoken~=0.4.0; extra == 'openai'
 Description-Content-Type: text/markdown
@@ -54,28 +55,31 @@
 
 kani (カニ) is a lightweight and highly hackable harness for chat-based language models with tool usage/function calling.
 
 Compared to other LM harnesses, kani is less opinionated and offers more fine-grained customizability
 over the parts of the control flow that matter, making it the perfect choice for NLP researchers, hobbyists, and
 developers alike.
 
+kani comes with support for OpenAI models and LLaMA v2 out of the box, with a model-agnostic framework to add support
+for many more.
+
 [Read the docs on ReadTheDocs!](http://kani.readthedocs.io/)
 
 ## Features
 
 - **Lightweight and high-level** - kani implements common boilerplate to interface with language models without forcing
   you to use opinionated prompt frameworks or complex library-specific tooling.
+- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
+  Implement these two, and kani can run with any language model.
 - **Automatic chat memory management** - Allow chat sessions to flow without worrying about managing the number of
   tokens in the history - kani takes care of it.
 - **Function calling with model feedback and retry** - Give models access to functions in just one line of code.
   kani elegantly provides feedback about hallucinated parameters and errors and allows the model to retry calls.
-- **Model agnostic** - kani provides a simple interface to implement: token counting and completion generation.
-  Implement these two, and kani can run with any language model.
-- **You are in control** - You can override and provide a custom implementation for all
-  of these features, allowing you to run experiments just the way you want to. There are no hidden prompt hacks.
+- **You control the prompts** - There are no hidden prompt hacks. We will never decide for you how to format your own
+  data, unlike other popular language model libraries.
 - **Fast to iterate and intuitive to learn** - With kani, you only write Python - we handle the rest.
 - **Asynchronous design from the start** - kani can scale to run multiple chat sessions in parallel easily, without
   having to manage multiple processes or programs.
 
 ## Quickstart
 
 kani requires Python 3.10 or above.
@@ -110,21 +114,32 @@
 # the docs for how to use kani programmatically.
 chat_in_terminal(ai)
 ```
 
 kani makes the time to set up a working chat model short, while offering the programmer deep customizability over
 every prompt, function call, and even the underlying language model.
 
+## Docs
+
 To learn more about how
 to [customize kani with your own prompt wrappers](https://kani.readthedocs.io/en/latest/customization.html),
 [function calling](https://kani.readthedocs.io/en/latest/function_calling.html), and
 more, [read the docs!](http://kani.readthedocs.io/)
 
 Or take a look at the hands-on examples [in this repo](https://github.com/zhudotexe/kani/tree/main/examples).
 
+## Demo
+
+Want to see kani in action? Using 4-bit quantization to shrink the model, we run LLaMA v2 as part of our test suite
+right on GitHub Actions:
+
+https://github.com/zhudotexe/kani/actions/workflows/pytest.yml?query=branch%3Amain
+
+Simply click on the latest build to see LLaMA's output!
+
 <!--
 For developers:
 
 ## Build and Publish
 
 `fastlmi` uses Hatchling to build.
```

