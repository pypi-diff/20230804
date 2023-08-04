# Comparing `tmp/llmx-0.0.3a0.tar.gz` & `tmp/llmx-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmx-0.0.3a0.tar", last modified: Wed Aug  2 21:25:29 2023, max compression
+gzip compressed data, was "llmx-0.0.5a0.tar", last modified: Fri Aug  4 17:30:02 2023, max compression
```

## Comparing `llmx-0.0.3a0.tar` & `llmx-0.0.5a0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3155 2023-08-02 21:22:10.000000 llmx-0.0.3a0/.gitignore
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.3a0/MANIFEST.in
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4944 2023-08-02 21:25:29.071923 llmx-0.0.3a0/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4405 2023-08-02 21:12:51.000000 llmx-0.0.3a0/README.md
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       52 2023-08-02 20:54:38.000000 llmx-0.0.3a0/llmx/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1286 2023-08-02 01:35:37.000000 llmx-0.0.3a0/llmx/datamodel.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/generators/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       83 2023-08-02 20:55:20.000000 llmx-0.0.3a0/llmx/generators/__init__.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/generators/text/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.3a0/llmx/generators/text/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1024 2023-08-02 14:48:18.000000 llmx-0.0.3a0/llmx/generators/text/base_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2806 2023-08-02 19:51:36.000000 llmx-0.0.3a0/llmx/generators/text/cohere_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8484 2023-08-02 21:08:19.000000 llmx-0.0.3a0/llmx/generators/text/hf_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2679 2023-08-02 20:14:24.000000 llmx-0.0.3a0/llmx/generators/text/openai_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3188 2023-08-02 20:59:05.000000 llmx-0.0.3a0/llmx/generators/text/palm_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1505 2023-08-02 20:54:21.000000 llmx-0.0.3a0/llmx/generators/text/textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2269 2023-08-01 22:45:11.000000 llmx-0.0.3a0/llmx/utils.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-02 21:21:40.000000 llmx-0.0.3a0/llmx/version.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx.egg-info/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4944 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      662 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/SOURCES.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/dependency_links.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/entry_points.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      127 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/requires.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/top_level.txt
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/notebooks/
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/notebooks/research/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.3a0/notebooks/research/travelbenchmark.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     5857 2023-08-02 21:14:31.000000 llmx-0.0.3a0/notebooks/tutorial.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1392 2023-08-02 17:35:12.000000 llmx-0.0.3a0/pyproject.toml
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-02 21:25:29.071923 llmx-0.0.3a0/setup.cfg
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.3a0/setup.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/tests/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1970 2023-08-02 21:19:19.000000 llmx-0.0.3a0/tests/test_generators.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3170 2023-08-03 03:11:18.000000 llmx-0.0.5a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1083 2023-08-04 04:13:34.000000 llmx-0.0.5a0/LICENSE
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.5a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-04 17:30:02.662583 llmx-0.0.5a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4948 2023-08-04 16:57:35.000000 llmx-0.0.5a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      185 2023-08-02 22:29:16.000000 llmx-0.0.5a0/llmx/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1322 2023-08-04 03:49:25.000000 llmx-0.0.5a0/llmx/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx/generators/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      128 2023-08-02 22:29:06.000000 llmx-0.0.5a0/llmx/generators/__init__.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/llmx/generators/text/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.5a0/llmx/generators/text/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1063 2023-08-02 23:44:59.000000 llmx-0.0.5a0/llmx/generators/text/base_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2865 2023-08-02 23:47:07.000000 llmx-0.0.5a0/llmx/generators/text/cohere_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8497 2023-08-02 23:46:52.000000 llmx-0.0.5a0/llmx/generators/text/hf_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2728 2023-08-02 23:46:09.000000 llmx-0.0.5a0/llmx/generators/text/openai_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3599 2023-08-04 04:05:33.000000 llmx-0.0.5a0/llmx/generators/text/palm_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1505 2023-08-02 23:47:30.000000 llmx-0.0.5a0/llmx/generators/text/textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4050 2023-08-04 04:03:40.000000 llmx-0.0.5a0/llmx/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-04 17:22:00.000000 llmx-0.0.5a0/llmx/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      670 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      119 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/top_level.txt
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/notebooks/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/notebooks/research/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.5a0/notebooks/research/travelbenchmark.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3669 2023-08-04 14:18:45.000000 llmx-0.0.5a0/notebooks/tutorial.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1384 2023-08-04 14:14:13.000000 llmx-0.0.5a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-04 17:30:02.662583 llmx-0.0.5a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.5a0/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/tests/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1916 2023-08-04 14:18:02.000000 llmx-0.0.5a0/tests/test_generators.py
```

### Comparing `llmx-0.0.3a0/.gitignore` & `llmx-0.0.5a0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .vscode
 .release.sh
 llmx/generators/cache
 llmx.egg-info
 notebooks/test.ipynb
