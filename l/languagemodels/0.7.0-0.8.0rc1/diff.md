# Comparing `tmp/languagemodels-0.7.0.tar.gz` & `tmp/languagemodels-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.7.0.tar", last modified: Thu Jul 27 14:47:18 2023, max compression
+gzip compressed data, was "languagemodels-0.8.0rc1.tar", last modified: Fri Aug  4 19:46:21 2023, max compression
```

## Comparing `languagemodels-0.7.0.tar` & `languagemodels-0.8.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.560143 languagemodels-0.7.0/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-07-27 14:47:18.560143 languagemodels-0.7.0/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.556142 languagemodels-0.7.0/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    12249 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9502 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/config.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8157 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10112 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/inference.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3526 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/models.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.560143 languagemodels-0.7.0/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      331 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       47 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-07-27 14:47:18.560143 languagemodels-0.7.0/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      775 2023-07-27 14:43:00.000000 languagemodels-0.7.0/setup.py
+drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)     9977 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/PKG-INFO
+drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/languagemodels/
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)    12249 2023-07-28 16:09:19.000000 languagemodels-0.8.0rc1/languagemodels/__init__.py
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)    10131 2023-08-04 19:35:02.000000 languagemodels-0.8.0rc1/languagemodels/config.py
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)     8157 2023-07-23 12:54:43.000000 languagemodels-0.8.0rc1/languagemodels/embeddings.py
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)    10112 2023-08-04 19:34:11.000000 languagemodels-0.8.0rc1/languagemodels/inference.py
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)     3758 2023-08-04 19:35:02.000000 languagemodels-0.8.0rc1/languagemodels/models.py
+drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/languagemodels.egg-info/
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)     9977 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/PKG-INFO
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)      331 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)        1 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)       47 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/requires.txt
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)       15 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/top_level.txt
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)       38 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/setup.cfg
+-rw-r--r--   0 jncraton  (1000) jncraton  (1000)      778 2023-08-04 19:45:50.000000 languagemodels-0.8.0rc1/setup.py
```

### Comparing `languagemodels-0.7.0/PKG-INFO` & `languagemodels-0.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.7.0
+Version: 0.8.0rc1
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```

### Comparing `languagemodels-0.7.0/languagemodels/__init__.py` & `languagemodels-0.8.0rc1/languagemodels/__init__.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.7.0/languagemodels/config.py` & `languagemodels-0.8.0rc1/languagemodels/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,161 +11,178 @@
 
 # Model list
 # This list is sorted in priority order, with the best models first
 # The best model that fits in the memory bounds and matches the model filter
 # will be selected
 models = [
     {
-        "name": "flan-alpaca-xl-ct2-int8",
+        "name": "flan-alpaca-xl",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "alpaca"],
         "params": 3e9,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",  # HF says apache-2.0, but alpaca is NC
     },
     {
-        "name": "flan-alpaca-gpt4-xl-ct2-int8",
+        "name": "flan-alpaca-gpt4-xl",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "gpt4-alpaca"],
         "params": 3e9,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",  # HF says apache-2.0, but alpaca is NC
     },
     {
-        "name": "flan-t5-xl-ct2-int8",
+        "name": "flan-t5-xl",
         "tuning": "instruct",
         "datasets": ["c4", "flan"],
         "params": 3e9,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
-        "name": "fastchat-t5-3b-v1.0-ct2-int8",
+        "name": "fastchat-t5-3b-v1.0",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "sharegpt"],
         "params": 3e9,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",  # This does use OpenAI-generated data
     },
     {
-        "name": "LaMini-Flan-T5-783M-ct2-int8",
+        "name": "LaMini-Flan-T5-783M",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "lamini"],
         "params": 783e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",
     },
     {
-        "name": "flan-t5-large-ct2-int8",
+        "name": "flan-t5-large",
         "tuning": "instruct",
         "datasets": ["c4", "flan"],
         "params": 783e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
-        "name": "LaMini-Flan-T5-248M-ct2-int8",
+        "name": "LaMini-Flan-T5-248M",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "lamini"],
         "params": 248e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",
     },
     {
-        "name": "flan-alpaca-base-ct2-int8",
+        "name": "flan-alpaca-base",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "alpaca"],
         "params": 248e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",  # HF says apache-2.0, but alpaca is NC
     },
     {
-        "name": "flan-t5-base-ct2-int8",
+        "name": "flan-t5-base",
         "tuning": "instruct",
         "datasets": ["c4", "flan"],
         "params": 248e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
-        "name": "LaMini-Flan-T5-77M-ct2-int8",
+        "name": "LaMini-Flan-T5-77M",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "lamini"],
         "params": 77e6,
