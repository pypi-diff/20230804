# Comparing `tmp/gptfunctionutil-0.2.3.tar.gz` & `tmp/gptfunctionutil-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.2.3.tar", last modified: Fri Jul 28 02:54:13 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.2.4.tar", last modified: Fri Aug  4 15:24:36 2023, max compression
```

## Comparing `gptfunctionutil-0.2.3.tar` & `gptfunctionutil-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.870466 gptfunctionutil-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.858466 gptfunctionutil-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/examples/async_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/examples/custom_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:54:13.870466 gptfunctionutil-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/converter_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/convertutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib_discord.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.376488 gptfunctionutil-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.376488 gptfunctionutil-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.376488 gptfunctionutil-0.2.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.376488 gptfunctionutil-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/examples/async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/examples/custom_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/examples/discord_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.376488 gptfunctionutil-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/converter_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/convertutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/functionlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/functionlib_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/src/gptfunctionutil/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-08-04 15:24:36.000000 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 15:24:36.000000 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:24:36.000000 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-04 15:24:36.000000 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 15:24:36.000000 gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:24:36.380488 gptfunctionutil-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-08-04 15:24:13.000000 gptfunctionutil-0.2.4/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.2.3/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.2.4/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/.gitignore` & `gptfunctionutil-0.2.4/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 pytest.local.ini
+secret.ini
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `gptfunctionutil-0.2.3/.vscode/settings.json` & `gptfunctionutil-0.2.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/LICENSE` & `gptfunctionutil-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/PKG-INFO` & `gptfunctionutil-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.3
-Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
+Version: 0.2.4
+Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python functions and coroutines using the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,55 +22,59 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
-Keywords: OpenAI,Function Calling API,GPT
+Keywords: OpenAI,Function Calling API,GPT,asyncio
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
 The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
-Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and invocation when given a function_call field..
 
-##Installation
+## Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your functions, and to invoke said functions using the Function Call field returned with a call to chat/completions.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+- **Decorate Invokable Functions, and Coroutines**: OpenAI's Function Calling Feature needs JSON schema to outline the name, description, and parameters of each invokable function.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
+  + You can decorate coroutines as well.
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
-- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, you can pass the returned `function_call` field into the `call_by_dict(function_call)`(or `call_by_dict_async` if you're trying to call a decorated coroutine) method to call the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
-   + Schema can also validate and convert responces returned from the chat/completions endpoint.
+   + Schema can also validate and convert responses returned from the chat/completions endpoint.
+
+- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary coroutine, provided you use the `call_by_dict_ctx` method.
+     + (see examples/discord_bot.py for an example.)
+
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.3/README.md` & `gptfunctionutil-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # GPT Function Calling Utility
 
 The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
-Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and invocation when given a function_call field..
 
-##Installation
+## Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your functions, and to invoke said functions using the Function Call field returned with a call to chat/completions.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+- **Decorate Invokable Functions, and Coroutines**: OpenAI's Function Calling Feature needs JSON schema to outline the name, description, and parameters of each invokable function.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
+  + You can decorate coroutines as well.
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
-- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, you can pass the returned `function_call` field into the `call_by_dict(function_call)`(or `call_by_dict_async` if you're trying to call a decorated coroutine) method to call the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
-   + Schema can also validate and convert responces returned from the chat/completions endpoint.
+   + Schema can also validate and convert responses returned from the chat/completions endpoint.
+
+- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary coroutine, provided you use the `call_by_dict_ctx` method.
+     + (see examples/discord_bot.py for an example.)
+
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.3/examples/async_functions.py` & `gptfunctionutil-0.2.4/examples/async_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 
-import inspect
-import re
-from typing import Any, Dict
 from gptfunctionutil import GPTFunctionLibrary, AILibFunction, LibParam
-from gptfunctionutil import add_converter,StringConverter
-from datetime import datetime
 import openai
 import asyncio
 
+'''
 
+'''
 class MyLib(GPTFunctionLibrary):
     @AILibFunction(name='wait_for',description='Wait for a few seconds, then return.')
     @LibParam(targetuser='Number of seconds to wait for.')
     async def wait_for(self,towait:int):
-        #Nothing fancy.  Just get the id, the type, and the string representation of User.
+        #Wait for a set period of time.
         print('launcing waitfor.')
         await asyncio.sleep(towait)
         return f"waited for {towait}'!"
 
 
 async def main():
     # Initialize your subclass before calling the API.
@@ -31,15 +28,14 @@
             {"role": "user", "content": "Wait for 25 seconds."}
         ],
         functions=mylib.get_schema(),
         function_call="auto"
     )
     message=completion.choices[0]['message']
     if 'function_call' in message:
-        #Process function call.
         result=await mylib.call_by_dict_async(message['function_call'])
         #Print result
         print(result)
     else:
         #Unable to tell that it's a function.
         print(completion.choices[0]['message']['content'])
```