+notebooks/data
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `llmx-0.0.3a0/PKG-INFO` & `llmx-0.0.5a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: llmx
-Version: 0.0.3a0
-Summary: LLMX: A library for LLM Text Generation
-Author-email: Victor Dibia <victor.dibia@gmail.com>
-Project-URL: Homepage, https://github.com/victordibia/llmx
-Project-URL: Bug Tracker, https://github.com/victordibia/llmx/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: web
-Provides-Extra: transformers
-
 # LLMX - An API for Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
 A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
 
 There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
@@ -40,17 +25,23 @@
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
 
 - **Good Utils (e.g., Caching etc)**: E.g. being able to use caching for faster responses. General policy is that cache is used if config (including messages) is the same. If you want to force a new response, set `use_cache=False` in the `generate` call.
 
 ```python
-response = gen.generate(messages=messages, use_cache=True)
+response = gen.generate(messages=messages, config=TextGeneratorConfig(n=1, use_cache=True))
+```
+
+Output looks like
+
+```text
+
+TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 
-# TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
 Install from pypi. Please use python3.9 or higher.
@@ -68,20 +59,25 @@
 ```
 
 Note that you may want to use the latest version of pip to install this package.
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
-Set your api keys first
+Set your api keys first for each service.
 
 ```bash
 export OPENAI_API_KEY=<your key>
 export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
+
+# for palm ..
+export PALM_SERVICE_ACCOUNT_KEY_FILE= <path to your service account key file>
+export PALM_PROJECT_ID=<your gcp project id>
+export PALM_PROJECT_LOCATION=<your project location>
 ```
 
 ```python
 from llmx import  text_generator as generator
 from llmx.datamodel import TextGenerationConfig
 
 messages =  messages = [
@@ -106,7 +102,22 @@
   - [x] Cohere
   - [x] HuggingFace (local)
 
 ## Caveats
 
 - **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
 - **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
+
+## Citation
+
+If you use this library in your work, please cite:
+
+```bibtex
+@software{victordibiallmx,
+author = {Victor Dibia},
+license = {MIT},
+month =  {10},
+title = {LLMX - An API for Language Models},
+url = {https://github.com/victordibia/llmx},
+year = {2023}
+}
+```
```

### Comparing `llmx-0.0.3a0/llmx/datamodel.py` & `llmx-0.0.5a0/llmx/datamodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     temperature: float = 0.1
     max_tokens: Union[int, None] = None
     top_p: float = 1.0
     top_k: int = 50
     frequency_penalty: float = 0.0
     presence_penalty: float = 0.0
     model_type: str = "openai"
-    model: str = None
-    stop: Union[list[str], str, None] = None 
+    model: Optional[str] = None
+    stop: Union[list[str], str, None] = None
+    use_cache: bool = True
 
     def __post_init__(self):
         self._fields_dict = asdict(self)
 
     def __getitem__(self, key: Union[str, int]) -> Any:
         return self._fields_dict.get(key)
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/base_textgen.py` & `llmx-0.0.5a0/llmx/generators/text/base_textgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from typing import Union
 from diskcache import Cache
 from ...utils import get_user_cache_dir
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...version import APP_NAME
 from abc import ABC, abstractmethod
 
-class BaseTextGenerator(ABC):
+
+class TextGenerator(ABC):
 
     def __init__(self, provider: str = "openai", **kwargs):
         self.provider = provider
         self.model_name = kwargs.get("model_name", "gpt-3.5-turbo")
 
         app_name = APP_NAME
         cache_dir_default = get_user_cache_dir(app_name)
         cache_dir_based_on_model = os.path.join(cache_dir_default, self.provider, self.model_name)
         self.cache_dir = kwargs.get("cache_dir", cache_dir_based_on_model)
         self.cache = Cache(self.cache_dir)
 
     @abstractmethod
     def generate(
-        self, messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
-    ) -> TextGenerationResponse:
+            self, messages: Union[list[dict],
+                                  str],
+            config: TextGenerationConfig = TextGenerationConfig(),
+            **kwargs) -> TextGenerationResponse:
         pass
 
     @abstractmethod
     def count_tokens(self, text) -> int:
