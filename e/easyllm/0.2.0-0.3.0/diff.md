# Comparing `tmp/easyllm-0.2.0.tar.gz` & `tmp/easyllm-0.3.0.tar.gz`

## Comparing `easyllm-0.2.0.tar` & `easyllm-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,50 @@
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.2.0/makefile
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 easyllm-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/check.yaml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 easyllm-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/clients.md
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/installation.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 easyllm-0.2.0/docs/prompt_utils.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/cli.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/clients/__init__.py
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/clients/huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/evol_instruct/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/base.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/prompt_utils/llama2.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/schema/base.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 easyllm-0.2.0/easyllm/schema/openai.py
--rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/chat-completion-api.ipynb
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/get-embeddings.ipynb
--rw-r--r--   0        0        0    41821 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/steam-text-completions.ipynb
--rw-r--r--   0        0        0    49555 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/stream-chat-completions.ipynb
--rw-r--r--   0        0        0     9013 2020-02-02 00:00:00.000000 easyllm-0.2.0/notebooks/text-completion-api.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.2.0/scripts/.gitkeep
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.2.0/tests/test_main.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 easyllm-0.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.2.0/LICENSE
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 easyllm-0.2.0/README.md
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 easyllm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 easyllm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 easyllm-0.3.0/makefile
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 easyllm-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/build-documentation.yaml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/check.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/deploy-documentation.yaml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/installation.md
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/prompt_utils.md
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/clients/huggingface.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/clients/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/examples/.gitkeep
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/examples/index.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/cli.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/clients/__init__.py
+-rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/clients/huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/evol_instruct/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/base.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/chatml_hf.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/llama2.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/open_assistant.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/stablebeluga.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/vicuna.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/wizardlm.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/schema/base.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/schema/openai.py
+-rw-r--r--   0        0        0    19400 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/chat-completion-api.ipynb
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/get-embeddings.ipynb
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/inference-endpoints-example.ipynb
+-rw-r--r--   0        0        0    26151 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/stream-chat-completions.ipynb
+-rw-r--r--   0        0        0    41712 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/stream-text-completions.ipynb
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/text-completion-api.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/scripts/.gitkeep
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/test_main.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_chatml_hf.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_llama2.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_open_assistant.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_stablebeluga.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_vicuna.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_wizardlm.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 easyllm-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 easyllm-0.3.0/README.md
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 easyllm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 easyllm-0.3.0/PKG-INFO
```

### Comparing `easyllm-0.2.0/mkdocs.yml` & `easyllm-0.3.0/mkdocs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -103,17 +103,25 @@
           format: !!python/name:pymdownx.superfences.fence_code_format
   - pymdownx.tabbed:
       alternate_style: true
   - pymdownx.tasklist:
       custom_checkbox: true
   - pymdownx.tilde
 
-
 nav:
   - Documentation:
     - EasyLLM: index.md 
     - Installation: installation.md
-    - "Getting Started":
-      - clients.md
+    - "API Reference":
+      - "Clients":
+        - clients/index.md
+        - clients/huggingface.md
+      - prompt_utils.md
   - Examples:
-    - examples/chat-completion-api.ipynb
-    - examples/stream-chat-completions.ipynb
+    - examples/index.md
+    - "Hugging Face":
+      - examples/chat-completion-api.ipynb
+      - examples/stream-chat-completions.ipynb
+      - examples/text-completion-api.ipynb
+      - examples/stream-text-completions.ipynb
+      - examples/get-embeddings.ipynb
+      - examples/inference-endpoints-example.ipynb
```

### Comparing `easyllm-0.2.0/.github/workflows/check.yaml` & `easyllm-0.3.0/.github/workflows/check.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 name: Quality Check
 
 on:
   push:
     branches:
       - main
   pull_request:
+      paths:
+      - 'easyllm/**'
+      - 'tests/**'
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
@@ -27,8 +30,8 @@
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-check
       - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install ".[dev]"
       - name: Run library checks
-        run: make check
+        run: make check
```

### Comparing `easyllm-0.2.0/.github/workflows/documentation.yaml` & `easyllm-0.3.0/.github/workflows/deploy-documentation.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 name: Publish documentation
 
 on:
+  push:
+    branches:
+      - main
+    paths:
+      - 'docs/**'
+      - 'notebooks/**'
   release:
     types:
       - created
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
```

### Comparing `easyllm-0.2.0/.github/workflows/publish.yaml` & `easyllm-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.2.0/.github/workflows/test.yaml` & `easyllm-0.3.0/.github/workflows/test.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 name: Unit Tests
 
 on:
   push:
     branches:
       - main
   pull_request:
+    paths:
+      - 'easyllm/**'
+      - 'tests/**'
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
@@ -27,8 +30,8 @@
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test
       - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install ".[test]"
       - name: Run tests
-        run: pytest
+        run: pytest
```

### Comparing `easyllm-0.2.0/docs/clients.md` & `easyllm-0.3.0/docs/clients/huggingface.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-# Clients
+# Hugging Face 
 
-In the context of EasyLLM, a "client" refers to the code that interfaces with a particular LLM API, e.g. OpenAI.
-
-Currently supported clients are:  
-
-- `ChatCompletion` - ChatCompletion clients are used to interface with LLMs that are compatible with the OpenAI ChatCompletion API.
-- `Completion` - Completion clients are used to interface with LLMs that are compatible with the OpenAI Completion API.
-- `Embedding` - Embedding clients are used to interface with LLMs that are compatible with the OpenAI Embedding API.
-
-Currently supported clients are:  
+EasyLLM provides a client for interfacing with HuggingFace models. The client is compatible with the [HuggingFace Inference API](https://huggingface.co/docs/api-inference/index), [Hugging Face Inference Endpoints](https://huggingface.co/docs/inference-endpoints/index) or any Web Service running [Text Generation Inference](https://github.com/huggingface/text-generation-inference) or compatible API endpoints. 
 
 - `huggingface.ChatCompletion` - a client for interfacing with HuggingFace models that are compatible with the OpenAI ChatCompletion API.
 - `huggingface.Completion` - a client for interfacing with HuggingFace models that are compatible with the OpenAI Completion API.
 - `huggingface.Embedding` - a client for interfacing with HuggingFace models that are compatible with the OpenAI Embedding API.
 
 ## `huggingface.ChatCompletion`
 
-The `huggingface.ChatCompletion` client is used to interface with HuggingFace models running on Text Generation infernece that are compatible with the OpenAI ChatCompletion API. Checkout the [Examples](../examples/chat-completion-api) for more details and [How to stream completions](../examples/stream-chat-completion-api) for an example how to stream requests.
+The `huggingface.ChatCompletion` client is used to interface with HuggingFace models running on Text Generation inference that are compatible with the OpenAI ChatCompletion API. Checkout the [Examples](../examples/chat-completion-api) for more details and [How to stream completions](../examples/stream-chat-completion-api) for an example how to stream requests.
 
 
 ```python
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
 # The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.
 # huggingface.api_key="hf_xxx"
-hubbingface.prompt_builder = build_llama2_prompt
+hubbingface.prompt_builder = "llama2"
 
 response = huggingface.ChatCompletion.create(
     model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "\nYou are a helpful, respectful and honest assistant."},
         {"role": "user", "content": "Knock knock."},
     ],
@@ -38,52 +29,51 @@
     max_tokens=1024,
 )
 ```
 
 
 Supported parameters are:
 
-* `model` - The model to use for the completion. If not provided, the defaults to base url.
+* `model` - The model to use for the completion. If not provided, defaults to the base url.
 * `messages` - `List[ChatMessage]` to use for the completion.
 * `temperature` - The temperature to use for the completion. Defaults to 0.9.
 * `top_p` - The top_p to use for the completion. Defaults to 0.6.
 * `top_k` - The top_k to use for the completion. Defaults to 10.
 * `n` - The number of completions to generate. Defaults to 1.
 * `max_tokens` - The maximum number of tokens to generate. Defaults to 1024.
 * `stop` - The stop sequence(s) to use for the completion. Defaults to None.
 * `stream` - Whether to stream the completion. Defaults to False.
 * `frequency_penalty` - The frequency penalty to use for the completion. Defaults to 1.0.
 * `debug` - Whether to enable debug logging. Defaults to False.
 
 ## `huggingface.Completion`
 
-The `huggingface.Completion` client is used to interface with HuggingFace models running on Text Generation infernece that are compatible with the OpenAI Completion API. Checkout the [Examples](../examples/text-completion-api) for more details and [How to stream completions](../examples/stream-text-completion-api) for an example how to stream requests.
+The `huggingface.Completion` client is used to interface with HuggingFace models running on Text Generation inference that are compatible with the OpenAI Completion API. Checkout the [Examples](../examples/text-completion-api) for more details and [How to stream completions](../examples/stream-text-completion-api) for an example how to stream requests.
 
 
 ```python
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
 # The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.
 # huggingface.api_key="hf_xxx"
-hubbingface.prompt_builder = build_llama2_prompt
+hubbingface.prompt_builder = "llama2"
 
 response = huggingface.Completion.create(
     model="meta-llama/Llama-2-70b-chat-hf",
     prompt="What is the meaning of life?",
     temperature=0.9,
     top_p=0.6,
     max_tokens=1024,
 )
 ```
 
 
 Supported parameters are:
 
-* `model` - The model to use for the completion. If not provided, the defaults to base url.
+* `model` - The model to use for the completion. If not provided, defaults to the base url.
 * `prompt` -  Text to use for the completion, if prompt_builder is set, prompt will be formatted with the prompt_builder.
 * `temperature` - The temperature to use for the completion. Defaults to 0.9.
 * `top_p` - The top_p to use for the completion. Defaults to 0.6.
 * `top_k` - The top_k to use for the completion. Defaults to 10.
 * `n` - The number of completions to generate. Defaults to 1.
 * `max_tokens` - The maximum number of tokens to generate. Defaults to 1024.
 * `stop` - The stop sequence(s) to use for the completion. Defaults to None.
@@ -110,60 +100,100 @@
 )
 
 len(embedding["data"][0]["embedding"])
 ```
 
 Supported parameters are:
 
-* `model` - The model to use to create the embedding. If not provided, the defaults to base url.
+* `model` - The model to use to create the embedding. If not provided, defaults to the base url.
 * `input` -  `Union[str, List[str]]` document(s) to embed.
 
 
 ## Environment Configuration
 
 You can configure the `huggingface` client by setting environment variables or overwriting the default values. See below on how to adjust the HF token, url and prompt builder.
 
 ### Setting HF token 
 
 By default the `huggingface` client will try to read the `HUGGINGFACE_TOKEN` environment variable. If this is not set, it will try to read the token from the `~/.huggingface` folder. If this is not set, it will not use a token.
 
 Alternatively you can set the token manually by setting `huggingface.api_key`.
 
+
+manually setting the api key:
+
 ```python
 from easyllm.clients import huggingface
 
 huggingface.api_key="hf_xxx"
 
 res = huggingface.ChatCompletion.create(...)
 ```
 
+Using environment variable:
+
+```python
+# can happen elsehwere
+import os
+os.environ["HUGGINGFACE_TOKEN"] = "hf_xxx"
+
+from easyllm.clients import huggingface
+```
+
+
 ### Changing url 
 
-By default the `huggingface` client will try to read the `HUGGINGFACE_API_BASE` environment variable. If this is not set, it will use the default url `https://api-inference.huggingface.co/models`. This is helpful if you want to use a different url like `https://api-inference.huggingface.co/models` or a local url like `http://localhost:8000` or an Hugging Face Inference Endpoint.
+By default the `huggingface` client will try to read the `HUGGINGFACE_API_BASE` environment variable. If this is not set, it will use the default url `https://api-inference.huggingface.co/models`. This is helpful if you want to use a different url like `https://zj5lt7pmzqzbp0d1.us-east-1.aws.endpoints.huggingface.cloud` or a local url like `http://localhost:8000` or an Hugging Face Inference Endpoint.
 