### Comparing `gptfunctionutil-0.2.3/examples/custom_converters.py` & `gptfunctionutil-0.2.4/examples/custom_converters.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/pyproject.toml` & `gptfunctionutil-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.2.3"
+version = "0.2.4"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
-description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
+description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python functions and coroutines using the OpenAI Function Calling API"
 readme = 'README.md'
 
-keywords = ['OpenAI', 'Function Calling API', 'GPT']
+keywords = ['OpenAI', 'Function Calling API', 'GPT','asyncio']
 requires-python = '>=3.10'
 
 [project.urls]
 "Homepage"= "https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility"
 
 
 [options.packages.find]
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/__init__.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/__init__.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/converter_core.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/converter_core.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/convertutil.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/convertutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,28 @@
     if typename not in substitutions:
         substitutions[typename] = converterclass
         logs.info(f"Adding converterclass %s for type %s",typename,converterclass)
     else:
         raise ConversionAddError(f'{typename} already in dictionary!')
 class ConvertStatic():
     '''static class for to_schema and from_schema logic.'''
+
     @staticmethod
     def parameter_into_schema(param_name:str,param:inspect.Parameter,dec:Union[str,Dict[str,any]])->Tuple[Dict[str, any], Type[Converter]]:
         """
         Generate a schema for the Converts a parameter signature into a schema.
 
         Parameters:
-        param_name (str): The name of the parameter.
-        param (inspect.Parameter): The parameter signature to convert .
-        dec (Union[str, Dict[str, any]]): Additional keywords to be added to the schema,
-        including definition
+            param_name (str): The name of the parameter.
+            param (inspect.Parameter): The parameter signature to convert .
+            dec (Union[str, Dict[str, any]]): Additional keywords to be added to the schema,
+            including definition
 
         Returns:
-        Tuple[Dict[str, any], Type[Converter]]: The schema generated along with the Converter Class.
+            Tuple[Dict[str, any], Type[Converter]]: The schema generated along with the Converter Class.
 
         Raises:
         ConversionToError: If conversion to schema fails.
         """
         decs=dec
         if isinstance(dec,str):
             decs={'description':dec}