+        "backend": "ct2",
         "quantization": "int8",
         "architecture": "encoder-decoder-transformer",
         "license": "cc-by-nc-4.0",
     },
     {
-        "name": "flan-t5-small-ct2-int8",
+        "name": "flan-t5-small",
         "tuning": "instruct",
         "datasets": ["c4", "flan"],
         "params": 77e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
-        "name": "LaMini-GPT-774M-ct2-int8",
+        "name": "LaMini-GPT-774M",
         "tuning": "instruct",
         "datasets": ["webtext", "lamini"],
         "params": 774e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "decoder-only-transformer",
         "license": "mit",
     },
     {
-        "name": "LaMini-GPT-124M-ct2-int8",
+        "name": "LaMini-GPT-124M",
         "tuning": "instruct",
         "datasets": ["webtext", "lamini"],
         "params": 124e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "decoder-only-transformer",
         "license": "mit",
     },
     {
-        "name": "codet5p-770m-py-ct2-int8",
+        "name": "codet5p-770m-py",
         "tuning": "code",
         "datasets": ["github-code"],
         "params": 770e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "bsd-3-clause",
     },
     {
-        "name": "codet5p-220m-py-ct2-int8",
+        "name": "codet5p-220m-py",
         "tuning": "code",
         "datasets": ["github-code"],
         "params": 220e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "bsd-3-clause",
     },
     {
-        "name": "all-MiniLM-L6-v2-ct2-int8",
+        "name": "all-MiniLM-L6-v2",
         "tuning": "embedding",
         "params": 22e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-only-transformer",
         "license": "apache-2.0",
     },
     {
-        "name": "e5-small-v2-ct2-int8",
+        "name": "e5-small-v2",
         "tuning": "embedding",
         "params": 33e6,
         "quantization": "int8",
+        "backend": "ct2",
         "architecture": "encoder-only-transformer",
         "license": "mit",
     },
 ]
 
 
 class Config(dict):
@@ -176,26 +193,26 @@
 
     Only appropriate keys and values are allowed to be set.
 
     >>> c = Config({'max_ram': '4gb'})
     >>> c
     {...'max_ram': 4.0...}
 
-    >>> c = Config({'instruct_model': 'flan-t5-small-ct2-int8'})
+    >>> c = Config({'instruct_model': 'flan-t5-small'})
     >>> c
-    {...'instruct_model': 'flan-t5-small-ct2-int8'...}
+    {...'instruct_model': 'flan-t5-small'...}
 
     >>> c = Config({'model_license': 'apache|mit|bsd'})
     >>> c
     {...'model_license': re.compile('apache|mit|bsd')...}
 
-    >>> c = Config({'instruct_model': 'flan-t5-bad-ct2-int8'})
+    >>> c = Config({'instruct_model': 'flan-t5-bad'})
     Traceback (most recent call last):
       ...
-    KeyError: 'flan-t5-bad-ct2-int8'
+    KeyError: 'flan-t5-bad'
 
     >>> c = Config({'bad_value': 1})
     Traceback (most recent call last):
       ...
     KeyError: 'bad_value'
 
     >>> c = Config()
@@ -226,17 +243,20 @@
     def __setitem__(self, key, value):
         super().__setitem__(key, Config.schema[key].initfn(value))
 
         # Auto-adjust instruct_model when filters change
         if key == "max_ram" or key == "model_license":
             found = set()
             for model in models:
-                assert model["quantization"] == "int8"
-
-                memsize = model["params"] / 1e9
+                if model["quantization"] == "int8":
+                    memsize = model["params"] / 1e9
+                elif model["quantization"] == "q3_k_m":
+                    memsize = model["params"] * 0.48 / 1e9
+                elif model["quantization"] == "q4_k_m":
+                    memsize = model["params"] * 0.59 / 1e9
 
                 sizefit = memsize < self["max_ram"]
 
                 if "model_license" in self:
                     licensematch = self["model_license"].match(model["license"])
                 else:
                     licensematch = True
@@ -253,14 +273,20 @@
             self[key] = other[key]
 
     @staticmethod
     def validate_model(model_name):
         return Config.model_names[model_name]["name"]
 
     @staticmethod