-Alternatively you can set the url manually by setting `huggingface.api_base`.
+Alternatively you can set the url manually by setting `huggingface.api_base`. If you set a custom you have to leave the `model` parameter empty. 
 
+manually setting the api base:
 
 ```python
 from easyllm.clients import huggingface
 
-huggingface.api_base="hf_xxx"
+huggingface.api_base="https://my-url"
+
 
 res = huggingface.ChatCompletion.create(...)
 ```
 
-### Build Prompt
+Using environment variable:
+
+```python
+# can happen elsehwere
+import os
+os.environ["HUGGINGFACE_API_BASE"] = "https://my-url"
+
+from easyllm.clients import huggingface
+```
+
 
-prompt_builder = None
 
-By default the `huggingface` client has no `prompt_builder` set. If you want to use the `prompt_builder` you have to set it manually. If you don't set it, the client will use the default.
+
+### Build Prompt
+
+By default the `huggingface` client will try to read the `HUGGINGFACE_PROMPT` environment variable and tries to map the value to the `PROMPT_MAPPING` dictionary. If this is not set, it will use the default prompt builder. 
+You can also set it manually.
 
 Checkout the [Prompt Utils](../prompt_utils) for more details.
 
+
+manually setting the prompt builder:
+
 ```python
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
-huggingface.prompt_builder = build_llama2_prompt
+huggingface.prompt_builder = "llama2"
 
 res = huggingface.ChatCompletion.create(...)
+```
+
+Using environment variable:
+
+```python
+# can happen elsehwere
+import os
+os.environ["HUGGINGFACE_PROMPT"] = "llama2"
+
+from easyllm.clients import huggingface
 ```
```

### Comparing `easyllm-0.2.0/docs/index.md` & `easyllm-0.3.0/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # EasyLLM
 
 EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. 
 
 EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion` with, for example, `huggingface.ChatCompletion`.
 
-* [ChatCompletion Clients](./clients.md)
-* [Prompt Utils](./prompt_utils.md)
-* [Examples](./examples/chat-completion-api.md)
+* [ChatCompletion Clients](./clients)
+* [Prompt Utils](./prompt_utils)
+* [Examples](./examples)
 
 ## 🚀 Getting Started
 
 Install EasyLLM via pip:
 
 ```bash
 pip install easyllm
 ```
 
 Then import and start using the clients:
 
 ```python
 
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
 # helper to build llama2 prompt
-huggingface.prompt_builder = build_llama2_prompt
+huggingface.prompt_builder = "llama2"
 
 response = huggingface.ChatCompletion.create(
     model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "\nYou are a helpful assistant speaking like a pirate. argh!"},
         {"role": "user", "content": "What is the sun?"},
     ],
-      temperature=0.9,
-      top_p=0.6,
-      max_tokens=256,
+    temperature=0.9,
+    top_p=0.6,
+    max_tokens=256,
 )
 
 print(response)
 ```
 the result will look like 
 
 ```bash
@@ -61,32 +60,35 @@
     "prompt_tokens": 111,
     "completion_tokens": 299,
     "total_tokens": 410
   }
 }
 ```
 
-Check out other examples:  
+Check out other examples:
 
 * [Detailed ChatCompletion Example](examples/chat-completion-api)
-* [Example how to stream requests](examples/stream-chat-completion-api)
+* [Example how to stream chat requests](examples/stream-chat-completion)
+* [Example how to stream text requests](examples/stream-text-completion)
+* [Detailed Completion Example](examples/text-completion-api)
+* [Create Embeddings](examples/get-embeddings)
 
 
 ## 💪🏻 Migration from OpenAI to HuggingFace
 
 Migrating from OpenAI to HuggingFace is easy. Just change the import statement and the client you want to use and optionally the prompt builder.
 
 ```diff
--import openai
+- import openai
 + from easyllm.clients import huggingface