-        pass
+        pass
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/cohere_textgen.py` & `llmx-0.0.5a0/llmx/generators/text/cohere_textgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Union
-from .base_textgen import BaseTextGenerator
+from .base_textgen import TextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse, Message
 from ...utils import cache_request, num_tokens_from_messages
 import os
 import cohere
 from dataclasses import asdict
 
 
-class CohereTextGenerator(BaseTextGenerator):
+class CohereTextGenerator(TextGenerator):
     def __init__(
         self,
         api_key: str = os.environ.get("COHERE_API_KEY", None),
         provider: str = "cohere",
         organization: str = None,
     ):
         super().__init__(provider=provider)
@@ -28,17 +28,20 @@
                 prompt += message["content"] + "\n"
             else:
                 prompt += message["role"] + ": " + message["content"] + "\n"
 
         return prompt
 
     def generate(
-        self,  messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
-    ) -> TextGenerationResponse:
-         
+            self, messages: Union[list[dict],
+                                  str],
+            config: TextGenerationConfig = TextGenerationConfig(),
+            **kwargs) -> TextGenerationResponse:
+
+        use_cache = config.use_cache
         messages = self.format_messages(messages)
         self.model_name = config.model
 
         cohere_config = {
             "model": config.model or "command",
             "prompt": messages,
             "max_tokens": config.max_tokens,
@@ -46,15 +49,15 @@
             "k": config.top_k,
             "p": config.top_p,
             "num_generations": config.n,
             "stop_sequences": config.stop,
             "frequency_penalty": config.frequency_penalty,
             "presence_penalty": config.presence_penalty,
         }
- 
+
         cache_key_params = cohere_config | {"messages": messages}
         if use_cache:
             response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
         co_response = self.client.generate(**cohere_config)
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/hf_textgen.py` & `llmx-0.0.5a0/llmx/generators/text/hf_textgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 from dataclasses import asdict, dataclass
 from transformers import (AutoTokenizer, AutoModelForCausalLM, GenerationConfig)
 import torch
 
 
-from .base_textgen import BaseTextGenerator
+from .base_textgen import TextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...utils import cache_request
 
 
 @dataclass
 class DialogueTemplate:
     system: str = None
@@ -84,15 +84,15 @@
                 prompt
                 + f" <<SYS>> {system_prompt} <</SYS>> \n"
                 + other_prompt
                 + "[/INST]"
             )
 
 
-class HFTextGenerator(BaseTextGenerator):
+class HFTextGenerator(TextGenerator):
     def __init__(self, provider: str = "huggingface", device_map=None, **kwargs):
 
         super().__init__(provider=provider)
 
         self.dialogue_type = kwargs.get("dialogue_type", "alpaca")
 
         self.model_name = kwargs.get("model", "TheBloke/gpt4-x-vicuna-13B-HF")
