# Comparing `tmp/openai_functools-1.0.96.tar.gz` & `tmp/openai_functools-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-1.0.96.tar", max compression
+gzip compressed data, was "openai_functools-1.0.97.tar", max compression
```

## Comparing `openai_functools-1.0.96.tar` & `openai_functools-1.0.97.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-08-04 14:21:20.441728 openai_functools-1.0.96/LICENSE
--rw-r--r--   0        0        0     8118 2023-08-04 14:21:20.441728 openai_functools-1.0.96/README.md
--rw-r--r--   0        0        0      342 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/__init__.py
--rw-r--r--   0        0        0      240 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/function_spec.py
--rw-r--r--   0        0        0     6838 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/functions_orchestrator.py
--rw-r--r--   0        0        0     1755 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/types.py
--rw-r--r--   0        0        0       69 2023-08-04 14:21:20.461730 openai_functools-1.0.96/openai_functools/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-08-04 14:21:48.667619 openai_functools-1.0.96/pyproject.toml
--rw-r--r--   0        0        0     8818 1970-01-01 00:00:00.000000 openai_functools-1.0.96/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 14:22:21.333068 openai_functools-1.0.97/LICENSE
+-rw-r--r--   0        0        0     8664 2023-08-04 14:22:21.333068 openai_functools-1.0.97/README.md
+-rw-r--r--   0        0        0      342 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/__init__.py
+-rw-r--r--   0        0        0      240 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/function_spec.py
+-rw-r--r--   0        0        0     7066 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/functions_orchestrator.py
+-rw-r--r--   0        0        0     1755 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/types.py
+-rw-r--r--   0        0        0        0 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/utils/__init__.py
+-rw-r--r--   0        0        0      798 2023-08-04 14:22:21.349068 openai_functools-1.0.97/openai_functools/utils/conversation.py
+-rw-r--r--   0        0        0      538 2023-08-04 14:22:45.965234 openai_functools-1.0.97/pyproject.toml
+-rw-r--r--   0        0        0     9364 1970-01-01 00:00:00.000000 openai_functools-1.0.97/PKG-INFO
```

### Comparing `openai_functools-1.0.96/LICENSE` & `openai_functools-1.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.96/README.md` & `openai_functools-1.0.97/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 "required": ["location"],
             },
         }
     ]
     # Proceed with calling openai, invoking the function using the response, etc..
 ```
 
-### Enhanced Automatic Approach
+### Automated Approach using openai-functools
 
 The `openai-functools` library simplifies the process by automatically generating the necessary JSON structure. You just need to import our package and wrap your function with the `openai_function` decorator. Here's how it works:
 
 ```python
 import json
 from openai_functools import openai_function
 