-+ huggingface.prompt_builder = build_llama2_prompt
++ huggingface.prompt_builder = "llama2"
 
 
--response = openai.ChatCompletion.create(
-+response = huggingface.ChatCompletion.create(
+- response = openai.ChatCompletion.create(
++ response = huggingface.ChatCompletion.create(
 -    model="gpt-3.5-turbo",
 +    model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Knock knock."},
     ],
 )
@@ -96,15 +98,15 @@
 
 ## ☑️ Key Features
 
 ### 🤝 Compatible Clients
 
 - Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`.
 - Easily switch between different LLMs like `openai.ChatCompletion` and `huggingface.ChatCompletion` by changing one line of code. 
-- Support for streaming of completions, checkout example [How to stream completions](./notebooks/stream-chat-completions.ipynb).
+- Support for streaming of completions, checkout example [How to stream completions](examples/stream-chat-completions).
 
 ### ⚙️ Helper Modules ⚙️
 
 - `evol_instruct` (work in progress) - Use evolutionary algorithms create instructions for LLMs.
 
 - `prompt_utils` - Helper methods to easily convert between prompt formats like OpenAI Messages to prompts for open source models like Llama 2.
```

### Comparing `easyllm-0.2.0/easyllm/utils.py` & `easyllm-0.3.0/easyllm/utils.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.2.0/easyllm/clients/huggingface.py` & `easyllm-0.3.0/easyllm/clients/huggingface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
 import os
-from typing import Any, Dict
+from typing import Any, Dict, List, Optional, Union
 
 from huggingface_hub import HfFolder, InferenceClient
 from nanoid import generate
 
-from easyllm.prompt_utils.base import buildBasePrompt
+from easyllm.prompt_utils.base import build_prompt, buildBasePrompt
 from easyllm.schema.base import ChatMessage, Usage
 from easyllm.schema.openai import (
     ChatCompletionRequest,
     ChatCompletionResponse,
     ChatCompletionResponseChoice,
     ChatCompletionResponseStreamChoice,
     ChatCompletionStreamResponse,
@@ -24,18 +24,23 @@
     EmbeddingsRequest,
     EmbeddingsResponse,
 )
 from easyllm.utils import logger
 
 # default parameters
 api_type = "huggingface"
-api_key = os.getenv("HUGGINGFACE_TOKEN") or HfFolder.get_token()
-api_base = os.getenv("HUGGINGFACE_API_BASE") or "https://api-inference.huggingface.co/models"
-api_version = os.getenv("HUGGINGFACE_API_VERSION") or "2023-07-29"
-prompt_builder = None
+api_key = (
+    os.environ.get(
+        "HUGGINGFACE_TOKEN",
+    )
+    or HfFolder.get_token()
+)
+api_base = os.environ.get("HUGGINGFACE_API_BASE", None) or "https://api-inference.huggingface.co/models"
+api_version = os.environ.get("HUGGINGFACE_API_VERSION", None) or "2023-07-29"
+prompt_builder = os.environ.get("HUGGINGFACE_PROMPT", None)
 stop_sequences = []
 seed = 42
 
 
 def stream_chat_request(client, prompt, stop, gen_kwargs, model):
     """Utility function for streaming chat requests."""
     id = f"hf-{generate(size=10)}"
@@ -74,114 +79,147 @@
         model=model,
         choices=[ChatCompletionResponseStreamChoice(index=0, finish_reason=reason, delta={})],
     ).model_dump(exclude_none=True)
 
 
 class ChatCompletion:
     @staticmethod
-    def create(**kwargs) -> Dict[str, Any]:
+    def create(
+        messages: List[ChatMessage],
+        model: Optional[str] = None,
+        temperature: float = 0.9,
+        top_p: float = 0.6,
+        top_k: Optional[int] = 10,
+        n: int = 1,
+        max_tokens: int = 1024,
+        stop: Optional[List[str]] = None,
+        stream: bool = False,
+        frequency_penalty: Optional[float] = 1.0,
+        debug: bool = False,
+    ) -> Dict[str, Any]:
         """
         Creates a new chat completion for the provided messages and parameters.
+
         Args:
-            param1 (int): The first parameter.
-            param2 (Optional[str]): The second parameter. Defaults to None.
+            messages (`List[ChatMessage]`): to use for the completion.
+            model (`str`, *optional*, defaults to None): The model to use for the completion. If not provided,
+                defaults to the base url.
+            temperature (`float`, defaults to 0.9): The temperature to use for the completion.
+            top_p (`float`, defaults to 0.6): The top_p to use for the completion.
+            top_k (`int`, *optional*, defaults to 10): The top_k to use for the completion.
+            n (`int`, defaults to 1): The number of completions to generate.
+            max_tokens (`int`, defaults to 1024): The maximum number of tokens to generate.
+            stop (`List[str]`, *optional*, defaults to None): The stop sequence(s) to use for the completion.
+            stream (`bool`, defaults to False): Whether to stream the completion.
+            frequency_penalty (`float`, *optional*, defaults to 1.0): The frequency penalty to use for the completion.
+            debug (`bool`, defaults to False): Whether to enable debug logging.
 
         Tip: Prompt builder
             Make sure to always use a prompt builder for your model.
         """
-        # deserialize the request
-        debug = kwargs.pop("debug", False)
         if debug:
             logger.setLevel(logging.DEBUG)
 
-        r = ChatCompletionRequest(**kwargs)
+        request = ChatCompletionRequest(
+            messages=messages,
+            model=model,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            n=n,
+            max_tokens=max_tokens,
+            stop=stop,
+            stream=stream,
+            frequency_penalty=frequency_penalty,
+        )
 
         if prompt_builder is None:
-            logging.warn(
+            logger.warn(
                 f"""huggingface.prompt_builder is not set.
 Using default prompt builder for. Prompt sent to model will be:
 ----------------------------------------
-{buildBasePrompt(r.messages)}.
+{buildBasePrompt(request.messages)}.
 ----------------------------------------
 If you want to use a custom prompt builder, set huggingface.prompt_builder to a function that takes a list of messages and returns a string.
 You can also use existing prompt builders by importing them from easyllm.prompt_utils"""
             )
-            prompt = buildBasePrompt(r.messages)
+            prompt = buildBasePrompt(request.messages)
         else:
-            prompt = prompt_builder(r.messages)
-        logger.debug(f"Prompt sent to model will be:\n{prompt}")
+            prompt = build_prompt(request.messages, prompt_builder)
 
         # if the model is a url, use it directly
-        if r.model:
-            url = f"{api_base}/{r.model}"
+        if request.model:
+            url = f"{api_base}/{request.model}"
             logger.debug(f"Url:\n{url}")
+        else:
+            url = api_base
 
         # create the client
         client = InferenceClient(url, token=api_key)
 
         # create stop sequences
-        if isinstance(r.stop, list):
-            stop = stop_sequences + r.stop
-        if isinstance(r.stop, str):
-            stop = stop_sequences + [r.stop]
+        if isinstance(request.stop, list):
+            stop = stop_sequences + request.stop
+        if isinstance(request.stop, str):
+            stop = stop_sequences + [request.stop]
         else:
             stop = stop_sequences
         logger.debug(f"Stop sequences:\n{stop}")
 
         # check if we can stream
-        if r.stream is True and r.n > 1:
+        if request.stream is True and request.n > 1:
             raise ValueError("Cannot stream more than one completion")
 
         # create generation parameters
-        if r.top_p == 0:
-            r.top_p = 2e-4
-        if r.top_p == 1:
-            r.top_p = 0.9999999
-        if r.temperature == 0:
-            r.temperature = 2e-4
+        if request.top_p == 0:
+            request.top_p = 2e-4
+        if request.top_p == 1:
+            request.top_p = 0.9999999
+        if request.temperature == 0:
+            request.temperature = 2e-4
 
         gen_kwargs = {
             "do_sample": True,
             "return_full_text": False,
-            "max_new_tokens": r.max_tokens,
-            "top_p": float(r.top_p),
-            "temperature": float(r.temperature),
+            "max_new_tokens": request.max_tokens,
+            "top_p": float(request.top_p),
+            "temperature": float(request.temperature),
             "stop_sequences": stop,
-            "repetition_penalty": r.frequency_penalty,
-            "top_k": r.top_k,
+            "repetition_penalty": request.frequency_penalty,
+            "top_k": request.top_k,
             "seed": seed,
         }
         logger.debug(f"Generation parameters:\n{gen_kwargs}")
 
-        if r.stream:
-            return stream_chat_request(client, prompt, stop, gen_kwargs, r.model)
+        if request.stream:
+            return stream_chat_request(client, prompt, stop, gen_kwargs, request.model)
         else:
             choices = []
             generated_tokens = 0
-            for _i in range(r.n):
+            for _i in range(request.n):
                 res = client.text_generation(
                     prompt,
                     details=True,
                     **gen_kwargs,
                 )
                 parsed = ChatCompletionResponseChoice(
                     index=_i,
                     message=ChatMessage(role="assistant", content=res.generated_text),
                     finish_reason=res.details.finish_reason.value,
                 )
                 generated_tokens += res.details.generated_tokens
                 choices.append(parsed)
                 logger.debug(f"Response at index {_i}:\n{parsed}")
-            # calcuate usage details
+            # calculate usage details
             # TODO: fix when details is fixed
             prompt_tokens = int(len(prompt) / 4)
             total_tokens = prompt_tokens + generated_tokens
 
             return ChatCompletionResponse(
-                model=r.model,
+                model=request.model,
                 choices=choices,
                 usage=Usage(
                     prompt_tokens=prompt_tokens, completion_tokens=generated_tokens, total_tokens=total_tokens
                 ),
             ).model_dump(exclude_none=True)
 
     @classmethod
@@ -215,121 +253,165 @@
             model=model,
             choices=[CompletionResponseStreamChoice(index=0, text=chunk.token.text, logprobs=chunk.token.logprob)],
         ).model_dump(exclude_none=True)
 
 
 class Completion:
     @staticmethod
-    def create(**kwargs) -> Dict[str, Any]:
+    def create(
+        prompt: Union[str, List[Any]],
+        model: Optional[str] = None,
+        suffix: Optional[str] = None,
+        temperature: float = 0.9,
+        top_p: float = 0.6,
+        top_k: Optional[int] = 10,
+        n: int = 1,
+        max_tokens: int = 1024,
+        stop: Optional[List[str]] = None,
+        stream: bool = False,
+        frequency_penalty: Optional[float] = 1.0,
+        logprobs: bool = False,
+        echo: bool = False,
+        debug: bool = False,
+    ) -> Dict[str, Any]:
         """
         Creates a new completion for the provided prompt and parameters.
+
         Args:
-            param1 (int): The first parameter.
-            param2 (Optional[str]): The second parameter. Defaults to None.
+            prompt (`Union[str, List[Any]]`) Text to use for the completion, if `prompt_builder` is set,
+                prompt will be formatted with the `prompt_builder`.
+            model (`str`, *optional*, defaults to None) The model to use for the completion. If not provided,
+                defaults to the base url.
+            suffix (`str`, *optional*, defaults to None) If defined, append this suffix to the prompt.
+            temperature (`float`, defaults to 0.9): The temperature to use for the completion.
+            top_p (`float`, defaults to 0.6): The top_p to use for the completion.
+            top_k (`int`, *optional*, defaults to 10): The top_k to use for the completion.
+            n (`int`, defaults to 1): The number of completions to generate.
+            max_tokens (`int`, defaults to 1024): The maximum number of tokens to generate.
+            stop (`List[str]`, *optional*, defaults to None): The stop sequence(s) to use for the completion.
+            stream (`bool`, defaults to False): Whether to stream the completion.
+            frequency_penalty (`float`, *optional*, defaults to 1.0): The frequency penalty to use for the completion.
+            logprobs (`bool`, defaults to False) Weather to return logprobs.
+            echo (`bool`, defaults to False) Whether to echo the prompt.
+            debug (`bool`, defaults to False): Whether to enable debug logging.
 
         Tip: Prompt builder
             Make sure to always use a prompt builder for your model.
         """
-        # deserialize the request
-        debug = kwargs.pop("debug", False)
         if debug:
             logger.setLevel(logging.DEBUG)
 
-        r = CompletionRequest(**kwargs)
+        request = CompletionRequest(
+            model=model,
+            prompt=prompt,
+            suffix=suffix,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            n=n,
+            max_tokens=max_tokens,
+            stop=stop,
+            stream=stream,
+            frequency_penalty=frequency_penalty,
+            logprobs=logprobs,
+            echo=echo,
+        )
 
         # include suffix if it exists
-        if r.suffix is not None:
-            r.prompt = r.prompt + r.suffix
+        if request.suffix is not None:
+            request.prompt = request.prompt + request.suffix
 
         if prompt_builder is None:
             logging.warn(
                 f"""huggingface.prompt_builder is not set.
 Using default prompt builder for. Prompt sent to model will be:
 ----------------------------------------
-{buildBasePrompt(r.prompt)}.
+{buildBasePrompt(request.prompt)}.
 ----------------------------------------
 If you want to use a custom prompt builder, set huggingface.prompt_builder to a function that takes a list of messages and returns a string.
 You can also use existing prompt builders by importing them from easyllm.prompt_utils"""
             )
-            prompt = buildBasePrompt(r.prompt)
+            prompt = buildBasePrompt(request.prompt)
         else:
-            prompt = prompt_builder(r.prompt)
+            prompt = build_prompt(request.prompt, prompt_builder)
         logger.debug(f"Prompt sent to model will be:\n{prompt}")
 
         # if the model is a url, use it directly
-        if r.model:
-            url = f"{api_base}/{r.model}"
+        if request.model:
+            url = f"{api_base}/{request.model}"
             logger.debug(f"Url:\n{url}")
+        else:
+            url = api_base
 
         # create the client
         client = InferenceClient(url, token=api_key)
 
         # create stop sequences
-        if isinstance(r.stop, list):
-            stop = stop_sequences + r.stop
-        if isinstance(r.stop, str):
-            stop = stop_sequences + [r.stop]
+        if isinstance(request.stop, list):
+            stop = stop_sequences + request.stop
+        if isinstance(request.stop, str):
+            stop = stop_sequences + [request.stop]
         else:
             stop = stop_sequences
         logger.debug(f"Stop sequences:\n{stop}")
 
         # check if we can stream
-        if r.stream is True and r.n > 1:
+        if request.stream is True and request.n > 1:
             raise ValueError("Cannot stream more than one completion")
 
         # create generation parameters
-        if r.top_p == 0:
-            r.top_p = 2e-4
-        if r.top_p == 1:
-            r.top_p = 0.9999999
-        if r.temperature == 0:
-            r.temperature = 2e-4
+        if request.top_p == 0:
+            request.top_p = 2e-4
+        if request.top_p == 1:
+            request.top_p = 0.9999999
+        if request.temperature == 0:
+            request.temperature = 2e-4
 
         gen_kwargs = {
             "do_sample": True,
-            "return_full_text": True if r.echo else False,
-            "max_new_tokens": r.max_tokens,
-            "top_p": float(r.top_p),
-            "temperature": float(r.temperature),
+            "return_full_text": True if request.echo else False,
+            "max_new_tokens": request.max_tokens,
+            "top_p": float(request.top_p),
+            "temperature": float(request.temperature),
             "stop_sequences": stop,
-            "repetition_penalty": r.frequency_penalty,
-            "top_k": r.top_k,
+            "repetition_penalty": request.frequency_penalty,
+            "top_k": request.top_k,
             "seed": seed,
         }
         logger.debug(f"Generation parameters:\n{gen_kwargs}")
 
-        if r.stream:
-            return stream_completion_request(client, prompt, stop, gen_kwargs, r.model)
+        if request.stream:
+            return stream_completion_request(client, prompt, stop, gen_kwargs, request.model)
         else:
             choices = []
             generated_tokens = 0
-            for _i in range(r.n):
+            for _i in range(request.n):
                 res = client.text_generation(
                     prompt,
                     details=True,
                     **gen_kwargs,
                 )
                 parsed = CompletionResponseChoice(
                     index=_i,
                     text=res.generated_text,
                     finish_reason=res.details.finish_reason.value,
                 )
-                if r.logprobs:
+                if request.logprobs:
                     parsed.logprobs = res.details.tokens
 
                 generated_tokens += res.details.generated_tokens
                 choices.append(parsed)
                 logger.debug(f"Response at index {_i}:\n{parsed}")
             # calcuate usage details
             # TODO: fix when details is fixed
             prompt_tokens = int(len(prompt) / 4)
             total_tokens = prompt_tokens + generated_tokens
 
             return CompletionResponse(
-                model=r.model,
+                model=request.model,
                 choices=choices,
                 usage=Usage(
                     prompt_tokens=prompt_tokens, completion_tokens=generated_tokens, total_tokens=total_tokens
                 ),
             ).model_dump(exclude_none=True)
 
     @classmethod
@@ -338,60 +420,67 @@
         Creates a new chat completion for the provided messages and parameters.
         """
         raise NotImplementedError("ChatCompletion.acreate is not implemented")
 
 
 class Embedding:
     @staticmethod
-    def create(**kwargs) -> Dict[str, Any]:
+    def create(
+        input: Union[str, List[Any]],
+        model: Optional[str] = None,
+        debug: bool = False,
+    ) -> Dict[str, Any]:
         """
         Creates a new embeddings for the provided prompt and parameters.
+
         Args:
-            param1 (int): The first parameter.
-            param2 (Optional[str]): The second parameter. Defaults to None.
+            input (`Union[str, List[Any]]`) document(s) to embed.
+            model (`str`, *optional*, defaults to None) The model to use for the completion. If not provided,
+                defaults to the base url.
+            debug (`bool`, defaults to False): Whether to enable debug logging.
 
         Tip: Prompt builder
             Make sure to always use a prompt builder for your model.
         """
-        # deserialize the request
-        debug = kwargs.pop("debug", False)
         if debug:
             logger.setLevel(logging.DEBUG)
 
-        r = EmbeddingsRequest(**kwargs)
+        request = EmbeddingsRequest(model=model, input=input)
 
         # if the model is a url, use it directly
-        if r.model:
+        if request.model:
             if api_base.endswith("/models"):
-                url = f"{api_base.replace('/models', '/pipeline/feature-extraction')}/{r.model}"
+                url = f"{api_base.replace('/models', '/pipeline/feature-extraction')}/{request.model}"
             else:
-                url = f"{api_base}/{r.model}"
+                url = f"{api_base}/{request.model}"
             logger.debug(f"Url:\n{url}")
+        else:
+            url = api_base
 
         # create the client
         client = InferenceClient(url, token=api_key)
 
         # client is currently not supporting batched request thats why we run sequentially
         emb = []
-        res = client.post(json={"inputs": r.input, "model": r.model, "task": "feature-extraction"})
+        res = client.post(json={"inputs": request.input, "model": request.model, "task": "feature-extraction"})
         parsed_res = json.loads(res.decode())
-        if isinstance(r.input, list):
+        if isinstance(request.input, list):
             for idx, i in enumerate(parsed_res):
                 emb.append(EmbeddingsObjectResponse(index=idx, embedding=i))
         else:
             emb.append(EmbeddingsObjectResponse(index=0, embedding=parsed_res))
 
         if isinstance(res, list):
             # TODO: only approximating tokens
-            tokens = [int(len(i) / 4) for i in r.input]
+            tokens = [int(len(i) / 4) for i in request.input]
         else:
-            tokens = int(len(r.input) / 4)
+            tokens = int(len(request.input) / 4)
 
         return EmbeddingsResponse(
-            model=r.model,
+            model=request.model,
             data=emb,
             usage=Usage(prompt_tokens=tokens, total_tokens=tokens),
         ).model_dump(exclude_none=True)
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         """
```

### Comparing `easyllm-0.2.0/easyllm/prompt_utils/llama2.py` & `easyllm-0.3.0/easyllm/prompt_utils/llama2.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.2.0/easyllm/schema/openai.py` & `easyllm-0.3.0/easyllm/schema/openai.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 
 
 # More documentation https://platform.openai.com/docs/api-reference/chat/create
 # adapted from https://github.com/lm-sys/FastChat/blob/main/fastchat/protocol/openai_api_protocol.py
 class ChatCompletionRequest(BaseModel):
     messages: List[ChatMessage]
     model: Optional[str] = None
-    temperature: Optional[float] = 0.9
-    top_p: Optional[float] = 0.6
+    temperature: float = 0.9
+    top_p: float = 0.6
     top_k: Optional[int] = 10
-    n: Optional[int] = 1
-    max_tokens: Optional[int] = 1024
+    n: int = 1
+    max_tokens: int = 1024
     stop: Optional[List[str]] = None
-    stream: Optional[bool] = False
+    stream: bool = False
     frequency_penalty: Optional[float] = 1.0
     user: Optional[str] = None
 
 
 class ChatCompletionResponseChoice(BaseModel):
     index: int
     message: ChatMessage
     finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
 
 
 class ChatCompletionResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
-    model: str
+    model: Optional[str] = "custom"
     choices: List[ChatCompletionResponseChoice]
     usage: Usage
 
 
 class DeltaMessage(BaseModel):
     role: Optional[str] = None
     content: Optional[str] = None
@@ -49,48 +49,47 @@
     finish_reason: Optional[Literal["stop", "length"]] = None
 
 
 class ChatCompletionStreamResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "chat.completion.chunk"
     created: int = Field(default_factory=lambda: int(time.time()))
-    model: str
+    model: Optional[str] = None
     choices: List[ChatCompletionResponseStreamChoice]
 
 
 class CompletionRequest(BaseModel):
-    model: str
+    model: Optional[str] = None
     prompt: Union[str, List[Any]]
     suffix: Optional[str] = None
-    temperature: Optional[float] = 0.9
-    top_p: Optional[float] = 0.6
+    temperature: float = 0.9
+    top_p: float = 0.6
     top_k: Optional[int] = 10
-    n: Optional[int] = 1
-    max_tokens: Optional[int] = 1024
+    n: int = 1
+    max_tokens: int = 1024
     stop: Optional[List[str]] = None
-    stream: Optional[bool] = False
+    stream: bool = False
     frequency_penalty: Optional[float] = 1.0
     user: Optional[str] = None
-    logprobs: Optional[bool] = None
-    echo: Optional[bool] = False
-    user: Optional[str] = None
+    logprobs: bool = False
+    echo: bool = False
 
 
 class CompletionResponseChoice(BaseModel):
     index: int
     text: str
     logprobs: Union[Optional[List[Dict[str, Any]]], float] = None
     finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
 
 
 class CompletionResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "text.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
-    model: str
+    model: Optional[str] = "custom"
     choices: List[CompletionResponseChoice]
     usage: Usage
 
 
 class CompletionResponseStreamChoice(BaseModel):
     index: int
     text: str
@@ -98,15 +97,15 @@
     finish_reason: Optional[Literal["stop_sequence", "length", "eos_token"]] = None
 
 
 class CompletionStreamResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"hf-{generate(size=10)}")
     object: str = "text.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