@@ -92,15 +93,15 @@
         logs.info(f"schema generated for param %s with type %s!",param_name,typename)
         return param_info, converter
 
 
     @staticmethod
     def schema_validate(param_name:str,value:any,schema:Union[str,Dict[str,any]],converter:Converter)->Any:
         """
-        Validate and apply needed a value based on schema.
+        Validate and apply any needed conversions to value based on schema.
 
         Parameters:
         param_name (str): The name of the parameter.
         value (any): The value to validate.
         schema (Union[str, Dict[str, any]]): The schema to validate against.
         converter (Converter): The converter to use for validation.
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/errors.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/errors.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/functionlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,36 +29,37 @@
     @staticmethod
     def load_command(name):
         return CommandSingleton._commands.get(name, None)
 
 
 
 class LibCommand:
-    '''This class is a container for functions.
-    that have been annotated with the LibParam and the AILibFunction decorators,
+    '''This class is a container for functions that have been annotated with the
+     LibParam and the AILibFunction decorators,
     wrapping them up with attributes that help the GPTFunctionLibary invoke them.'''
     def __init__(self, func: Union[callable,Coroutine], name: str, description: str, required:List[str]=[],force_words:List[str]=[], enabled=True):
         '''
-        Description: This class represents a library command. It encapsulates a Discord bot command, along with its associated metadata and functionality.
+        This class represents a library command. It encapsulates a callable method/coroutine,
+        along with its associated metadata and functionality.
 
         Args:
-            func (Command): The Discord.py bot command object. (commands.command())
+            func (Union[callable,Coroutine]): The callable method or coroutine to be wrapped.
             name (str): The name of the command.
             description (str): The description of the command.
             required (List[str], optional): A list of required parameter names. Defaults to an empty list.
             force_words (List[str], optional): A list of force words. Defaults to an empty list.
             enabled (bool, optional): Indicates whether the command is enabled. Defaults to True.
         '''
         self.command=func
         self.internal_name=self.function_name=name
         self.comm_type='callable'
 
         if inspect.iscoroutinefunction(func):
             self.comm_type='coroutine'
-        logs.info("adding %s, comm type is %s",self.function_name,self.comm_type)
+        logs.info("initalizing %s, comm type is %s",self.function_name,self.comm_type)
         my_schema= {
             'name': self.function_name,
             'description': description,
             'parameters':{'type': 'object','properties': {},'required': []}
         }
 
         self.function_schema=my_schema
@@ -67,16 +68,17 @@
         self.param_converters={}
         self.param_iterate()
 
         self.enabled=enabled
         self.force_words=force_words
     def param_iterate(self):
         '''
-        Iterates over the command's arguments and update the function_schema dictionary with parameter information.
-        Every parameter that isn't 'self' or ctx must be added!
+        Iterates over the command's arguments and update the function_schema
+        dictionary with parameter information.
+        Every parameter that is not decorated with a valid type will not be added!
         '''
         func=self.command
         paramdict={}
         param_decorators={}
 
         sig = inspect.signature(func)
         if hasattr(func,'parameter_decorators'):
@@ -205,14 +207,15 @@
         Update the FunctionDict with decorated methods from a descended class.
 
         This method iterates over the class's methods and adds the ones with function schema to the FunctionDict.
         """
         for name, method in self.__class__.__dict__.items():
             if hasattr(method, "libcommand"):
                 function_name = method.libcommand.function_name or method.__name__