@@ -123,15 +123,15 @@
 orchestrator = FunctionsOrchestrator()
 orchestrator.register_all([get_current_weather, get_weather_next_day])
 # ...
 ```
 
 #### Registering Functions
 
-Functions can be registered using the `register_all` or `register` method as shown in the code snippet above. `register_all` accepts a list of functions, while `register` is used to register a single function. 
+Functions can be registered using the `register_all` or `register` method as shown in the code snippet above. `register_all` accepts a list of functions, while `register` is used to register a single function.
 
 ### Creating and Using Function Descriptions
 
 Function descriptions are automatically created based on the registered functions using `create_function_descriptions` method. These descriptions can then be passed to the OpenAI `ChatCompletion.create` method.
 
 ```python
 response = openai.ChatCompletion.create(
@@ -168,14 +168,19 @@
 
 Currently, only "reStructuredText" (reST) is supported by default, although this can be extended in the future (feel free to contribute!). Under the hood we make use of [docstring parser](https://pypi.org/project/docstring-parser/) to enable this.
 
 ## Examples
 
 Several examples can be found in the `examples` directory of this repository.
 
+1. The [Maintenance app usecase](./examples/maintenance_app_usecase/) is the recommended example to analyse, it shows the power of the library in a (spoofed) real-world setting.
+1. The [Naive approach example](./examples/naive_approach.py) shows how to call openai-functions without use of the library.
+1. The [Simple example](./examples/simple_example.py) is similar to the naive approach, but makes use our decorator.
+1. The [Orchestrator example](./examples/orchestrator_example.py) shows how one can use the orchestrator class.
+
 ## Contributing
 
 We welcome contributions to `openai-functools`! Please see our [contributing guide](CONTRIBUTING.md) for more details.
 
 ## Support
 
 For support with `openai-functools`, please open an issue on this GitHub repository. We will do our best to assist you.
```

### Comparing `openai_functools-1.0.96/openai_functools/functions_orchestrator.py` & `openai_functools-1.0.97/openai_functools/functions_orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,30 +119,35 @@
         Args:
             openai_response (dict): The OpenAI response containing the function call information.
 
         Returns:
             dict: The responses from the called function.
         """
         response_message = openai_response["choices"][0]["message"]
-        responses = {}
 
         if function_call := response_message.get("function_call"):
             function_name = function_call["name"]
             function_args = json.loads(function_call["arguments"])
             function = self._get_matching_function(function_name)
 
             if function is None:
                 raise ValueError(
                     f'Function "{function_name}" is not '
                     f"registered with the orchestrator."
                 )
 
-            responses[function_name] = function(**function_args)
+            function_response = function(**function_args)
 
-        return responses
+            try:
+                if not isinstance(function_response, str):
+                    function_response = json.dumps(function_response)
+            except (TypeError, ValueError):
+                function_response = str(function_response)
+
+        return function_response
 
     def _get_matching_function(self, function_name: str) -> Optional[Callable]:
         """
         Returns the function that matches the provided function name, if it exists.
 
         Args:
             function_name (str): The name of the function to be retrieved.
```

### Comparing `openai_functools-1.0.96/openai_functools/metadata_generator.py` & `openai_functools-1.0.97/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.96/pyproject.toml` & `openai_functools-1.0.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "1.0.96"
+version = "1.0.97"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `openai_functools-1.0.96/PKG-INFO` & `openai_functools-1.0.97/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 1.0.96
+Version: 1.0.97
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -93,15 +93,15 @@
                 "required": ["location"],
             },
         }
     ]
     # Proceed with calling openai, invoking the function using the response, etc..
 ```
 
-### Enhanced Automatic Approach
+### Automated Approach using openai-functools
 
 The `openai-functools` library simplifies the process by automatically generating the necessary JSON structure. You just need to import our package and wrap your function with the `openai_function` decorator. Here's how it works:
 
 ```python
 import json
 from openai_functools import openai_function
 
@@ -142,15 +142,15 @@
 orchestrator = FunctionsOrchestrator()
 orchestrator.register_all([get_current_weather, get_weather_next_day])
 # ...
 ```
 
 #### Registering Functions
 
-Functions can be registered using the `register_all` or `register` method as shown in the code snippet above. `register_all` accepts a list of functions, while `register` is used to register a single function. 
+Functions can be registered using the `register_all` or `register` method as shown in the code snippet above. `register_all` accepts a list of functions, while `register` is used to register a single function.
 
 ### Creating and Using Function Descriptions
 
 Function descriptions are automatically created based on the registered functions using `create_function_descriptions` method. These descriptions can then be passed to the OpenAI `ChatCompletion.create` method.
 
 ```python
 response = openai.ChatCompletion.create(
@@ -187,14 +187,19 @@
 
 Currently, only "reStructuredText" (reST) is supported by default, although this can be extended in the future (feel free to contribute!). Under the hood we make use of [docstring parser](https://pypi.org/project/docstring-parser/) to enable this.
 
 ## Examples
 
 Several examples can be found in the `examples` directory of this repository.
 
+1. The [Maintenance app usecase](./examples/maintenance_app_usecase/) is the recommended example to analyse, it shows the power of the library in a (spoofed) real-world setting.
+1. The [Naive approach example](./examples/naive_approach.py) shows how to call openai-functions without use of the library.
+1. The [Simple example](./examples/simple_example.py) is similar to the naive approach, but makes use our decorator.
+1. The [Orchestrator example](./examples/orchestrator_example.py) shows how one can use the orchestrator class.
+
 ## Contributing
 
 We welcome contributions to `openai-functools`! Please see our [contributing guide](CONTRIBUTING.md) for more details.
 
 ## Support
 
 For support with `openai-functools`, please open an issue on this GitHub repository. We will do our best to assist you.
```