-    model: str
+    model: Optional[str] = "custom"
     choices: List[CompletionResponseStreamChoice]
 
 
 class EmbeddingsRequest(BaseModel):
     model: Optional[str] = None
     input: Union[str, List[Any]]
     user: Optional[str] = None
@@ -117,9 +116,9 @@
     object: str = "embedding"
     embedding: List[float]
 
 
 class EmbeddingsResponse(BaseModel):
     object: str = "list"
     data: List[EmbeddingsObjectResponse]
-    model: str
+    model: Optional[str] = "custom"
     usage: Usage
```

### Comparing `easyllm-0.2.0/notebooks/chat-completion-api.ipynb` & `easyllm-0.3.0/notebooks/chat-completion-api.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946871227350257%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# How to use Chat Completion clients\\n'), (2, 'EasyLLM "*

 * *            'can be used as an abstract layer to replace `gpt-3.5-turbo` and `gpt-4` with open '*

 * *            "source models.\\n')], delete: [2, 0]}}, 4: {'source': {insert: [(8, 'Compared to "*

 * *            'OpenAI api is the `huggingface` module also exposing a `prompt_builder` and '*

 * *            '`stop_sequences` parameter you can use to customize the prompt and stop sequences. '*

 * *            "The EasyLLM pack […]*