+    def validate_device(device):
+        assert device in ["auto", "cpu"]
+
+        return device
+
+    @staticmethod
     def convert_to_gb(space):
         """Convert max RAM string to int
 
         Output will be in gigabytes
 
         If not specified, input is assumed to be in gigabytes
 
@@ -321,14 +347,15 @@
             return float(space[:-1]) * multipliers[space[-1]]
         else:
             return float(space)
 
 
 Config.schema = {
     "max_ram": ConfigItem(Config.convert_to_gb, 0.48),
+    "device": ConfigItem(Config.validate_device, "cpu"),
     "model_license": ConfigItem(re.compile, ".*"),
-    "instruct_model": ConfigItem(Config.validate_model, "LaMini-Flan-T5-248M-ct2-int8"),
-    "embedding_model": ConfigItem(Config.validate_model, "all-MiniLM-L6-v2-ct2-int8"),
-    "code_model": ConfigItem(Config.validate_model, "codet5p-220m-py-ct2-int8"),
+    "instruct_model": ConfigItem(Config.validate_model, "LaMini-Flan-T5-248M"),
+    "embedding_model": ConfigItem(Config.validate_model, "all-MiniLM-L6-v2"),
+    "code_model": ConfigItem(Config.validate_model, "codet5p-220m-py"),
 }
 
 config = Config()
```

### Comparing `languagemodels-0.7.0/languagemodels/embeddings.py` & `languagemodels-0.8.0rc1/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.7.0/languagemodels/inference.py` & `languagemodels-0.8.0rc1/languagemodels/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def generate_instruct(
     prompt,
     max_tokens=200,
     temperature=0.1,
     topk=1,
-    repetition_penalty=1.2,
+    repetition_penalty=1.3,
     prefix="",
     suppress=[],
 ):
     """Generates one completion for a prompt using an instruction-tuned model
 
     This may use a local model, or it may make an API call to an external
     model if API keys are available.
```

### Comparing `languagemodels-0.7.0/languagemodels/models.py` & `languagemodels-0.8.0rc1/languagemodels/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,55 +13,62 @@
     pass
 
 
 def get_model_info(model_type="instruct"):
     """Gets info about the current model in use
 
     >>> get_model_info('instruct')
-    {'name': 'LaMini-Flan-T5-248M-ct2-int8', 'tuning': 'instruct'...
+    {'name': 'LaMini-Flan-T5-248M', 'tuning': 'instruct'...
     """
     model_name = config[f"{model_type}_model"]
 
     m = [m for m in models if m["name"] == model_name][0]
 
     param_bits = int(re.search(r"\d+", m["quantization"]).group(0))
 
     m["size_gb"] = m["params"] * param_bits / 8 / 1e9
+    m["path"] = f"jncraton/{m['name']}-{m['backend']}-{m['quantization']}"
 
     return m
 
 
 def initialize_tokenizer(model_type, model_name):
-    tok_config = hf_hub_download(f"jncraton/{model_name}", "tokenizer.json")
+    model_info = get_model_info(model_type)
+
+    tok_config = hf_hub_download(model_info["path"], "tokenizer.json")
     tokenizer = Tokenizer.from_file(tok_config)
 
     if model_type == "embedding":
         tokenizer.no_padding()
         tokenizer.no_truncation()
 
     return tokenizer
 
 
 def initialize_model(model_type, model_name):
-    hf_hub_download(f"jncraton/{model_name}", "config.json")
-    model_path = hf_hub_download(f"jncraton/{model_name}", "model.bin")
+    model_info = get_model_info(model_type)
+
+    hf_hub_download(model_info["path"], "config.json")
+    model_path = hf_hub_download(model_info["path"], "model.bin")
     model_base_path = model_path[:-10]
 
-    if model_type == "embedding":
-        hf_hub_download(f"jncraton/{model_name}", "vocabulary.txt")
-        return ctranslate2.Encoder(model_base_path, compute_type="int8", device="auto")
-    elif "gpt" in model_name.lower():
-        hf_hub_download(f"jncraton/{model_name}", "vocabulary.json")
+    if model_info["architecture"] == "encoder-only-transformer":
+        hf_hub_download(model_info["path"], "vocabulary.txt")
+        return ctranslate2.Encoder(
+            model_base_path, compute_type="int8", device=config["device"]
+        )
+    elif model_info["architecture"] == "decoder-only-transformer":
+        hf_hub_download(model_info["path"], "vocabulary.json")
         return ctranslate2.Generator(
-            model_base_path, compute_type="int8", device="auto"
+            model_base_path, compute_type="int8", device=config["device"]
         )
     else:
-        hf_hub_download(f"jncraton/{model_name}", "shared_vocabulary.txt")
+        hf_hub_download(model_info["path"], "shared_vocabulary.txt")
         return ctranslate2.Translator(
-            model_base_path, compute_type="int8", device="auto"
+            model_base_path, compute_type="int8", device=config["device"]
         )
 
 
 def get_model(model_type, tokenizer_only=False):
     """Gets a model from the loaded model cache
 
     If tokenizer_only, the model itself will not be (re)loaded
```

### Comparing `languagemodels-0.7.0/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.8.0rc1/languagemodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.7.0
+Version: 0.8.0rc1
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```

### Comparing `languagemodels-0.7.0/setup.py` & `languagemodels-0.8.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.7.0",
+    version="0.8.0rc1",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