@@ -150,15 +150,16 @@
         # print(instruction)
         return instruction
 
     def generate(
             self, messages: Union[list[dict],
                                   str],
             config: TextGenerationConfig = TextGenerationConfig(),
-            use_cache=True, **kwargs) -> TextGenerationResponse:
+            **kwargs) -> TextGenerationResponse:
+        use_cache = config.use_cache
         config.model = self.model_name
         cache_key_params = {
             **asdict(config),
             **kwargs,
             "messages": messages,
             "dialogue_type": self.dialogue_type}
         if use_cache:
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/openai_textgen.py` & `llmx-0.0.5a0/llmx/generators/text/openai_textgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union
-from .base_textgen import BaseTextGenerator
+from .base_textgen import TextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...utils import cache_request, num_tokens_from_messages
 import os
 import openai
 from dataclasses import asdict
 
 context_lengths = {
@@ -16,15 +16,15 @@
     "gpt-3.5-turbo-0301": 4096,
     "gpt-3.5-turbo-16k": 16384,
     "gpt-3.5-turbo-0613": 4096,
     "gpt-3.5-turbo-16k-0613": 16384,
 }
 
 
-class OpenAITextGenerator(BaseTextGenerator):
+class OpenAITextGenerator(TextGenerator):
     def __init__(
         self,
         api_key: str = os.environ.get("OPENAI_API_KEY", None),
         provider: str = "openai",
         organization: str = None,
     ):
         super().__init__(provider=provider)
@@ -34,40 +34,42 @@
             )
         openai.api_key = api_key
         if organization:
             openai.organization = organization
         self.api_key = api_key
 
     def generate(
-        self,  messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
-    ) -> TextGenerationResponse:
+            self, messages: Union[list[dict],
+                                  str],
+            config: TextGenerationConfig = TextGenerationConfig(),
+            **kwargs) -> TextGenerationResponse:
 
-        model = config.model  or "gpt-3.5-turbo-0301"
+        use_cache = config.use_cache
+        model = config.model or "gpt-3.5-turbo-0301"
         prompt_tokens = num_tokens_from_messages(messages)
         max_tokens = max(context_lengths.get(model, 4096) - prompt_tokens - 10, 200)
 
         oai_config = {
             "model": model,
             "temperature": config.temperature,
             "max_tokens": max_tokens,
             "top_p": config.top_p,
             "frequency_penalty": config.frequency_penalty,
             "presence_penalty": config.presence_penalty,
             "n": config.n,
             "messages": messages,
         }
-         
+
         self.model_name = model
-        cache_key_params = (oai_config) | {"messages": messages} 
+        cache_key_params = (oai_config) | {"messages": messages}
         if use_cache:
             response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
-        
         oai_response = openai.ChatCompletion.create(**oai_config)
 
         response = TextGenerationResponse(
             text=[dict(x.message) for x in oai_response.choices],
             logprobs=[],
             config=oai_config,
             usage=dict(oai_response.usage),
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/palm_textgen.py` & `llmx-0.0.5a0/llmx/generators/text/palm_textgen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from dataclasses import asdict
 import os
 from typing import Union
-import google.generativeai as palm
-from .base_textgen import BaseTextGenerator
+from .base_textgen import TextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse, Message
-from ...utils import cache_request, num_tokens_from_messages
+from ...utils import cache_request, gcp_request, num_tokens_from_messages, get_gcp_credentials
 
 
-class PalmTextGenerator(BaseTextGenerator):
+class PalmTextGenerator(TextGenerator):
     def __init__(
         self,
-        api_key: str = os.environ.get("PALM_API_KEY", None),
+        palm_key_file: str = os.environ.get("PALM_SERVICE_ACCOUNT_KEY_FILE", None),
+        project_id: str = os.environ.get("PALM_PROJECT_ID", None),
+        project_location=os.environ.get("PALM_PROJECT_LOCATION", "us-central1"),
         provider: str = "google",
     ):
         super().__init__(provider=provider)
 
-        if api_key is None:
-            raise ValueError(
-                "Palm API key is not set. Please set the PALM_API_KEY environment variable."
-            )
-
-        palm.configure(api_key=api_key)
-        self.api_key = api_key
+        self.project_id = project_id
+        self.project_location = project_location
+        self.credentials = get_gcp_credentials(palm_key_file)
 
     def format_messages(self, messages):
         palm_messages = []
         system_messages = ""
         for message in messages:
             if message["role"] == "system":
                 system_messages += message["content"] + "\n"
@@ -37,55 +34,68 @@
                 palm_messages.append(palm_message)
         return system_messages, palm_messages
 
     def generate(
             self, messages: Union[list[dict],
                                   str],
             config: TextGenerationConfig = TextGenerationConfig(),
-            use_cache=True, **kwargs) -> TextGenerationResponse:
-        model = config.model or "models/chat-bison-001"
-        self.model_name = model
+            **kwargs) -> TextGenerationResponse:
+
+        use_cache = config.use_cache
+        model = config.model or "codechat-bison"
         system_messages, messages = self.format_messages(messages)