```diff
@@ -1,17 +1,17 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# How to format inputs to Chat models\n",
+                "# How to use Chat Completion clients\n",
                 "\n",
-                "Easyllm can be used as an abstract layer to replace `gpt-3.5-turbo` and `gpt-4` with open source models.\n",
+                "EasyLLM can be used as an abstract layer to replace `gpt-3.5-turbo` and `gpt-4` with open source models.\n",
                 "\n",
                 "You can change your own applications from the OpenAI API, by simply changing the client. \n",
                 "\n",
                 "Chat models take a series of messages as input, and return an AI-written message as output.\n",
                 "\n",
                 "This guide illustrates the chat format with a few example API calls."
             ]
@@ -53,60 +53,64 @@
                 "\n",
                 "A chat API call has two required inputs:\n",
                 "- `model`: the name of the model you want to use (e.g., `meta-llama/Llama-2-70b-chat-hf`) or leave it empty to just call the api\n",
                 "- `messages`: a list of message objects, where each object has two required fields:\n",
                 "    - `role`: the role of the messenger (either `system`, `user`, or `assistant`)\n",
                 "    - `content`: the content of the message (e.g., `Write me a beautiful poem`)\n",
                 "\n",
-                "Compared to OpenAI api is the `huggingface` module also exposing a `prompt_builder` and `stop_sequences` parameter you can use to customize the prompt and stop sequences. The EasyLLM package comes with build in popular methods for both of these parameters, e.g. `llama2_prompt_builder` and `llama2_stop_sequences`. \n",
+                "Compared to OpenAI api is the `huggingface` module also exposing a `prompt_builder` and `stop_sequences` parameter you can use to customize the prompt and stop sequences. The EasyLLM package comes with prompt builder utilities.\n",
                 "\n",
                 "Let's look at an example chat API calls to see how the chat format works in practice."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'id': 'hf-VH-mBO0hVT',\n",
+                            "{'id': 'hf-5sljhaJk2y',\n",
                             " 'object': 'chat.completion',\n",
-                            " 'created': 1690987326,\n",
+                            " 'created': 1691129787,\n",
                             " 'model': 'meta-llama/Llama-2-70b-chat-hf',\n",
                             " 'choices': [{'index': 0,\n",
-                            "   'message': {'role': 'assistant', 'content': ' Apple who?'},\n",
+                            "   'message': {'role': 'assistant', 'content': ' Cat who?'},\n",
                             "   'finish_reason': 'eos_token'}],\n",
                             " 'usage': {'prompt_tokens': 149, 'completion_tokens': 5, 'total_tokens': 154}}"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "import os \n",
+                "# set env for prompt builder\n",
+                "os.environ[\"HUGGINGFACE_PROMPT\"] = \"llama2\" # vicuna, wizardlm, stablebeluga, open_assistant\n",
+                "# os.environ[\"HUGGINGFACE_TOKEN\"] = \"hf_xxx\" \n",
                 "\n",
                 "from easyllm.clients import huggingface\n",
-                "from easyllm.prompt_utils import llama2_stop_sequences, build_llama2_prompt\n",
-                "# Example EasyLLM Python library request\n",
-                "MODEL = \"meta-llama/Llama-2-70b-chat-hf\"\n",
-                "huggingface.prompt_builder = build_llama2_prompt\n",
                 "\n",
-                "# The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.\n",
+                "# Changing configuration without using environment variables\n",
                 "# huggingface.api_key=\"hf_xxx\"\n",
+                "# huggingface.prompt_builder = \"llama2\"\n",
+                "\n",
+                "\n",
+                "MODEL=\"meta-llama/Llama-2-70b-chat-hf\"\n",
                 "\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
                 "    messages=[\n",
                 "        {\"role\": \"system\", \"content\": \"\\nYou are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\\n\\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.\"},\n",
                 "        {\"role\": \"user\", \"content\": \"Knock knock.\"},\n",
                 "        {\"role\": \"assistant\", \"content\": \"Who's there?\"},\n",
-                "        {\"role\": \"user\", \"content\": \"Apple.\"},\n",
+                "        {\"role\": \"user\", \"content\": \"Cat.\"},\n",
                 "    ],\n",
                 "      temperature=0.9,\n",
                 "      top_p=0.6,\n",
                 "      max_tokens=1024,\n",
                 ")\n",
                 "response"
             ]
@@ -134,22 +138,22 @@
             "metadata": {},
             "source": [
                 "Extract just the reply with:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        " Apple who?\n"
+                        " Cat who?\n"
                     ]
                 }
             ],
             "source": [
                 "print(response['choices'][0]['message']['content'])"
             ]
         },
@@ -161,52 +165,45 @@
                 "Even non-conversation-based tasks can fit into the chat format, by placing the instruction in the first user message.\n",
                 "\n",
                 "For example, to ask the model to explain asynchronous programming in the style of the pirate Blackbeard, we can structure conversation as follows:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " Hello, my dear students! Today, we're going to learn about a fascinating topic that will help us understand how to make our programs more efficient and responsive: asynchronous programming.\n",
                         "\n",
-                        "Imagine you're working on a project with your classmates, and you need to finish a task, but you're waiting for someone else to finish their part first. You can't start your work until they're done, but you don't want to just sit there twiddling your thumbs. That's where asynchronous programming comes in!\n",
+                        "Imagine you're working on a project with a group of people, and you need to finish your part before others can start theirs. But, you're waiting for someone else to finish their part so you can start yours. This is similar to how asynchronous programming works.\n",
                         "\n",
-                        "Asynchronous programming is like working on a project with your classmates, but instead of waiting for them to finish, you can start working on something else in the meantime. You can think of it like this:\n",
+                        "In asynchronous programming, we break down a program into smaller parts called \"tasks.\" These tasks can run independently, without blocking other tasks from running. This means that if one task is waiting for something to happen, like a response from a server or a user input, other tasks can keep running in the meantime.\n",
                         "\n",
-                        "1. You give a task to your classmate, and they start working on it.\n",
-                        "2. While they're working, you start working on another task that doesn't depend on their work.\n",
-                        "3. When your classmate finishes their task, they give it back to you, and you can continue working on your task.\n",
+                        "Let's use a simple example to illustrate this. Imagine you're making a sandwich. You need to put the bread slices together, add the filling, and then put the sandwich in the fridge to chill. But, you can't start making the sandwich until the bread is toasted, and you can't put the sandwich in the fridge until it's assembled.\n",
                         "\n",
-                        "This way, you can work on multiple tasks simultaneously, and you don't have to wait for each other to finish before moving on to the next step. It's like having multiple people working on a project at the same time, but they're all working on different parts of it.\n",
+                        "In this scenario, toasting the bread and assembling the sandwich are two separate tasks. If we were to do them synchronously, we would do them one after the other, like this:\n",
                         "\n",
-                        "Now, let's see how this works in programming. Imagine you're building a website, and you want to load some data from an API. You can't start building the website until the data is loaded, but you don't want to wait for the data to be loaded before you start building the website. That's where asynchronous programming comes in!\n",
+                        "1. Toast the bread\n",
+                        "2. Assemble the sandwich\n",
+                        "3. Put the sandwich in the fridge\n",
                         "\n",
-                        "You can use a special function called a \"callback\" to handle this situation. A callback is like a homework assignment that you give to a classmate. You give them the assignment, and they work on it. When they're done, they give it back to you, and you can continue working on your project.\n",
+                        "But, with asynchronous programming, we can do them simultaneously, like this:\n",
                         "\n",
-                        "Here's an example of how this might look in code:\n",
-                        "```\n",
-                        "// Give the homework assignment (callback) to the API\n",
-                        "fetchDataFromApi(callback);\n",
+                        "1. Toast the bread (starts)\n",
+                        "2. Assemble the sandwich (starts)\n",
+                        "3. Toast the bread (finishes)\n",
+                        "4. Put the sandwich in the fridge\n",
                         "\n",
-                        "// Start working on the website while waiting for the data to be loaded\n",
-                        "buildWebsite();\n",
+                        "By doing tasks simultaneously, we can save time and make our program more efficient. But, we need to be careful not to get confused about the order in which things happen. That's why we use special tools, like \"promises\" and \"callbacks,\" to keep track of everything.\n",
                         "\n",