+                logs.info("adding %s: '%s' into %s function_dictionary",method.libcommand.comm_type,function_name,self.__class__.__name__)
                 self.FunctionDict[function_name] = method.libcommand
 
     def force_word_check(self,query:str):
         '''
         Check if the query contains the force words of any command.
         force words will force OpenAI to invoke THAT particular command, as opposed to
         invoking a command automatically.
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib_discord.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/functionlib_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.internal_name=self.function_name=name
         self.comm_type='callable'
 
         if isinstance(func, Command):
             self.function_name=func.qualified_name
             self.comm_type='command'
 
-            logs.info("adding %s, comm type is %s",self.function_name,self.comm_type)
+            logs.info("initalizing %s, comm type is %s",self.function_name,self.comm_type)
             my_schema= {
                 'name': self.function_name,
                 'description': description,
                 'parameters':{'type': 'object','properties': {},'required': []}
             }
 
             self.function_schema=my_schema
@@ -196,18 +196,19 @@
         """
         Update the FunctionDict with decorated discord.py bot commands.
         This has to be called somewhere before a call to the AI API if you
         want to use the commands.
         """
         for command in bot.walk_commands():
             if "libcommand" in command.extras:
-                logs.info("from command s%, adding %s",command.qualified_name,command.extras["libcommand"])
+                libcommand=command.extras["libcommand"]
+                logs.info("adding %s: '%s' into %s function_dictionary",libcommand.comm_type,command.qualified_name,self.__class__.__name__)
 
                 function_name = command.qualified_name
-                self.FunctionDict[function_name] = command.extras["libcommand"]
+                self.FunctionDict[function_name] = libcommand
 
 
     async def call_by_dict_ctx(self, ctx:Context, function_dict: Dict[str, Any]) -> Coroutine:
         """
         Call a Coroutine or Bot Command based on the provided dictionary.
         Bot Commands must be decorated.
 
@@ -226,17 +227,19 @@
             function_name,function_args=self.parse_name_args(function_dict)
         except GPTLibError as e:
             if isinstance(e, FunctionNotFound):
                 return self.default_callback(e.function_name,e.arguments)
 
             result=str(e)
             return result
-        logs.info('calling function %s with args %s',function_name, function_args)
+
         libmethod = self.FunctionDict.get(function_name)
+        logs.info('invoking %s `%s` with args %s',libmethod.comm_type, function_name, function_args)
         if libmethod.comm_type=='command':
+
             return await libmethod.invoke_command(ctx, function_args)
 
         else:
             if libmethod.comm_type=='coroutine':
                 if len(function_args)>0:
                     return await libmethod.command(self,**function_args)
                 return await libmethod.command(self)
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil/logger.py` & `gptfunctionutil-0.2.4/src/gptfunctionutil/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
-
-# Define the logs
+'''
+a simple logger.
+'''
 logs = logging.getLogger('gptfunctionutil')
 logs.setLevel(logging.DEBUG)
 
 # Create a console handler and set the level to INFO
 console_handler = logging.StreamHandler()
 console_handler.setLevel(logs.level)
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/PKG-INFO` & `gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.3
-Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
+Version: 0.2.4
+Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python functions and coroutines using the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,55 +22,59 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
-Keywords: OpenAI,Function Calling API,GPT
+Keywords: OpenAI,Function Calling API,GPT,asyncio
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
 The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
-Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and invocation when given a function_call field..
 
-##Installation
+## Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your defined methods, and has methods that invoke methods utilizing the Function Call field returned with a call to chat/completions.
+- **Simplified Function Modeling Via Inheritance**: This package utilizes subclasses decended from the `GPTFunctionLibrary` class that allows you to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint.  `GPTFunctionLibrary` contains methods to create a json schema describing your functions, and to invoke said functions using the Function Call field returned with a call to chat/completions.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+- **Decorate Invokable Functions, and Coroutines**: OpenAI's Function Calling Feature needs JSON schema to outline the name, description, and parameters of each invokable function.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
   + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
   + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
   + (`@LibParamSpec`) can apply additional keywords depending on the type. (see https://json-schema.org/understanding-json-schema/index.html for details.)
+  + You can decorate coroutines as well.
 
 
 - **Parameter Typing and Descriptions:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  The library utilizes a collection of converter objects to generate schema for each parameter based on type annotations.
 
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
-- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
-   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, you can pass the returned `function_call` field into the `call_by_dict(function_call)`(or `call_by_dict_async` if you're trying to call a decorated coroutine) method to call the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
-   + Schema can also validate and convert responces returned from the chat/completions endpoint.
+   + Schema can also validate and convert responses returned from the chat/completions endpoint.
+
+- **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
+   + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary coroutine, provided you use the `call_by_dict_ctx` method.
+     + (see examples/discord_bot.py for an example.)
+
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/SOURCES.txt` & `gptfunctionutil-0.2.4/src/gptfunctionutil.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publishpackage.yaml
 .vscode/settings.json
 examples/async_functions.py
 examples/custom_converters.py
+examples/discord_bot.py
 src/README.md
 src/gptfunctionutil/__init__.py
 src/gptfunctionutil/converter_core.py
 src/gptfunctionutil/convertutil.py
 src/gptfunctionutil/errors.py
 src/gptfunctionutil/functionlib.py
 src/gptfunctionutil/functionlib_discord.py
```

### Comparing `gptfunctionutil-0.2.3/tests/conftest.py` & `gptfunctionutil-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.3/tests/test_methods.py` & `gptfunctionutil-0.2.4/tests/test_methods.py`

 * *Files identical despite different names*