+        self.model_name = model
+
+        api_url = f"https://us-central1-aiplatform.googleapis.com/v1/projects/{self.project_id}/locations/{self.project_location}/publishers/google/models/{model}:predict"
+
+#  'candidateCount': max(1, min(8, config.n)),  # 1 <= n <= 8,
+# 'topP': config.top_p,
+#                 'topK': config.top_k,
+
         palm_config = {
-            "model": model,
-            "context": system_messages,
-            "examples": None,
-            "candidate_count": max(1, min(8, config.n)),  # 1 <= n <= 8
-            "temperature": config.temperature,
-            "top_p": config.top_p,
-            "top_k": config.top_k,
-            "messages": messages,
+            'temperature': config.temperature,
+            'maxOutputTokens': config.max_tokens}
+        palm_payload = {
+            'instances': [
+                {'messages': messages,
+                 'context': system_messages,
+                 'examples': [],
+                 }
+            ],
+            'parameters': palm_config
         }
-        # print("*********", config)
-        cache_key_params = palm_config | {"messages": messages}
+        # print("*********", palm_payload)
+
+        palm_response = gcp_request(
+            url=api_url,
+            body=palm_payload,
+            method="POST",
+            credentials=self.credentials)
+
+        cache_key_params = palm_payload
         if use_cache:
             response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
-        try:
-            palm_response = palm.chat(**palm_config)
-        except Exception as e:
-            raise ValueError(f"Error generating text: {e}")
-
         response_text = [
             Message(
                 role="assistant" if x["author"] == "1" else x["author"],
                 content=x["content"],
             )
-            for x in palm_response.candidates
+            for x in palm_response["predictions"][0]["candidates"]
         ]
 
         response = TextGenerationResponse(
             text=response_text,
             logprobs=[],
             config=palm_config,
             usage={
                 "total_tokens": num_tokens_from_messages(
-                    response_text, model=palm_config["model"]
+                    response_text, model=self.model_name
                 )
             },
         )
 
         cache_request(cache=self.cache, params=(cache_key_params), values=asdict(response))
         return response
```

### Comparing `llmx-0.0.3a0/llmx/generators/text/textgen.py` & `llmx-0.0.5a0/llmx/generators/text/textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.3a0/llmx.egg-info/PKG-INFO` & `llmx-0.0.5a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.3a0
+Version: 0.0.5a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) <year> Adam Veldhousen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
 Project-URL: Homepage, https://github.com/victordibia/llmx
 Project-URL: Bug Tracker, https://github.com/victordibia/llmx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: web
 Provides-Extra: transformers
+License-File: LICENSE
 
 # LLMX - An API for Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
 A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
 