-                        "// When the data is loaded, continue working on the website\n",
-                        "function callback(data) {\n",
-                        "  // Use the data to finish building the website\n",
-                        "  buildWebsiteWithData(data);\n",
-                        "}\n",
-                        "```\n",
-                        "Asynchronous programming can be a bit tricky to wrap your head around at first, but once you understand the concept, it's a powerful tool for building efficient and responsive programs. So, keep practicing, and soon you'll be a master of asynchronous programming!\n"
+                        "So, my dear students, I hope this helps you understand asynchronous programming a bit better. Remember, it's all about breaking down a program into smaller, independent tasks that can run simultaneously, making our programs more efficient and responsive. Now, go forth and create some amazing programs!\n"
                     ]
                 }
             ],
             "source": [
                 "# example with a system message\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
@@ -217,46 +214,46 @@
                 ")\n",
                 "\n",
                 "print(response['choices'][0]['message']['content'])\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
                         "<s>[INST] Explain asynchronous programming in the style of the pirate Blackbeard. [/INST]\n",
-                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Url:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Url:\n",
                         "https://api-inference.huggingface.co/models/meta-llama/Llama-2-70b-chat-hf\n",
-                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Stop sequences:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Stop sequences:\n",
                         "[]\n",
-                        "08/02/2023 16:42:33 - DEBUG - easyllm.utils - Generation parameters:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Generation parameters:\n",
                         "{'do_sample': True, 'return_full_text': False, 'max_new_tokens': 1024, 'top_p': 0.6, 'temperature': 0.9, 'stop_sequences': [], 'repetition_penalty': 1.0, 'top_k': 10, 'seed': 42}\n",
-                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Response at index 0:\n",
-                        "index=0 message=ChatMessage(role='assistant', content=\" Ahoy matey! Yer lookin' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o' grog and listen close, for Blackbeard's got a story fer ye.\\n\\nAsynchronous programming, me hearty, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the rocks and shoals that'll sink ye ship if ye ain't careful.\\n\\nImagine ye're sailin' along, and ye need to send a message to another ship, say, to arrange a meetin' at the next port o' call. Now, ye could just shout out the message and hope the other ship hears ye, but that be a risky business. The wind and the waves might carry yer words away, and the other ship might not hear ye at all.\\n\\nOr, ye could use a bit o' magic, like a bottle with a message inside, and throw it into the sea. The currents and the tides'll carry it to the other ship, and they'll find it when they least expect it. That be asynchronous programming, me hearty!\\n\\nYe see, when ye send a message, ye don't know when it'll arrive, or even if it'll arrive at all. It's like sendin' a ship's boy up the riggin' to fetch a sail that's stuck. Ye don't know when he'll get there, but ye trust that he'll do his best to fetch it down.\\n\\nAnd that's where the magic comes in, me hearty. Ye gotta have faith that the message'll get there, and that the other ship'll receive it in good time. And while ye wait, ye can keep sailin' on, doin' other tasks, like fixin' the riggin' or swabbin' the decks.\\n\\nNow, there be times when the message don't arrive at all, or it arrives too late. That be like a storm blowin' in, and ye gotta adjust yer sails to keep the ship afloat. But that's the way o' the sea, me hearty. Ye gotta be ready fer anythin', and keep yer wits about ye at all times.\\n\\nSo there ye have it, me hearty. Asynchronous programming be like sailin' the high seas, with a bit o' magic and a lot o' faith. Keep yer wits about ye, and ye'll navigate the treacherous waters like a seasoned pirate! Arrr!\") finish_reason='eos_token'\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Response at index 0:\n",
+                        "index=0 message=ChatMessage(role='assistant', content=' Ahoy matey! Yer lookin\\' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o\\' grog and listen close, for Blackbeard\\'s got a story fer ye.\\n\\nAsynchronous programming, me hearties, be like sailin\\' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the hidden dangers that lie beneath the surface.\\n\\nImagine ye\\'re sailin\\' along, and suddenly, out o\\' the blue, a great storm brews up. The winds howl, the waves crash, and yer ship takes on water. Now, ye gotta act fast, or ye\\'ll be sent to Davy Jones\\' locker!\\n\\nBut, me hearties, ye can\\'t just abandon ship. Ye gotta batten down the hatches, and ride out the storm. And that\\'s where asynchronous programming comes in.\\n\\nAsynchronous programming be like haulin\\' up the sails, and lettin\\' the wind do the work fer ye. Ye don\\'t have to worry about the details o\\' how the wind\\'s blowin\\', or the waves crashin\\', ye just gotta keep yer ship pointed in the right direction, and let nature take its course.\\n\\nNow, I know what ye\\'re thinkin\\', \"Blackbeard, how do I know when me ship\\'s gonna make it through the storm?\" And that, me hearties, be the beauty o\\' asynchronous programming. Ye don\\'t have to know! Ye just have to trust that the winds o\\' change will carry ye through, and ye\\'ll make it to the other side, all in one piece.\\n\\nBut, me hearties, don\\'t ye be thinkin\\' this be easy. Asynchronous programming be like navigatin\\' through treacherous waters, with a crew o\\' mutinous code, and a hull full o\\' bugs. Ye gotta be prepared fer the unexpected, and have a stout heart, or ye\\'ll be walkin\\' the plank!\\n\\nSo, me hearties, there ye have it. Asynchronous programming in the style o\\' Blackbeard. May the winds o\\' change blow in yer favor, and may yer code always be free o\\' bugs! Arrr!') finish_reason='eos_token'\n",
                         " Ahoy matey! Yer lookin' fer a tale of asynchronous programming, eh? Well, settle yerself down with a pint o' grog and listen close, for Blackbeard's got a story fer ye.\n",
                         "\n",
-                        "Asynchronous programming, me hearty, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the rocks and shoals that'll sink ye ship if ye ain't careful.\n",
+                        "Asynchronous programming, me hearties, be like sailin' a ship through treacherous waters. Ye gotta keep yer wits about ye, and watch out fer the hidden dangers that lie beneath the surface.\n",
                         "\n",
-                        "Imagine ye're sailin' along, and ye need to send a message to another ship, say, to arrange a meetin' at the next port o' call. Now, ye could just shout out the message and hope the other ship hears ye, but that be a risky business. The wind and the waves might carry yer words away, and the other ship might not hear ye at all.\n",
+                        "Imagine ye're sailin' along, and suddenly, out o' the blue, a great storm brews up. The winds howl, the waves crash, and yer ship takes on water. Now, ye gotta act fast, or ye'll be sent to Davy Jones' locker!\n",
                         "\n",
-                        "Or, ye could use a bit o' magic, like a bottle with a message inside, and throw it into the sea. The currents and the tides'll carry it to the other ship, and they'll find it when they least expect it. That be asynchronous programming, me hearty!\n",
+                        "But, me hearties, ye can't just abandon ship. Ye gotta batten down the hatches, and ride out the storm. And that's where asynchronous programming comes in.\n",
                         "\n",
-                        "Ye see, when ye send a message, ye don't know when it'll arrive, or even if it'll arrive at all. It's like sendin' a ship's boy up the riggin' to fetch a sail that's stuck. Ye don't know when he'll get there, but ye trust that he'll do his best to fetch it down.\n",
+                        "Asynchronous programming be like haulin' up the sails, and lettin' the wind do the work fer ye. Ye don't have to worry about the details o' how the wind's blowin', or the waves crashin', ye just gotta keep yer ship pointed in the right direction, and let nature take its course.\n",
                         "\n",
-                        "And that's where the magic comes in, me hearty. Ye gotta have faith that the message'll get there, and that the other ship'll receive it in good time. And while ye wait, ye can keep sailin' on, doin' other tasks, like fixin' the riggin' or swabbin' the decks.\n",
+                        "Now, I know what ye're thinkin', \"Blackbeard, how do I know when me ship's gonna make it through the storm?\" And that, me hearties, be the beauty o' asynchronous programming. Ye don't have to know! Ye just have to trust that the winds o' change will carry ye through, and ye'll make it to the other side, all in one piece.\n",
                         "\n",
-                        "Now, there be times when the message don't arrive at all, or it arrives too late. That be like a storm blowin' in, and ye gotta adjust yer sails to keep the ship afloat. But that's the way o' the sea, me hearty. Ye gotta be ready fer anythin', and keep yer wits about ye at all times.\n",
+                        "But, me hearties, don't ye be thinkin' this be easy. Asynchronous programming be like navigatin' through treacherous waters, with a crew o' mutinous code, and a hull full o' bugs. Ye gotta be prepared fer the unexpected, and have a stout heart, or ye'll be walkin' the plank!\n",
                         "\n",
-                        "So there ye have it, me hearty. Asynchronous programming be like sailin' the high seas, with a bit o' magic and a lot o' faith. Keep yer wits about ye, and ye'll navigate the treacherous waters like a seasoned pirate! Arrr!\n"
+                        "So, me hearties, there ye have it. Asynchronous programming in the style o' Blackbeard. May the winds o' change blow in yer favor, and may yer code always be free o' bugs! Arrr!\n"
                     ]
                 }
             ],
             "source": [
                 "# example without a system message and debug flag on:\n",
                 "response = huggingface.ChatCompletion.create(\n",
                 "    model=MODEL,\n",
@@ -281,34 +278,34 @@
                 "One way to show the model what you want is with faked example messages.\n",
                 "\n",
                 "For example:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Prompt sent to model will be:\n",
                         "<s>[INST] <<SYS>>\n",
                         "You are a helpful, pattern-following assistant.\n",
                         "<</SYS>>\n",
                         "\n",
                         "Help me translate the following corporate jargon into plain English. [/INST] Sure, I'd be happy to!</s><s>[INST] New synergies will help drive top-line growth. [/INST] Things working well together will increase revenue.</s><s>[INST] Let's circle back when we have more bandwidth to touch base on opportunities for increased leverage. [/INST] Let's talk later when we're less busy about how to do better.</s><s>[INST] This late pivot means we don't have time to boil the ocean for the client deliverable. [/INST]\n",
-                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Url:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Url:\n",
                         "https://api-inference.huggingface.co/models/meta-llama/Llama-2-70b-chat-hf\n",
-                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Stop sequences:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Stop sequences:\n",
                         "[]\n",
-                        "08/02/2023 16:42:58 - DEBUG - easyllm.utils - Generation parameters:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Generation parameters:\n",
                         "{'do_sample': True, 'return_full_text': False, 'max_new_tokens': 1024, 'top_p': 0.6, 'temperature': 0.9, 'stop_sequences': [], 'repetition_penalty': 1.0, 'top_k': 10, 'seed': 42}\n",
-                        "08/02/2023 16:42:59 - DEBUG - easyllm.utils - Response at index 0:\n",
+                        "08/04/2023 08:16:57 - DEBUG - easyllm.utils - Response at index 0:\n",
                         "index=0 message=ChatMessage(role='assistant', content=\" We've changed direction too late to do a complete job for the client.\") finish_reason='eos_token'\n",
                         " We've changed direction too late to do a complete job for the client.\n"
                     ]
                 }
             ],
             "source": [
                 "# An example of a faked few-shot conversation to prime the model into translating business jargon to simpler speech\n",
```

### Comparing `easyllm-0.2.0/notebooks/get-embeddings.ipynb` & `easyllm-0.3.0/notebooks/get-embeddings.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999702380952381%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(0, '# import os \\n'), (1, '# "*

 * *            'os.environ["HUGGINGFACE_TOKEN"] = "hf_xxx"  # Use Environment Variable\\n\'), (2, '*

 * *            "'\\n')]}}}"}*

```diff
@@ -62,14 +62,17 @@
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "# import os \n",
+                "# os.environ[\"HUGGINGFACE_TOKEN\"] = \"hf_xxx\"  # Use Environment Variable\n",
+                "\n",
                 "from easyllm.clients import huggingface\n",
                 "\n",
                 "# The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.\n",
                 "# huggingface.api_key=\"hf_xxx\"\n",
                 "\n",
                 "embedding = huggingface.Embedding.create(\n",
                 "    model=\"sentence-transformers/all-MiniLM-L6-v2\",\n",
```

### Comparing `easyllm-0.2.0/notebooks/steam-text-completions.ipynb` & `easyllm-0.3.0/notebooks/stream-text-completions.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967293233082707%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# How to stream Text Completion requests\\n')], delete: "*

 * *            '[0]}}, 3: {\'outputs\': {0: {\'text\': ["{\'id\': \'hf-PokypeK2an\', \'object\': '*

 * *            "'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', "*

 * *            '\'choices\': [{\'index\': 0, \'text\': \' \', \'logprobs\': 0.0}]}\\n", "{\'id\': '*

 * *            "'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': "*

 * *            "'meta-llama/ […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# How to stream completions\n",
+                "# How to stream Text Completion requests\n",
                 "\n",
                 "By default, when you request a completion, the entire completion is generated before being sent back in a single response.\n",
                 "\n",
                 "If you're generating long completions, waiting for the response can take many seconds.\n",
                 "\n",
                 "To get responses sooner, you can 'stream' the completion as it's being generated. This allows you to start printing or processing the beginning of the completion before the full completion is finished.\n",
                 "\n",
@@ -53,219 +53,219 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' Sure', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '!', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' Here', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' it', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' is', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ':', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '\\n', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '\\n', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
-                        "{'id': 'hf-ag7to4gy5M', 'object': 'text.completion', 'created': 1690987194, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n"
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' Sure', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '!', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' Here', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' it', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' is', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ':', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '\\n', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '\\n', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '1', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '2', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '3', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '6', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '7', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '8', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '4', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '9', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ',', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': ' ', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '5', 'logprobs': 0.0}]}\n",
+                        "{'id': 'hf-PokypeK2an', 'object': 'text.completion', 'created': 1691129904, 'model': 'meta-llama/Llama-2-70b-chat-hf', 'choices': [{'index': 0, 'text': '0', 'logprobs': 0.0}]}\n"
                     ]
                 }
             ],
             "source": [
                 "from easyllm.clients import huggingface\n",
-                "from easyllm.prompt_utils import build_llama2_prompt\n",
-                "huggingface.prompt_builder = build_llama2_prompt\n",
+                "\n",
+                "huggingface.prompt_builder = \"llama2\"\n",
                 "\n",
                 "# a ChatCompletion request\n",
                 "response = huggingface.Completion.create(\n",
                 "    model=\"meta-llama/Llama-2-70b-chat-hf\",\n",
                 "    prompt=\"Count to 50, with a comma between each number and no newlines. E.g., 1, 2, 3, ...\",\n",
                 "    stream=True  # this time, we set stream=True\n",
                 ")\n",
@@ -282,29 +282,29 @@
                 "As you can see above, streaming responses have a `text` field which holds the generated tokens. \n",
                 "\n",
                 "Below is an example where we print the generated text as it comes in, and stop when we see a `</s>` token."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "  Sure! Here it is: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10."
                     ]
                 }
             ],
             "source": [
                 "from easyllm.clients import huggingface\n",
-                "from easyllm.prompt_utils import build_llama2_prompt\n",
-                "huggingface.prompt_builder = build_llama2_prompt\n",
+                "\n",
+                "huggingface.prompt_builder = \"llama2\"\n",
                 "\n",
                 "# a ChatCompletion request\n",
                 "response = huggingface.Completion.create(\n",
                 "    model=\"meta-llama/Llama-2-70b-chat-hf\",\n",
                 "    prompt=\"Count to 10, with a comma between each number and no newlines. E.g., 1, 2, 3, ...\",\n",
                 "    stream=True  # this time, we set stream=True\n",
                 ")\n",
```

### Comparing `easyllm-0.2.0/notebooks/text-completion-api.ipynb` & `easyllm-0.3.0/notebooks/text-completion-api.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852503156565657%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# # How to use Text (Instruction) Completion "*

 * *            "clients\\n'), (2, 'EasyLLM can be used as an abstract layer to replace "*

 * *            "`text-davinci-003` with open source models.\\n')], delete: [2, 0]}}, 5: {'outputs': "*

 * *            '{0: {\'data\': {\'text/plain\': {insert: [(0, "{\'id\': \'hf-ZK--Ndk30h\',\\n"), (2, '*

 * *            '" \'created\': 1691129933,\\n"), (5, \'   \\\'text\\\': " The meaning of life is a '*

 * *            'question that has puzzled  […]*

```diff
@@ -1,17 +1,17 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# How to format inputs to Text (Instruction) models\n",
+                "# # How to use Text (Instruction) Completion clients\n",
                 "\n",
-                "Easyllm can be used as an abstract layer to replace `text-davinci-003` with open source models.\n",
+                "EasyLLM can be used as an abstract layer to replace `text-davinci-003` with open source models.\n",
                 "\n",
                 "You can change your own applications from the OpenAI API, by simply changing the client. \n",
                 "\n",
                 "Chat models take a series of messages as input, and return an AI-written message as output.\n",
                 "\n",
                 "This guide illustrates the chat format with a few example API calls."
             ]
@@ -64,36 +64,36 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'id': 'hf-bgZcyBsDW_',\n",
+                            "{'id': 'hf-ZK--Ndk30h',\n",
                             " 'object': 'text.completion',\n",
-                            " 'created': 1690986829,\n",
+                            " 'created': 1691129933,\n",
                             " 'model': 'meta-llama/Llama-2-70b-chat-hf',\n",
                             " 'choices': [{'index': 0,\n",
-                            "   'text': \" The meaning of life is a question that has puzzled philosophers, theologians, and scientists for centuries. There are many different perspectives on what constitutes the meaning of life, and there is no one definitive answer. However, some common themes that people often associate with the meaning of life include:\\n\\n1. Purpose: Having a sense of purpose or direction in life, whether it be through work, relationships, or personal goals.\\n2. Fulfillment: Feeling fulfilled and satisfied with one's experiences and achievements.\\n3. Happiness: Pursuing happiness and well-being, whether through personal relationships, material possessions, or personal growth.\\n4. Legacy: Leaving a lasting impact or legacy, whether through contributions to society, artistic or cultural achievements, or the impact one has on others.\\n5. Spirituality: Connecting with a higher power or a sense of something greater than oneself, whether through religion, meditation, or personal beliefs.\\n6. Personal growth: Continuously learning, growing, and improving oneself.\\n7. Love: Experiencing and expressing love for oneself, others, and the world around us.\\n8. Community: Building and being a part of a community, whether through family, friends, or social connections.\\n9. Contribution: Making a positive impact in the world and contributing to the greater good.\\n10. Meaningful experiences: Having experiences that are meaningful and memorable, whether through travel, personal achievements, or time with loved ones.\\n\\nUltimately, the meaning of life is a deeply personal and subjective question, and what gives meaning and purpose to one person's life may be different for another. It's a question that each person must answer for themselves, and it may change throughout their life as they grow and evolve.\",\n",
+                            "   'text': \" The meaning of life is a question that has puzzled philosophers, theologians, and scientists for centuries. There are many different perspectives on what constitutes the meaning of life, and there is no one definitive answer. However, some common themes that people often associate with the meaning of life include:\\n\\n1. Purpose: Having a sense of purpose or direction in life, whether it be through work, relationships, or personal goals.\\n2. Fulfillment: Feeling fulfilled and satisfied with one's experiences and achievements.\\n3. Happiness: Pursuing happiness and well-being, whether through personal relationships, material possessions, or personal growth.\\n4. Self-actualization: Realizing one's potential and living up to one's capabilities.\\n5. Legacy: Leaving a lasting impact or legacy, whether through contributions to society, artistic or cultural achievements, or impacting the lives of others.\\n6. Spirituality: Connecting with a higher power or a sense of something greater than oneself, and finding meaning and purpose through faith or spiritual practices.\\n7. Love: Finding and experiencing love, whether it be through romantic relationships, friendships, or family.\\n8. Personal growth: Continuously learning, growing, and improving oneself.\\n9. Community: Building and being a part of a community, whether it be through work, volunteering, or social connections.\\n10. Making a difference: Making a positive impact in the world and leaving it a better place than when you arrived.\\n\\nUltimately, the meaning of life is a deeply personal and subjective question, and what gives meaning and purpose to one person's life may be different for another. It's a question that each person must answer for themselves, and it may change throughout their life as they grow and evolve.\",\n",
                             "   'finish_reason': 'eos_token'}],\n",
                             " 'usage': {'prompt_tokens': 11, 'completion_tokens': 406, 'total_tokens': 417}}"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\n",
                 "from easyllm.clients import huggingface\n",
-                "from easyllm.prompt_utils import build_llama2_prompt\n",
+                "\n",
                 "# Example EasyLLM Python library request\n",
                 "MODEL = \"meta-llama/Llama-2-70b-chat-hf\"\n",
-                "huggingface.prompt_builder = build_llama2_prompt\n",
+                "huggingface.prompt_builder = \"llama2\"\n",
                 "\n",
                 "# The module automatically loads the HuggingFace API key from the environment variable HUGGINGFACE_TOKEN or from the HuggingFace CLI configuration file.\n",
                 "# huggingface.api_key=\"hf_xxx\"\n",
                 "\n",
                 "response = huggingface.Completion.create(\n",
                 "    model=MODEL,\n",
                 "    prompt=\"What is the meaning of life?\",\n",
@@ -127,41 +127,48 @@
             "metadata": {},
             "source": [
                 "Extract just the reply with:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " The meaning of life is a question that has puzzled philosophers, theologians, and scientists for centuries. There are many different perspectives on what constitutes the meaning of life, and there is no one definitive answer. However, some common themes that people often associate with the meaning of life include:\n",
                         "\n",
                         "1. Purpose: Having a sense of purpose or direction in life, whether it be through work, relationships, or personal goals.\n",
                         "2. Fulfillment: Feeling fulfilled and satisfied with one's experiences and achievements.\n",
                         "3. Happiness: Pursuing happiness and well-being, whether through personal relationships, material possessions, or personal growth.\n",
-                        "4. Legacy: Leaving a lasting impact or legacy, whether through contributions to society, artistic or cultural achievements, or the impact one has on others.\n",
-                        "5. Spirituality: Connecting with a higher power or a sense of something greater than oneself, whether through religion, meditation, or personal beliefs.\n",
-                        "6. Personal growth: Continuously learning, growing, and improving oneself.\n",
-                        "7. Love: Experiencing and expressing love for oneself, others, and the world around us.\n",
-                        "8. Community: Building and being a part of a community, whether through family, friends, or social connections.\n",
-                        "9. Contribution: Making a positive impact in the world and contributing to the greater good.\n",
-                        "10. Meaningful experiences: Having experiences that are meaningful and memorable, whether through travel, personal achievements, or time with loved ones.\n",
+                        "4. Self-actualization: Realizing one's potential and living up to one's capabilities.\n",
+                        "5. Legacy: Leaving a lasting impact or legacy, whether through contributions to society, artistic or cultural achievements, or impacting the lives of others.\n",
+                        "6. Spirituality: Connecting with a higher power or a sense of something greater than oneself, and finding meaning and purpose through faith or spiritual practices.\n",
+                        "7. Love: Finding and experiencing love, whether it be through romantic relationships, friendships, or family.\n",
+                        "8. Personal growth: Continuously learning, growing, and improving oneself.\n",
+                        "9. Community: Building and being a part of a community, whether it be through work, volunteering, or social connections.\n",
+                        "10. Making a difference: Making a positive impact in the world and leaving it a better place than when you arrived.\n",
                         "\n",
                         "Ultimately, the meaning of life is a deeply personal and subjective question, and what gives meaning and purpose to one person's life may be different for another. It's a question that each person must answer for themselves, and it may change throughout their life as they grow and evolve.\n"
                     ]
                 }
             ],
             "source": [
                 "print(response['choices'][0]['text'])"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "openai",
             "language": "python",
             "name": "python3"
```

### Comparing `easyllm-0.2.0/.gitignore` & `easyllm-0.3.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -124,8 +124,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .ruff_cache
-docs/notebooks/
+docs/examples/*.ipynb
+.vscode
```

### Comparing `easyllm-0.2.0/LICENSE` & `easyllm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyllm-0.2.0/README.md` & `easyllm-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # EasyLLM - 
 
 EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. Get immediataly started or check out the [documentation](https://philschmid.github.io/easyllm/).
 
-EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion` with, for example, `huggingface.ChatCompletion` or `huggingface.Completion`.
+EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion`, `openai.Embedding` with, for example, `huggingface.ChatCompletion`, `huggingface.Completion` or `huggingface.Embedding` by changing one line of code.
+
+### Supported Clients 
+
+* `huggingface` - [HuggingFace](https://huggingface.co/) models
+  * `huggingface.ChatCompletion` - Chat with LLMs
+  * `huggingface.Completion` - Text completion with LLMs
+  * `huggingface.Embedding` - Create embeddings with LLMs
+
+Check out the [Examples](./examples) to get started.
 
 ## 🚀 Getting Started
 
 Install EasyLLM via pip:
 
 ```bash
 pip install easyllm
 ```
 
 Then import and start using the clients:
 
 ```python
 
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
 # helper to build llama2 prompt
-huggingface.prompt_builder = build_llama2_prompt
+huggingface.prompt_builder = "llama2"
 
 response = huggingface.ChatCompletion.create(
     model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "\nYou are a helpful assistant speaking like a pirate. argh!"},
         {"role": "user", "content": "What is the sun?"},
     ],
-      temperature=0.9,
-      top_p=0.6,
-      max_tokens=256,
+    temperature=0.9,
+    top_p=0.6,
+    max_tokens=256,
 )
 
 print(response)
 ```
 the result will look like 
 
 ```bash
@@ -58,33 +66,34 @@
     "completion_tokens": 299,
     "total_tokens": 410
   }
 }
 ```
 
 Check out other examples:
-* [Detailed ChatCompletion Example](examples/chat-completion-api)
-* [Example how to stream chat requests](examples/stream-chat-completion-api)
-* [Example how to stream text requests](examples/stream-text-completion-api)
-* [Detailed Completion Example](examples/text-completion-api)
+* [Detailed ChatCompletion Example](notebooks/chat-completion-api.ipynb)
+* [Example how to stream chat requests](notebooks/stream-chat-completions.ipynb)
+* [Example how to stream text requests](notebooks/stream-text-completions.ipynb)
+* [Detailed Completion Example](notebooks/text-completion-api.ipynb)
+* [Create Embeddings](notebooks/get-embeddings)
 
 See the [documentation](https://philschmid.github.io/easyllm/) for more detailed usage and examples.
 
 ## 💪🏻 Migration from OpenAI to HuggingFace
 
 Migrating from OpenAI to HuggingFace is easy. Just change the import statement and the client you want to use and optionally the prompt builder.
 
 ```diff
--import openai
+- import openai
 + from easyllm.clients import huggingface
-+ huggingface.prompt_builder = build_llama2_prompt
++ huggingface.prompt_builder = "llama2"
 
 
--response = openai.ChatCompletion.create(
-+response = huggingface.ChatCompletion.create(
+- response = openai.ChatCompletion.create(
++ response = huggingface.ChatCompletion.create(
 -    model="gpt-3.5-turbo",
 +    model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Knock knock."},
     ],
 )
@@ -92,15 +101,15 @@
 
 Make sure when you switch your client that your hyperparameters are still valid. For example, `temperature` of GPT-3 might be different than `temperature` of `Llama-2`.
 
 ## ☑️ Key Features
 
 ### 🤝 Compatible Clients
 
-- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`.
+- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`, `openai.Embedding`.
 - Easily switch between different LLMs like `openai.ChatCompletion` and `huggingface.ChatCompletion` by changing one line of code. 
 - Support for streaming of completions, checkout example [How to stream completions](./notebooks/stream-chat-completions.ipynb).
 
 ### ⚙️ Helper Modules ⚙️
 
 - `evol_instruct` (work in progress) - Use evolutionary algorithms create instructions for LLMs.
```

### Comparing `easyllm-0.2.0/pyproject.toml` & `easyllm-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyllm-0.2.0/PKG-INFO` & `easyllm-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyllm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Description
 Project-URL: Documentation, https://github.com/unknown/hatch-demo#readme
 Project-URL: Issues, https://github.com/unknown/hatch-demo/issues
 Project-URL: Source, https://github.com/unknown/hatch-demo
 Author-email: Philipp Schmid <schmidphilipp1995@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -45,43 +45,51 @@
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # EasyLLM - 
 
 EasyLLM is an open source project that provides helpful tools and methods for working with large language models (LLMs), both open source and closed source. Get immediataly started or check out the [documentation](https://philschmid.github.io/easyllm/).
 
-EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion` with, for example, `huggingface.ChatCompletion` or `huggingface.Completion`.
+EasyLLM implements clients that are compatible with OpenAI's Completion API. This means you can easily replace `openai.ChatCompletion`, `openai.Completion`, `openai.Embedding` with, for example, `huggingface.ChatCompletion`, `huggingface.Completion` or `huggingface.Embedding` by changing one line of code.
+
+### Supported Clients 
+
+* `huggingface` - [HuggingFace](https://huggingface.co/) models
+  * `huggingface.ChatCompletion` - Chat with LLMs
+  * `huggingface.Completion` - Text completion with LLMs
+  * `huggingface.Embedding` - Create embeddings with LLMs
+
+Check out the [Examples](./examples) to get started.
 
 ## 🚀 Getting Started
 
 Install EasyLLM via pip:
 
 ```bash
 pip install easyllm
 ```
 
 Then import and start using the clients:
 
 ```python
 
 from easyllm.clients import huggingface
-from easyllm.prompt_utils import build_llama2_prompt
 
 # helper to build llama2 prompt
-huggingface.prompt_builder = build_llama2_prompt
+huggingface.prompt_builder = "llama2"
 
 response = huggingface.ChatCompletion.create(
     model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "\nYou are a helpful assistant speaking like a pirate. argh!"},
         {"role": "user", "content": "What is the sun?"},
     ],
-      temperature=0.9,
-      top_p=0.6,
-      max_tokens=256,
+    temperature=0.9,
+    top_p=0.6,
+    max_tokens=256,
 )
 
 print(response)
 ```
 the result will look like 
 
 ```bash
@@ -105,33 +113,34 @@
     "completion_tokens": 299,
     "total_tokens": 410
   }
 }
 ```
 
 Check out other examples:
-* [Detailed ChatCompletion Example](examples/chat-completion-api)
-* [Example how to stream chat requests](examples/stream-chat-completion-api)
-* [Example how to stream text requests](examples/stream-text-completion-api)
-* [Detailed Completion Example](examples/text-completion-api)
+* [Detailed ChatCompletion Example](notebooks/chat-completion-api.ipynb)
+* [Example how to stream chat requests](notebooks/stream-chat-completions.ipynb)
+* [Example how to stream text requests](notebooks/stream-text-completions.ipynb)
+* [Detailed Completion Example](notebooks/text-completion-api.ipynb)
+* [Create Embeddings](notebooks/get-embeddings)
 
 See the [documentation](https://philschmid.github.io/easyllm/) for more detailed usage and examples.
 
 ## 💪🏻 Migration from OpenAI to HuggingFace
 
 Migrating from OpenAI to HuggingFace is easy. Just change the import statement and the client you want to use and optionally the prompt builder.
 
 ```diff
--import openai
+- import openai
 + from easyllm.clients import huggingface
-+ huggingface.prompt_builder = build_llama2_prompt
++ huggingface.prompt_builder = "llama2"
 
 
--response = openai.ChatCompletion.create(
-+response = huggingface.ChatCompletion.create(
+- response = openai.ChatCompletion.create(
++ response = huggingface.ChatCompletion.create(
 -    model="gpt-3.5-turbo",
 +    model="meta-llama/Llama-2-70b-chat-hf",
     messages=[
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Knock knock."},
     ],
 )
@@ -139,15 +148,15 @@
 
 Make sure when you switch your client that your hyperparameters are still valid. For example, `temperature` of GPT-3 might be different than `temperature` of `Llama-2`.
 
 ## ☑️ Key Features
 
 ### 🤝 Compatible Clients
 
-- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`.
+- Implementation of clients compatible with OpenAI API format of `openai.ChatCompletion`, `openai.Completion`, `openai.Embedding`.
 - Easily switch between different LLMs like `openai.ChatCompletion` and `huggingface.ChatCompletion` by changing one line of code. 
 - Support for streaming of completions, checkout example [How to stream completions](./notebooks/stream-chat-completions.ipynb).
 
 ### ⚙️ Helper Modules ⚙️
 
 - `evol_instruct` (work in progress) - Use evolutionary algorithms create instructions for LLMs.
```