@@ -40,17 +62,23 @@
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
 
 - **Good Utils (e.g., Caching etc)**: E.g. being able to use caching for faster responses. General policy is that cache is used if config (including messages) is the same. If you want to force a new response, set `use_cache=False` in the `generate` call.
 
 ```python
-response = gen.generate(messages=messages, use_cache=True)
+response = gen.generate(messages=messages, config=TextGeneratorConfig(n=1, use_cache=True))
+```
+
+Output looks like
+
+```text
+
+TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 
-# TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
 Install from pypi. Please use python3.9 or higher.
@@ -68,20 +96,25 @@
 ```
 
 Note that you may want to use the latest version of pip to install this package.
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
-Set your api keys first
+Set your api keys first for each service.
 
 ```bash
 export OPENAI_API_KEY=<your key>
 export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
+
+# for palm ..
+export PALM_SERVICE_ACCOUNT_KEY_FILE= <path to your service account key file>
+export PALM_PROJECT_ID=<your gcp project id>
+export PALM_PROJECT_LOCATION=<your project location>
 ```
 
 ```python
 from llmx import  text_generator as generator
 from llmx.datamodel import TextGenerationConfig
 
 messages =  messages = [
@@ -106,7 +139,22 @@
   - [x] Cohere
   - [x] HuggingFace (local)
 
 ## Caveats
 
 - **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
 - **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
+
+## Citation
+
+If you use this library in your work, please cite:
+
+```bibtex
+@software{victordibiallmx,
+author = {Victor Dibia},
+license = {MIT},
+month =  {10},
+title = {LLMX - An API for Language Models},
+url = {https://github.com/victordibia/llmx},
+year = {2023}
+}
+```
```

### Comparing `llmx-0.0.3a0/llmx.egg-info/SOURCES.txt` & `llmx-0.0.5a0/llmx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 llmx/__init__.py
 llmx/datamodel.py
 llmx/utils.py
```

### Comparing `llmx-0.0.3a0/notebooks/research/travelbenchmark.ipynb` & `llmx-0.0.5a0/notebooks/research/travelbenchmark.ipynb`

 * *Files identical despite different names*

### Comparing `llmx-0.0.3a0/pyproject.toml` & `llmx-0.0.5a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 dependencies = [
     "pydantic",
-    "openai", 
-    "google-generativeai",
+    "openai",  
     "tiktoken",
     "diskcache",
     "cohere", 
+    "google.auth"
 ]
 optional-dependencies = {web = ["fastapi", "uvicorn"], transformers = ["transformers[torch]>=4.26"]}
 
 dynamic = ["version"]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `llmx-0.0.3a0/tests/test_generators.py` & `llmx-0.0.5a0/tests/test_generators.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,59 +7,60 @@
 config = TextGenerationConfig(
     n=2,
     temperature=0.4,
     max_tokens=100,
     top_p=1.0,
     top_k=50,
     frequency_penalty=0.0,
-    presence_penalty=0.0
+    presence_penalty=0.0,
+    use_cache=False
 )
 
 messages = [
     {"role": "user",
      "content": "What is the capital of France? Only respond with the exact answer"}]
 
 
 def test_openai():
     openai_gen = generator(provider="openai")
-    openai_response = openai_gen.generate(messages, config=config, use_cache=False)
+    openai_response = openai_gen.generate(messages, config=config)
     answer = openai_response.text[0].content
     print(openai_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(openai_response.text) == 2
 
 
 def test_google():
     google_gen = generator(provider="google")
-    config.model = "models/chat-bison-001"
-    google_response = google_gen.generate(messages, config=config, use_cache=False)
+    config.model = "chat-bison@001"
+    google_response = google_gen.generate(messages, config=config)
     answer = google_response.text[0].content
     print(google_response.text[0].content)
 
     assert ("paris" in answer.lower())
     # assert len(google_response.text) == 2 palm may chose to return 1 or 2 responses
 
 
 def test_cohere():
     cohere_gen = generator(provider="cohere")
     config.model = "command"
-    cohere_response = cohere_gen.generate(messages, config=config, use_cache=False)
+    cohere_response = cohere_gen.generate(messages, config=config)
     answer = cohere_response.text[0].content
     print(cohere_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(cohere_response.text) == 2
 
 
 @pytest.mark.skipif("RUNALL" not in os.environ, reason="takes too long")
 def test_hf_local():
     hf_local_gen = generator(
         provider="hf",
         model="TheBloke/Llama-2-7b-chat-fp16",
         device_map="auto")
-    hf_local_response = hf_local_gen.generate(messages, config=config, use_cache=False)
+    hf_local_response = hf_local_gen.generate(messages, config=config)
     answer = hf_local_response.text[0].content
     print(hf_local_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(hf_local_response.text) == 2
```

