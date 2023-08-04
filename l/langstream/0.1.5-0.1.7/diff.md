# Comparing `tmp/langstream-0.1.5.tar.gz` & `tmp/langstream-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langstream-0.1.5.tar", last modified: Fri Jul 28 06:04:28 2023, max compression
+gzip compressed data, was "langstream-0.1.7.tar", last modified: Fri Aug  4 05:44:49 2023, max compression
```

## Comparing `langstream-0.1.5.tar` & `langstream-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.178701 langstream-0.1.5/
--rw-r--r--   0 rchavesferna   (502) staff       (20)     1070 2023-07-03 19:03:14.000000 langstream-0.1.5/LICENSE
--rw-r--r--   0 rchavesferna   (502) staff       (20)       24 2023-07-06 16:19:10.000000 langstream-0.1.5/MANIFEST.in
--rw-r--r--   0 rchavesferna   (502) staff       (20)     1323 2023-07-28 06:04:28.177003 langstream-0.1.5/PKG-INFO
--rw-r--r--   0 rchavesferna   (502) staff       (20)       59 2023-07-28 06:03:42.000000 langstream-0.1.5/README.md
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.161732 langstream-0.1.5/langstream.egg-info/
--rw-r--r--   0 rchavesferna   (502) staff       (20)     1323 2023-07-28 06:04:28.000000 langstream-0.1.5/langstream.egg-info/PKG-INFO
--rw-r--r--   0 rchavesferna   (502) staff       (20)      542 2023-07-28 06:04:28.000000 langstream-0.1.5/langstream.egg-info/SOURCES.txt
--rw-r--r--   0 rchavesferna   (502) staff       (20)        1 2023-07-28 06:04:28.000000 langstream-0.1.5/langstream.egg-info/dependency_links.txt
--rw-r--r--   0 rchavesferna   (502) staff       (20)       81 2023-07-28 06:04:28.000000 langstream-0.1.5/langstream.egg-info/requires.txt
--rw-r--r--   0 rchavesferna   (502) staff       (20)       16 2023-07-28 06:04:28.000000 langstream-0.1.5/langstream.egg-info/top_level.txt
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.162343 langstream-0.1.5/litechain/
--rw-r--r--   0 rchavesferna   (502) staff       (20)     5009 2023-07-03 07:16:20.000000 langstream-0.1.5/litechain/__init__.py
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.164566 langstream-0.1.5/litechain/contrib/
--rw-r--r--   0 rchavesferna   (502) staff       (20)      740 2023-07-19 11:17:06.000000 langstream-0.1.5/litechain/contrib/__init__.py
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.172470 langstream-0.1.5/litechain/contrib/llms/
--rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-07-06 16:04:59.000000 langstream-0.1.5/litechain/contrib/llms/__init__.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)     2950 2023-07-25 19:05:19.000000 langstream-0.1.5/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)    14041 2023-07-25 20:04:04.000000 langstream-0.1.5/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.174219 langstream-0.1.5/litechain/core/
--rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-07-06 16:04:25.000000 langstream-0.1.5/litechain/core/__init__.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)    23686 2023-07-20 20:03:30.000000 langstream-0.1.5/litechain/core/chain.py
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.175999 langstream-0.1.5/litechain/utils/
--rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-07-06 16:04:44.000000 langstream-0.1.5/litechain/utils/__init__.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)     2540 2023-07-01 15:44:25.000000 langstream-0.1.5/litechain/utils/async_generator.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)     6924 2023-07-20 20:03:30.000000 langstream-0.1.5/litechain/utils/chain.py
--rw-r--r--   0 rchavesferna   (502) staff       (20)      135 2023-07-25 19:51:35.000000 langstream-0.1.5/requirements.txt
--rw-r--r--   0 rchavesferna   (502) staff       (20)       38 2023-07-28 06:04:28.178793 langstream-0.1.5/setup.cfg
--rw-r--r--   0 rchavesferna   (502) staff       (20)     1673 2023-07-28 06:03:12.000000 langstream-0.1.5/setup.py
-drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-07-28 06:04:28.176526 langstream-0.1.5/tests/
--rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-06-23 07:11:41.000000 langstream-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.671893 langstream-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 05:44:40.000000 langstream-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 05:44:40.000000 langstream-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-08-04 05:44:49.671893 langstream-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-08-04 05:44:40.000000 langstream-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.667894 langstream-0.1.7/langstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.667894 langstream-0.1.7/langstream/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.667894 langstream-0.1.7/langstream/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/contrib/llms/gpt4all_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.667894 langstream-0.1.7/langstream/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/core/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.671893 langstream-0.1.7/langstream/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/utils/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-08-04 05:44:40.000000 langstream-0.1.7/langstream/utils/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.667894 langstream-0.1.7/langstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-08-04 05:44:49.000000 langstream-0.1.7/langstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-04 05:44:49.000000 langstream-0.1.7/langstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 05:44:49.000000 langstream-0.1.7/langstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 05:44:49.000000 langstream-0.1.7/langstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 05:44:49.000000 langstream-0.1.7/langstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-04 05:44:40.000000 langstream-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 05:44:49.671893 langstream-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-04 05:44:40.000000 langstream-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:49.671893 langstream-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:44:40.000000 langstream-0.1.7/tests/__init__.py
```

### Comparing `langstream-0.1.5/LICENSE` & `langstream-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langstream-0.1.5/litechain/__init__.py` & `langstream-0.1.7/langstream/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 """
-🪽🔗 LiteChain
+🪽🔗 LangStream
 
-This is the top level module for [LiteChain](https://github.com/rogeriochaves/litechain),
+This is the top level module for [LangStream](https://github.com/rogeriochaves/langstream),
 all the core classes and functions are made available to be imported from here:
 
->>> from litechain import Chain, as_async_generator, filter_final_output # etc
+>>> from langstream import Stream, as_async_generator, filter_final_output # etc
 
-Chain
+Stream
 =====
 
-The `Chain` is the core concept of LiteChain for working with LLMs (Large Language Models), it
+The `Stream` is the core concept of LangStream for working with LLMs (Large Language Models), it
 provides a way to create composable calls to LLMs and any other processing elements.
 
-Since LLMs produce one token at a time, chains are essentially Python AsyncGenerators under the
+Since LLMs produce one token at a time, streams are essentially Python AsyncGenerators under the
 hood, with type-safe composable functions on top. By making use of the type hints and the
-composable functions, LiteChain makes it very easy to build and debug a complex chain of execution
+composable functions, LangStream makes it very easy to build and debug a complex stream of execution
 for working with LLMs.
 
-Since async generation streams is the fundamental block of LiteChain, it's processing should never be blocking.
-When executing a Chain with input, you get back an AsyncGenerator that produces the outputs of all
-pieces in the whole Chain, not only the final one. This means you have access to the each step of
-what is happening, making it easier to display and debug. The final output at the edge of the chain
-is marked as `final` when you process the Chain stream, with helpers available to filter them.
+Since async generation streams is the fundamental block of LangStream, it's processing should never be blocking.
+When executing a Stream with input, you get back an AsyncGenerator that produces the outputs of all
+pieces in the whole Stream, not only the final one. This means you have access to the each step of
+what is happening, making it easier to display and debug. The final output at the edge of the stream
+is marked as `final` when you process the Stream stream, with helpers available to filter them.
 
-On this module, we document the low-level concepts of Chains, so we use simple examples of hardcoded
+On this module, we document the low-level concepts of Streams, so we use simple examples of hardcoded
 string generation. But one you learn the composition fundamentals here, you can expect to apply the
-same functions for composing everythere in LiteChain.
+same functions for composing everythere in LangStream.
 
 Core Concepts
 -------------
 
-`Chain`:
-    A Chain takes in a name and a function, which takes an input and produces an asynchronous stream of outputs from it (AsyncGenerator).
-    Chains can be chained together with the composition methods below, and their input and output types can be
+`Stream`:
+    A Stream takes in a name and a function, which takes an input and produces an asynchronous stream of outputs from it (AsyncGenerator).
+    Streams can be streamed together with the composition methods below, and their input and output types can be
     specifying in the type signature.
 
-`SingleOutputChain`:
-    A SingleOutputChain is a subtype of Chain that produces a single asynchronous final output after processing,
+`SingleOutputStream`:
+    A SingleOutputStream is a subtype of Stream that produces a single asynchronous final output after processing,
     rather than an asynchronous stream of outputs.
 
 Composition Methods
 ------------------
 
-`Chain.map`:
-    Transforms the output of the Chain by applying a function to each token as they arrive. This is
-    non-blocking and maps as chain generations flow in: `chain.map(lambda token: token.lower())`
-
-`Chain.and_then`:
-    Applies a function on the list of results of the Chain. Differently from `map`, this is blocking,
-    and collects the outputs before applying the function. It can also take another Chain as argument,
-    effectively composing two Chains together: `first_chain.and_then(second_chain)`.
+`Stream.map`:
+    Transforms the output of the Stream by applying a function to each token as they arrive. This is
+    non-blocking and maps as stream generations flow in: `stream.map(lambda token: token.lower())`
+
+`Stream.and_then`:
+    Applies a function on the list of results of the Stream. Differently from `map`, this is blocking,
+    and collects the outputs before applying the function. It can also take another Stream as argument,
+    effectively composing two Streams together: `first_stream.and_then(second_stream)`.
 
-`Chain.collect`:
-    Collects the output of a Chain into a list. This is a blocking operation and can be used
+`Stream.collect`:
+    Collects the output of a Stream into a list. This is a blocking operation and can be used
     when the next processing step requires the full output at once.
 
-`Chain.join`:
-    Joins the output of a string producing Chain into a single string by concatenating each item.
+`Stream.join`:
+    Joins the output of a string producing Stream into a single string by concatenating each item.
 
-`Chain.gather`:
-    Gathers results from a chain that produces multiple async generators and processes them in parallel,
-    returning a list of lists of the results of all generators, allowing you to execute many Chains at
+`Stream.gather`:
+    Gathers results from a stream that produces multiple async generators and processes them in parallel,
+    returning a list of lists of the results of all generators, allowing you to execute many Streams at
     the same time, this is similar to `asyncio.gather`.
 
 Contrib: OpenAI, GPT4All and more
 ---------------------------------
 
-The core of LiteChain is kept small and stable, so all the integrations that build on top of it live separate,
-under the `litechain.contrib` module. Check it out for reference and code examples of the integrations.
+The core of LangStream is kept small and stable, so all the integrations that build on top of it live separate,
+under the `langstream.contrib` module. Check it out for reference and code examples of the integrations.
 
 Examples
 --------
 
-Using Chain to process text data:
+Using Stream to process text data:
 
-    >>> from litechain import Chain, as_async_generator, collect_final_output
+    >>> from langstream import Stream, as_async_generator, collect_final_output
     >>> import asyncio
     ...
     >>> async def example():
-    ...     # Chain that splits a sentence into words
-    ...     words_chain = Chain[str, str]("WordsChain", lambda sentence: as_async_generator(*sentence.split(" ")))
-    ...     # Chain that capitalizes each word
-    ...     capitalized_chain = words_chain.map(lambda word: word.capitalize())
+    ...     # Stream that splits a sentence into words
+    ...     words_stream = Stream[str, str]("WordsStream", lambda sentence: as_async_generator(*sentence.split(" ")))
+    ...     # Stream that capitalizes each word
+    ...     capitalized_stream = words_stream.map(lambda word: word.capitalize())
     ...     # Join the capitalized words into a single string
-    ...     chain = capitalized_chain.join(" ")
+    ...     stream = capitalized_stream.join(" ")
     ...
-    ...     async for output in chain("this is an example"):
+    ...     async for output in stream("this is an example"):
     ...         if output.final:
     ...             return output.data
     ...
     >>> asyncio.run(example())
     'This Is An Example'
 
 ---
 
-Here you can find the reference and code examples, for further tutorials and use cases, consult the [documentation](https://github.com/rogeriochaves/litechain).
+Here you can find the reference and code examples, for further tutorials and use cases, consult the [documentation](https://github.com/rogeriochaves/langstream).
 """
 
-from litechain.core.chain import Chain, ChainOutput, SingleOutputChain
-from litechain.utils.chain import (
+from langstream.core.stream import Stream, StreamOutput, SingleOutputStream
+from langstream.utils.stream import (
     debug,
     filter_final_output,
     collect_final_output,
     join_final_output,
 )
-from litechain.utils.async_generator import (
+from langstream.utils.async_generator import (
     as_async_generator,
     collect,
     join,
     gather,
     next_item,
 )
 
 __all__ = (
-    "Chain",
-    "ChainOutput",
-    "SingleOutputChain",
+    "Stream",
+    "StreamOutput",
+    "SingleOutputStream",
     "debug",
     "filter_final_output",
     "collect_final_output",
     "join_final_output",
     "as_async_generator",
     "collect",
     "join",
```

### Comparing `langstream-0.1.5/litechain/contrib/llms/gpt4all_chain.py` & `langstream-0.1.7/langstream/contrib/llms/gpt4all_stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import asyncio
 from typing import AsyncGenerator, Callable, Iterable, Optional, TypeVar, cast
 
 from gpt4all import GPT4All
 
-from litechain.core.chain import Chain
+from langstream.core.stream import Stream
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-class GPT4AllChain(Chain[T, U]):
+class GPT4AllStream(Stream[T, U]):
     """
-    GPT4AllChain is a Chain that allows you to run local LLMs easily
+    GPT4AllStream is a Stream that allows you to run local LLMs easily
     using [GPT4All](https://gpt4all.io/) model.
 
     [GPT4All](https://gpt4all.io/) is a project that focuses on making
     the LLM models very small and very fast to be able to run in any computer
     without GPUs. Check out more about the project [here](https://gpt4all.io/).
 
-    You can use it as any other chain, on the first use, it will download the model
+    You can use it as any other stream, on the first use, it will download the model
     (a few GB). Alternatively, you can point to a locally downloaded model.bin file.
 
     There are serveral parameters you can use to adjust the model output such as
     `temperature`, `max_tokens`, `top_k`, `repeat_penalty`, etc, you can read more
     about them [here](https://docs.gpt4all.io/gpt4all_python.html#generation-parameters).
 
     Example
     -------
 
-    >>> from litechain import join_final_output
-    >>> from litechain.contrib import GPT4AllChain
+    >>> from langstream import join_final_output
+    >>> from langstream.contrib import GPT4AllStream
     >>> import asyncio
     ...
     >>> async def example():
-    ...     greet_chain = GPT4AllChain[str, str](
-    ...         "GreetingChain",
+    ...     greet_stream = GPT4AllStream[str, str](
+    ...         "GreetingStream",
     ...         lambda name: f"### User: Hello, my name is {name}. How is it going?\\n\\n### Response:",
     ...         model="orca-mini-3b.ggmlv3.q4_0.bin",
     ...         temperature=0,
     ...     )
     ...
-    ...     return await join_final_output(greet_chain("Alice"))
+    ...     return await join_final_output(greet_stream("Alice"))
     ...
     >>> asyncio.run(example()) # doctest:+ELLIPSIS +SKIP
     Found model file at ...
     " I'm doing well, thank you for asking! How about you?"
 
     """
 
     def __init__(
-        self: "GPT4AllChain[T, str]",
+        self: "GPT4AllStream[T, str]",
         name: str,
         call: Callable[
             [T],
             str,
         ],
         model: str,
         temperature: float = 0,
```

### Comparing `langstream-0.1.5/litechain/contrib/llms/open_ai.py` & `langstream-0.1.7/langstream/contrib/llms/open_ai.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,54 +13,54 @@
     cast,
 )
 
 import openai
 from colorama import Fore
 from retry import retry
 
-from litechain.core.chain import Chain, ChainOutput
+from langstream.core.stream import Stream, StreamOutput
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
 
-class OpenAICompletionChain(Chain[T, U]):
+class OpenAICompletionStream(Stream[T, U]):
     """
-    `OpenAICompletionChain` uses the most simple LLMs from OpenAI based on GPT-3 for text completion, if you are looking for ChatCompletion, take a look at `OpenAIChatChain`.
+    `OpenAICompletionStream` uses the most simple LLMs from OpenAI based on GPT-3 for text completion, if you are looking for ChatCompletion, take a look at `OpenAIChatStream`.
 
-    The `OpenAICompletionChain` takes a lambda function that should return a string with the prompt for completion.
+    The `OpenAICompletionStream` takes a lambda function that should return a string with the prompt for completion.
 
-    To use this chain you will need an `OPENAI_API_KEY` environment variable to be available, and then you can generate completions out of it.
+    To use this stream you will need an `OPENAI_API_KEY` environment variable to be available, and then you can generate completions out of it.
 
     You can read more about the completion API on [OpenAI API reference](https://platform.openai.com/docs/api-reference/completions)
 
     Example
     -------
 
-    >>> from litechain import join_final_output
-    >>> from litechain.contrib import OpenAICompletionChain
+    >>> from langstream import join_final_output
+    >>> from langstream.contrib import OpenAICompletionStream
     >>> import asyncio
     ...
     >>> async def example():
-    ...     recipe_chain = OpenAICompletionChain[str, str](
-    ...         "RecipeChain",
+    ...     recipe_stream = OpenAICompletionStream[str, str](
+    ...         "RecipeStream",
     ...         lambda recipe_name: f"Here is my {recipe_name} recipe: ",
     ...         model="ada",
     ...     )
     ...
-    ...     return await join_final_output(recipe_chain("instant noodles"))
+    ...     return await join_final_output(recipe_stream("instant noodles"))
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     '【Instant Noodles】\\n\\nIngredients:\\n\\n1 cup of water'
 
     """
 
     def __init__(
-        self: "OpenAICompletionChain[T, str]",
+        self: "OpenAICompletionStream[T, str]",
         name: str,
         call: Callable[
             [T],
             str,
         ],
         model: str,
         temperature: Optional[float] = 0,
@@ -94,15 +94,15 @@
 
         super().__init__(name, lambda input: completion(call(input)))
 
 
 @dataclass
 class OpenAIChatMessage:
     """
-    OpenAIChatMessage is a data class that represents a chat message for building `OpenAIChatChain` prompt.
+    OpenAIChatMessage is a data class that represents a chat message for building `OpenAIChatStream` prompt.
 
     Attributes
     ----------
     role : Literal["system", "user", "assistant", "function"]
         The role of who sent this message in the chat, can be one of `"system"`, `"user"`, `"assistant"` or "function"
 
     name: Optional[str]
@@ -120,15 +120,15 @@
     def to_dict(self):
         return {k: v for k, v in self.__dict__.items() if v is not None}
 
 
 @dataclass
 class OpenAIChatDelta:
     """
-    OpenAIChatDelta is a data class that represents the output of an `OpenAIChatChain`.
+    OpenAIChatDelta is a data class that represents the output of an `OpenAIChatStream`.
 
     Attributes
     ----------
     role : Optional[Literal["assistant", "function"]]
         The role of the output message, the first message will have the role, while
         the subsequent partial content output ones will have the role as `None`.
         For now the only possible values it will have is either None or `"assistant"`
@@ -142,95 +142,95 @@
 
     """
 
     role: Optional[Literal["assistant", "function"]]
     content: str
     name: Optional[str] = None
 
-    def __chain_debug__(self):
+    def __stream_debug__(self):
         name = ""
         if self.name:
             name = f" {self.name}"
         if self.role is not None:
             print(f"{Fore.YELLOW}{self.role.capitalize()}{name}:{Fore.RESET} ", end="")
         print(
             self.content,
             end="",
             flush=True,
         )
 
 
-class OpenAIChatChain(Chain[T, U]):
+class OpenAIChatStream(Stream[T, U]):
     """
-    `OpenAIChatChain` gives you access to the more powerful LLMs from OpenAI, like `gpt-3.5-turbo` and `gpt-4`, they are structured in a chat format with roles.
+    `OpenAIChatStream` gives you access to the more powerful LLMs from OpenAI, like `gpt-3.5-turbo` and `gpt-4`, they are structured in a chat format with roles.
 
-    The `OpenAIChatChain` takes a lambda function that should return a list of `OpenAIChatMessage` for the assistant to reply, it is stateless, so it doesn't keep
-    memory of the past chat messages, you will have to handle the memory yourself, you can [follow this guide to get started on memory](https://rogeriochaves.github.io/litechain/docs/llms/memory).
+    The `OpenAIChatStream` takes a lambda function that should return a list of `OpenAIChatMessage` for the assistant to reply, it is stateless, so it doesn't keep
+    memory of the past chat messages, you will have to handle the memory yourself, you can [follow this guide to get started on memory](https://rogeriochaves.github.io/langstream/docs/llms/memory).
 
-    The `OpenAIChatChain` also produces `OpenAIChatDelta` as output, one per token, it contains the `role` that started the output, and then subsequent `content` updates.
+    The `OpenAIChatStream` also produces `OpenAIChatDelta` as output, one per token, it contains the `role` that started the output, and then subsequent `content` updates.
     If you want the final content as a string, you will need to use the `.content` property from the delta and accumulate it for the final result.
 
-    To use this chain you will need an `OPENAI_API_KEY` environment variable to be available, and then you can generate chat completions out of it.
+    To use this stream you will need an `OPENAI_API_KEY` environment variable to be available, and then you can generate chat completions out of it.
 
     You can read more about the chat completion API on [OpenAI API reference](https://platform.openai.com/docs/api-reference/chat)
 
     Example
     -------
 
-    >>> from litechain import Chain, join_final_output
-    >>> from litechain.contrib import OpenAIChatChain, OpenAIChatMessage, OpenAIChatDelta
+    >>> from langstream import Stream, join_final_output
+    >>> from langstream.contrib import OpenAIChatStream, OpenAIChatMessage, OpenAIChatDelta
     >>> import asyncio
     ...
     >>> async def example():
-    ...     recipe_chain: Chain[str, str] = OpenAIChatChain[str, OpenAIChatDelta](
-    ...         "RecipeChain",
+    ...     recipe_stream: Stream[str, str] = OpenAIChatStream[str, OpenAIChatDelta](
+    ...         "RecipeStream",
     ...         lambda recipe_name: [
     ...             OpenAIChatMessage(
     ...                 role="system",
     ...                 content="You are ChefGPT, an assistant bot trained on all culinary knowledge of world's most proeminant Michelin Chefs",
     ...             ),
     ...             OpenAIChatMessage(
     ...                 role="user",
     ...                 content=f"Hello, could you write me a recipe for {recipe_name}?",
     ...             ),
     ...         ],
     ...         model="gpt-3.5-turbo",
     ...         max_tokens=10,
     ...     ).map(lambda delta: delta.content)
     ...
-    ...     return await join_final_output(recipe_chain("instant noodles"))
+    ...     return await join_final_output(recipe_stream("instant noodles"))
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     "Of course! Here's a simple and delicious recipe"
 
     You can also pass OpenAI function schemas in the `function` argument with all parameter definitions, the model may then produce a `function` role `OpenAIChatDelta`,
     using your function, with the `content` field as a json which you can parse to call an actual function.
 
-    Take a look [at our guide](https://rogeriochaves.github.io/litechain/docs/llms/open_ai_functions) to learn more about OpenAI function calls in LiteChain.
+    Take a look [at our guide](https://rogeriochaves.github.io/langstream/docs/llms/open_ai_functions) to learn more about OpenAI function calls in LangStream.
 
     Function Call Example
     ---------------------
 
-    >>> from litechain import Chain, collect_final_output
-    >>> from litechain.contrib import OpenAIChatChain, OpenAIChatMessage, OpenAIChatDelta
+    >>> from langstream import Stream, collect_final_output
+    >>> from langstream.contrib import OpenAIChatStream, OpenAIChatMessage, OpenAIChatDelta
     >>> from typing import Literal, Union, Dict
     >>> import asyncio
     ...
     >>> async def example():
     ...     def get_current_weather(
     ...         location: str, format: Literal["celsius", "fahrenheit"] = "celsius"
     ...     ) -> Dict[str, str]:
     ...         return {
     ...             "location": location,
     ...             "forecast": "sunny",
     ...             "temperature": "25 C" if format == "celsius" else "77 F",
     ...         }
     ...
-    ...     chain : Chain[str, Union[OpenAIChatDelta, Dict[str, str]]] = OpenAIChatChain[str, Union[OpenAIChatDelta, Dict[str, str]]](
-    ...         "WeatherChain",
+    ...     stream : Stream[str, Union[OpenAIChatDelta, Dict[str, str]]] = OpenAIChatStream[str, Union[OpenAIChatDelta, Dict[str, str]]](
+    ...         "WeatherStream",
     ...         lambda user_input: [
     ...             OpenAIChatMessage(role="user", content=user_input),
     ...         ],
     ...         model="gpt-3.5-turbo",
     ...         functions=[
     ...             {
     ...                 "name": "get_current_weather",
@@ -255,39 +255,39 @@
     ...         temperature=0,
     ...     ).map(
     ...         lambda delta: get_current_weather(**json.loads(delta.content))
     ...         if delta.role == "function" and delta.name == "get_current_weather"
     ...         else delta
     ...     )
     ...
-    ...     return await collect_final_output(chain("how is the weather today in Rio de Janeiro?"))
+    ...     return await collect_final_output(stream("how is the weather today in Rio de Janeiro?"))
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     [{'location': 'Rio de Janeiro', 'forecast': 'sunny', 'temperature': '25 C'}]
 
     """
 
     def __init__(
-        self: "OpenAIChatChain[T, OpenAIChatDelta]",
+        self: "OpenAIChatStream[T, OpenAIChatDelta]",
         name: str,
         call: Callable[
             [T],
             List[OpenAIChatMessage],
         ],
         model: str,
         functions: Optional[List[Dict[str, Any]]] = None,
-        function_call: Optional[Union[Literal["none", "auto"], str]] = None,
+        function_call: Optional[Union[Literal["none", "auto"], Dict[str, Any]]] = None,
         temperature: Optional[float] = 0,
         max_tokens: Optional[int] = None,
         timeout: int = 5,
         retries: int = 3,
     ) -> None:
         async def chat_completion(
             messages: List[OpenAIChatMessage],
-        ) -> AsyncGenerator[ChainOutput[OpenAIChatDelta], None]:
+        ) -> AsyncGenerator[StreamOutput[OpenAIChatDelta], None]:
             loop = asyncio.get_event_loop()
 
             @retry(tries=retries)
             def get_completions():
                 function_kwargs = {}
                 if functions is not None:
                     function_kwargs["functions"] = functions
```

### Comparing `langstream-0.1.5/litechain/core/chain.py` & `langstream-0.1.7/langstream/core/stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Core Chain module
+Core Stream module
 """
 import asyncio
 from dataclasses import dataclass
 from typing import (
     Any,
     AsyncGenerator,
     Callable,
@@ -13,588 +13,750 @@
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
-from litechain.utils.async_generator import as_async_generator
+import asyncstdlib
+
+from langstream.utils.async_generator import as_async_generator, merge
+from langstream.utils._typing import unwrap
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 W = TypeVar("W")
 X = TypeVar("X")
 
 
 @dataclass
-class ChainOutput(Generic[T]):
+class StreamOutput(Generic[T]):
     """
-    ChainOutput is a data class that represents the output of a Chain at each step.
+    StreamOutput is a data class that represents the output of a Stream at each step.
 
     Attributes
     ----------
-    chain : str
-        The name of the chain that produced this output. This helps in identifying
+    stream : str
+        The name of the stream that produced this output. This helps in identifying
         which part of the processing pipeline the output is coming from.
 
     output : Union[T, Any]
-        The actual output data produced by the chain. This will be type T for final chain output,
-        but can be also be of any type produced by any step of the whole chain.
+        The actual output data produced by the stream. This will be type T for final stream output,
+        but can be also be of any type produced by any step of the whole stream.
 
     final : bool
-        A boolean flag indicating whether this output is the final output of the chain.
-        Only the outputs at the end of the chain are marked as "final".
+        A boolean flag indicating whether this output is the final output of the stream.
+        Only the outputs at the end of the stream are marked as "final".
 
     Example
     -------
 
-    >>> from litechain import Chain
+    >>> from langstream import Stream
     >>> import asyncio
     ...
     >>> async def example():
-    ...     greet_chain = Chain[str, str]("GreetingChain", lambda name: f"Hello, {name}!")
-    ...     polite_chain = greet_chain.map(lambda greeting: f"{greeting} How are you?")
+    ...     greet_stream = Stream[str, str]("GreetingStream", lambda name: f"Hello, {name}!")
+    ...     polite_stream = greet_stream.map(lambda greeting: f"{greeting} How are you?")
     ...
-    ...     async for output in polite_chain("Alice"):
-    ...         # Output is of type ChainOutput
+    ...     async for output in polite_stream("Alice"):
+    ...         # Output is of type StreamOutput
     ...         print(output)
     ...
     >>> asyncio.run(example())
-    ChainOutput(chain='GreetingChain', data='Hello, Alice!', final=False)
-    ChainOutput(chain='GreetingChain@map', data='Hello, Alice! How are you?', final=True)
+    StreamOutput(stream='GreetingStream', data='Hello, Alice!', final=False)
+    StreamOutput(stream='GreetingStream@map', data='Hello, Alice! How are you?', final=True)
     """
 
-    chain: str
+    stream: str
     data: Union[T, Any]
     final: bool
 
 
-class Chain(Generic[T, U]):
+class Stream(Generic[T, U]):
     """"""
 
     _call: Callable[
-        [T], Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U]
+        [T], Union[AsyncGenerator[StreamOutput[U], Any], AsyncGenerator[U, Any], U]
     ]
 
     def __init__(
         self,
         name: str,
         call: Callable[
             [T],
-            Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U],
+            Union[AsyncGenerator[StreamOutput[U], Any], AsyncGenerator[U, Any], U],
         ],
     ) -> None:
         self.name = name
         self._call = call
 
-    def __call__(self, input: T) -> AsyncGenerator[ChainOutput[U], Any]:
+    def __call__(self, input: T) -> AsyncGenerator[StreamOutput[U], Any]:
         result = self._call(input)
         return self._wrap(result)
 
     def _wrap(
         self,
-        value: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
+        value: Union[AsyncGenerator[StreamOutput[V], Any], AsyncGenerator[V, Any], V],
+        final: Optional[bool] = None,
         name: Optional[str] = None,
-    ) -> AsyncGenerator[ChainOutput[V], Any]:
+    ) -> AsyncGenerator[StreamOutput[V], Any]:
         async def _wrap(
-            values: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any]],
-        ) -> AsyncGenerator[ChainOutput[V], Any]:
+            values: Union[AsyncGenerator[StreamOutput[V], Any], AsyncGenerator[V, Any]],
+        ) -> AsyncGenerator[StreamOutput[V], Any]:
             async for value in values:
-                yield self._output_wrap(value, name=name)
+                yield self._output_wrap(value, final=final, name=name)
 
         if isinstance(value, AsyncGenerator):
             return _wrap(value)
         return _wrap(as_async_generator(value))
 
     def _output_wrap(
-        self, value: Union[ChainOutput[V], V], final=None, name=None
-    ) -> ChainOutput[V]:
-        if isinstance(value, ChainOutput):
+        self, value: Union[StreamOutput[V], V], final=None, name=None
+    ) -> StreamOutput[V]:
+        if isinstance(value, StreamOutput):
             final = final if final is not None else value.final
-            return ChainOutput[V](chain=value.chain, data=value.data, final=final)
+            return StreamOutput[V](stream=value.stream, data=value.data, final=final)
 
         final = final if final is not None else True
-        return ChainOutput[V](
-            chain=self.name if name is None else name, data=value, final=final
+        return StreamOutput[V](
+            stream=self.name if name is None else name, data=value, final=final
         )
 
     async def _reyield(
-        self, async_iterable: AsyncGenerator[ChainOutput[U], Any]
-    ) -> AsyncGenerator[Tuple[List[U], ChainOutput[U]], Any]:
+        self, async_iterable: AsyncGenerator[StreamOutput[U], Any]
+    ) -> AsyncGenerator[Tuple[List[U], StreamOutput[U]], Any]:
         values: List[U] = []
         async for u in async_iterable:
             u_rewrapped = self._output_wrap(u, final=False)
             if u.final:
                 values.append(u.data)
             yield (values, u_rewrapped)
 
-    def map(self, fn: Callable[[U], V]) -> "Chain[T, V]":
+    def map(self, fn: Callable[[U], V]) -> "Stream[T, V]":
         """
-        Maps the output of the current chain through a function as they arrive.
+        Maps the output of the current stream through a function as they arrive.
 
-        The transform function will receive the current output of the chain and
+        The transform function will receive the current output of the stream and
         should return a modified version of it. This method is non-blocking and
-        will continue processing the chain in parallel.
+        will continue processing the stream in parallel.
 
         Example:
 
-        >>> from litechain import Chain, join_final_output
+        >>> from langstream import Stream, join_final_output
         >>> import asyncio
         ...
         >>> async def example():
-        ...     greet_chain = Chain[str, str]("GreetingChain", lambda name: f"Hello, {name}!")
-        ...     polite_chain = greet_chain.map(lambda greeting: f"{greeting} How are you?")
-        ...     return await join_final_output(polite_chain("Alice"))
+        ...     greet_stream = Stream[str, str]("GreetingStream", lambda name: f"Hello, {name}!")
+        ...     polite_stream = greet_stream.map(lambda greeting: f"{greeting} How are you?")
+        ...     return await join_final_output(polite_stream("Alice"))
         ...
         >>> asyncio.run(example())
         'Hello, Alice! How are you?'
 
 
         Example of processing one token at a time:
 
-        >>> from litechain import Chain, as_async_generator, join_final_output
+        >>> from langstream import Stream, as_async_generator, join_final_output
         >>> import asyncio
         ...
         >>> async def example():
-        ...     words_chain = Chain[str, str]("WordsChain", lambda sentence: as_async_generator(*sentence.split(" "))) # produces one word at a time
-        ...     accronym_chain = words_chain.map(lambda word: word.upper()[0]) # uppercases each word and take the first letter
-        ...     return await join_final_output(accronym_chain("as soon as possible"))
+        ...     words_stream = Stream[str, str]("WordsStream", lambda sentence: as_async_generator(*sentence.split(" "))) # produces one word at a time
+        ...     accronym_stream = words_stream.map(lambda word: word.upper()[0]) # uppercases each word and take the first letter
+        ...     return await join_final_output(accronym_stream("as soon as possible"))
         ...
         >>> asyncio.run(example())
         'ASAP'
         """
 
         next_name = f"{self.name}@map"
 
-        async def map(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
-            # Reyield previous chain so we never block the stream, and at the same time yield mapped values
+        async def map(input: T) -> AsyncGenerator[StreamOutput[V], Any]:
+            # Reyield previous stream so we never block the stream, and at the same time yield mapped values
             prev_len_values = 0
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[V], to_reyield)
+                yield cast(StreamOutput[V], to_reyield)
                 if len(values) > prev_len_values:  # as soon as there is a new value
                     prev_len_values = len(values)
                     yield self._output_wrap(fn(values[-1]), name=next_name)
 
-        return Chain[T, V](next_name, lambda input: map(input))
+        return Stream[T, V](next_name, lambda input: map(input))
+
+    def filter(self, fn: Callable[[U], bool]) -> "Stream[T, U]":
+        """
+        Filters the output of the current stream, keeping only the values that return True.
+
+        This method is non-blocking and expects a function that returns True for keeping the value,
+        or False for dropping it, as they arrive.
+
+        Example:
+
+        >>> from langstream import Stream, as_async_generator, collect_final_output
+        >>> import asyncio
+        ...
+        >>> async def example():
+        ...     numbers_stream = Stream[int, int]("NumbersStream", lambda input: as_async_generator(*range(0, input)))
+        ...     even_stream = numbers_stream.filter(lambda input: input % 2 == 0)
+        ...     return await collect_final_output(even_stream(9))
+        ...
+        >>> asyncio.run(example())
+        [0, 2, 4, 6, 8]
+        """
+
+        next_name = f"{self.name}@filter"
+
+        async def filter(input: T) -> AsyncGenerator[StreamOutput[U], Any]:
+            # Reyield previous stream so we never block the stream, and at the same time yield mapped values
+            prev_len_values = 0
+            async for values, to_reyield in self._reyield(self(input)):
+                yield to_reyield
+                if len(values) > prev_len_values:  # as soon as there is a new value
+                    prev_len_values = len(values)
+                    if fn(values[-1]):
+                        yield self._output_wrap(values[-1], name=next_name)
+
+        return Stream[T, U](next_name, lambda input: filter(input))
 
     def and_then(
         self,
         next: Callable[
             [Iterable[U]],
-            Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
+            Union[AsyncGenerator[StreamOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
-    ) -> "Chain[T, V]":
+    ) -> "Stream[T, V]":
         """
-        Processes the output of the current chain through a transformation function or another chain.
+        Processes the output of the current stream through a transformation function or another stream.
 
         Unlike the map method, which applies transformations to outputs as they arrive,
-        the and_then method first collects all the outputs and then passes them to the transformation function or the next chain.
-        This method is blocking and will wait for the entire chain to be processed before applying the transformation.
+        the and_then method first collects all the outputs and then passes them to the transformation function or the next stream.
+        This method is blocking and will wait for the entire stream to be processed before applying the transformation.
 
         If `transform` is a function, it should accept the list of collected outputs and return a modified version of it.
-        If `transform` is another chain, it is used to process the list of collected outputs.
+        If `transform` is another stream, it is used to process the list of collected outputs.
 
         Example using a function:
 
-        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> from langstream import Stream, as_async_generator, collect_final_output
         >>> import asyncio
         ...
         >>> async def example():
-        ...     word_chain = Chain[str, str]("WordChain", lambda word: as_async_generator(word, "!"))
-        ...     count_chain : Chain[str, int] = word_chain.and_then(lambda outputs: len(list(outputs)))
-        ...     return await collect_final_output(count_chain("Hi"))
+        ...     word_stream = Stream[str, str]("WordStream", lambda word: as_async_generator(word, "!"))
+        ...     count_stream : Stream[str, int] = word_stream.and_then(lambda outputs: len(list(outputs)))
+        ...     return await collect_final_output(count_stream("Hi"))
         ...
         >>> asyncio.run(example())
         [2]
 
 
-        Example using another chain:
+        Example using another stream:
 
-        >>> from litechain import Chain, as_async_generator, join_final_output
+        >>> from langstream import Stream, as_async_generator, join_final_output
         >>> from typing import Iterable
         >>> import asyncio
         ...
         >>> async def example():
-        ...     words_chain = Chain[str, str]("WordsChain", lambda sentence: as_async_generator(*sentence.split(" "))) # produces one word at a time
-        ...     acronym_chain = Chain[Iterable[str], str]("AcronymChain", lambda words: "".join(word.upper()[0] for word in words)) # produces acronym
-        ...     composed_chain = words_chain.and_then(acronym_chain)
-        ...     return await join_final_output(composed_chain("as soon as possible"))
+        ...     words_stream = Stream[str, str]("WordsStream", lambda sentence: as_async_generator(*sentence.split(" "))) # produces one word at a time
+        ...     acronym_stream = Stream[Iterable[str], str]("AcronymStream", lambda words: "".join(word.upper()[0] for word in words)) # produces acronym
+        ...     composed_stream = words_stream.and_then(acronym_stream)
+        ...     return await join_final_output(composed_stream("as soon as possible"))
         ...
         >>> asyncio.run(example())
         'ASAP'
         """
 
         next_name = f"{self.name}@and_then"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def and_then(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[V], Any]:
-            # First, reyield previous chain so we never block the stream, and collect the results until they are done
+        ) -> AsyncGenerator[StreamOutput[V], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the results until they are done
             iter_u: Iterable[U] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[V], to_reyield)
+                yield cast(StreamOutput[V], to_reyield)
                 iter_u = values
 
-            # Then, call in the next chain
+            # Then, call in the next stream
             iter_v = self._wrap(next(iter_u), name=next_name)
             async for v in iter_v:
                 yield v
 
-        return Chain[T, V](next_name, and_then)
+        return Stream[T, V](next_name, and_then)
+
+    def pipe(
+        self,
+        fn: Callable[
+            [AsyncGenerator[U, Any]], AsyncGenerator[Union[StreamOutput[V], V], Any]
+        ],
+    ) -> "Stream[T, V]":
+        """
+        Lower level constructor to pipe a stream into another one, giving you the underlying AsyncGenerator.
+        Pipe takes a callback function which should always produce an AsyncGenerator in return, which means you
+        need to declare an async function and your function needs to use `yield` for generating values, the advantage
+        of that is that you have fine control on whether it will be blocking the stream or not.
+
+        In fact, with pipe you can reconstruct `map` and `and_then`, for example:
+
+        >>> from langstream import Stream, as_async_generator, collect_final_output
+        >>> from typing import List, AsyncGenerator
+        >>> import asyncio
+        ...
+        >>> async def example(items):
+        ...     async def mario_pipe(stream: AsyncGenerator[str, None]) -> AsyncGenerator[str, None]:
+        ...        waiting_for_mushroom = False
+        ...        async for item in stream:
+        ...            if item == "Mario":
+        ...                waiting_for_mushroom = True
+        ...            elif item == "Mushroom" and waiting_for_mushroom:
+        ...                yield "Super Mario!"
+        ...            else:
+        ...                yield item + "?"
+        ...
+        ...     piped_stream = Stream[List[str], str](
+        ...         "PipedStream", lambda items: as_async_generator(*items)
+        ...     ).pipe(mario_pipe)
+        ...
+        ...     return await collect_final_output(piped_stream(items))
+        ...
+        >>> asyncio.run(example(["Mario", "Mushroom"]))
+        ['Super Mario!']
+        >>> asyncio.run(example(["Luigi"]))
+        ['Luigi?']
+        >>> asyncio.run(example(["Mario", "Luigi", "Mushroom"]))
+        ['Luigi?', 'Super Mario!']
+
+        As you can see this pipe blocks kinda like `and_then` when it sees "Mario", until a mushroom arrives, but for other random items
+        such as "Luigi" it just re-yields it immediately, adding a question mark, non-blocking, like `map`.
+
+        You can also call another stream from `pipe` directly, just be sure to re-yield its outputs
+        """
+
+        next_name = f"{self.name}@pipe"
+
+        async def filter_final_output(
+            async_iterable: AsyncGenerator[StreamOutput[U], Any]
+        ) -> AsyncGenerator[U, Any]:
+            async for output in async_iterable:
+                if output.final:
+                    yield cast(U, output.data)
+
+        def pipe(input: T) -> AsyncGenerator[StreamOutput[V], Any]:
+            previous, final = asyncstdlib.tee(self(input), n=2, lock=asyncio.Lock())
+
+            previous = self._wrap(previous, name=next_name, final=False)
+            previous = cast(AsyncGenerator[StreamOutput[V], Any], previous)
+
+            final = filter_final_output(
+                cast(AsyncGenerator[StreamOutput[U], Any], final)
+            )
+            final = cast(
+                AsyncGenerator[StreamOutput[V], Any],
+                self._wrap(fn(final), name=next_name),
+            )
 
-    def collect(self: "Chain[T, U]") -> "SingleOutputChain[T, List[U]]":
+            return merge(previous, final)
+
+        return Stream[T, V](next_name, pipe)
+
+    def collect(self: "Stream[T, U]") -> "SingleOutputStream[T, List[U]]":
         """
-        Collects all the outputs produced by the chain and returns them as a list.
+        Collects all the outputs produced by the stream and returns them as a list.
 
-        This method is blocking useful when the next chain or processing step needs to have access to the
+        This method is blocking useful when the next stream or processing step needs to have access to the
         entire output all at once, rather than processing elements as they arrive.
 
         Example:
 
-        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> from langstream import Stream, as_async_generator, collect_final_output
         >>> import asyncio
         ...
         >>> async def example():
-        ...     word_chain: Chain[str, List[str]] = Chain[str, str](
-        ...         "WordChain", lambda word: as_async_generator(word, "!")
+        ...     word_stream: Stream[str, List[str]] = Stream[str, str](
+        ...         "WordStream", lambda word: as_async_generator(word, "!")
         ...     ).collect()
-        ...     return await collect_final_output(word_chain("Hi"))
+        ...     return await collect_final_output(word_stream("Hi"))
         ...
         >>> asyncio.run(example())
         [['Hi', '!']]
         """
 
         next_name = f"{self.name}@collect"
 
         async def _collect(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[List[U]], Any]:
-            # First, reyield previous chain so we never block the stream, and collect the results until they are done
+        ) -> AsyncGenerator[StreamOutput[List[U]], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the results until they are done
             iter_u: Iterable[U] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[List[U]], to_reyield)
+                yield cast(StreamOutput[List[U]], to_reyield)
                 iter_u = values
 
             # Then, yield the collected results
             yield self._output_wrap(iter_u, name=next_name)
 
-        return SingleOutputChain[T, List[U]](next_name, _collect)
+        return SingleOutputStream[T, List[U]](next_name, _collect)
 
-    def join(self: "Chain[T, str]", separator="") -> "SingleOutputChain[T, str]":
+    def join(self: "Stream[T, str]", separator="") -> "SingleOutputStream[T, str]":
         """
-        Joins the output of a string-producing chain into a single string.
+        Joins the output of a string-producing stream into a single string.
 
-        The `join` method concatenates each item in the output of the chain, using the
+        The `join` method concatenates each item in the output of the stream, using the
         provided separator between each element. This is particularly useful when working
         with text, and you want to merge all the generated tokens.
 
-        Note that this method blocks until all outputs of the chain are available, as it
+        Note that this method blocks until all outputs of the stream are available, as it
         needs to wait for the complete output to perform the join operation.
 
         Params
         ----------
         separator : str
             A string that will be used as a separator between the elements. Default is an empty string.
 
         Example:
 
-        >>> from litechain import Chain, as_async_generator, join_final_output
+        >>> from langstream import Stream, as_async_generator, join_final_output
         >>> import asyncio
         ...
         >>> async def example():
-        ...     words_chain = Chain[str, str]("WordsChain", lambda sentence: as_async_generator(*sentence.split(" ")))
-        ...     capitalized_chain = words_chain.map(lambda word: word.capitalize())
-        ...     joined_chain = capitalized_chain.join(" ")
-        ...     return await join_final_output(joined_chain("this is an example"))
+        ...     words_stream = Stream[str, str]("WordsStream", lambda sentence: as_async_generator(*sentence.split(" ")))
+        ...     capitalized_stream = words_stream.map(lambda word: word.capitalize())
+        ...     joined_stream = capitalized_stream.join(" ")
+        ...     return await join_final_output(joined_stream("this is an example"))
         ...
         >>> asyncio.run(example())
         'This Is An Example'
         """
 
         next_name = f"{self.name}@join"
 
         async def _join(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[str], Any]:
-            # First, reyield previous chain so we never block the stream, and collect the results until they are done
+        ) -> AsyncGenerator[StreamOutput[str], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the results until they are done
             iter_u: Iterable[str] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[str], to_reyield)
+                yield to_reyield
                 iter_u = values
 
             # Then, return the joined result
             output: str = separator.join(iter_u)
             yield self._output_wrap(output, name=next_name)
 
-        return SingleOutputChain[T, str](next_name, _join)
+        return SingleOutputStream[T, str](next_name, _join)
 
     def gather(
-        self: "Union[Chain[T, AsyncGenerator[ChainOutput[V], Any]], Chain[T, AsyncGenerator[V, Any]]]",
-    ) -> "SingleOutputChain[T, List[List[V]]]":
+        self: "Union[Stream[T, AsyncGenerator[StreamOutput[V], Any]], Stream[T, AsyncGenerator[V, Any]]]",
+    ) -> "SingleOutputStream[T, List[List[V]]]":
         """
-        Gathers results from multiple chains and processes them in parallel.
+        Gathers results from multiple streams and processes them in parallel.
 
-        The `gather` method is used to process several chains concurrently, and it waits until all of
+        The `gather` method is used to process several streams concurrently, and it waits until all of
         them are complete before continuing. This is similar to `asyncio.gather`, and is useful when you
         want to run multiple asynchronous tasks in parallel and wait for all of them to complete.
 
-        Note that the order of results corresponds to the order of chains passed to the `gather` method.
+        Note that the order of results corresponds to the order of streams passed to the `gather` method.
 
-        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> from langstream import Stream, as_async_generator, collect_final_output
         >>> import asyncio
         ...
         >>> async def delayed_output(x):
         ...     await asyncio.sleep(0.1)
         ...     yield f"Number: {x}"
         ...
         >>> async def example():
-        ...     number_chain = Chain[int, int](
-        ...         "NumberChain", lambda x: as_async_generator(*range(x))
+        ...     number_stream = Stream[int, int](
+        ...         "NumberStream", lambda x: as_async_generator(*range(x))
         ...     )
-        ...     gathered_chain : Chain[int, str] = (
-        ...         number_chain.map(delayed_output)
+        ...     gathered_stream : Stream[int, str] = (
+        ...         number_stream.map(delayed_output)
         ...         .gather()
         ...         .and_then(lambda results: as_async_generator(*(r[0] for r in results)))
         ...     )
-        ...     return await collect_final_output(gathered_chain(3))
+        ...     return await collect_final_output(gathered_stream(3))
         ...
         >>> asyncio.run(example()) # will take 0.1s to finish, not 0.3s, because it runs in parallel
         ['Number: 0', 'Number: 1', 'Number: 2']
         """
         return self.collect().gather()
 
     def on_error(
         self,
-        handler: Callable[[Exception], Union[AsyncGenerator[ChainOutput[V], Any], V]],
-    ) -> "Chain[T, Union[U, V]]":
+        handler: Callable[[Exception], Union[AsyncGenerator[StreamOutput[V], Any], V]],
+    ) -> "Stream[T, Union[U, V]]":
         """
-        Handles any uncaught exceptions that might occur during the execution of the current chain.
+        Handles any uncaught exceptions that might occur during the execution of the current stream.
 
         The `handler` function takes an exception as its argument and returns a new value that
-        will be used as the output of the chain instead of the exception. The function can also re-raise
-        the exception or raise a new one, which will then be propagated further up the chain.
+        will be used as the output of the stream instead of the exception. The function can also re-raise
+        the exception or raise a new one, which will then be propagated further up the stream.
 
         If an exception occurs in the `handler` function itself, it will be propagated without any
         further handling.
 
         Example:
 
-        >>> from litechain import Chain, join_final_output
+        >>> from langstream import Stream, join_final_output
         >>> import asyncio
         ...
         >>> def failed_greeting(name: str):
         ...     raise Exception(f"Giving {name} a cold shoulder")
         ...
         >>> async def example():
-        ...     greet_chain = Chain[str, str](
-        ...         "GreetingChain",
+        ...     greet_stream = Stream[str, str](
+        ...         "GreetingStream",
         ...         failed_greeting
         ...     ).on_error(lambda e: f"Sorry, an error occurred: {str(e)}")
         ...
-        ...     async for output in greet_chain("Alice"):
+        ...     async for output in greet_stream("Alice"):
         ...         print(output)
         ...
         >>> asyncio.run(example())
-        ChainOutput(chain='GreetingChain', data=Exception('Giving Alice a cold shoulder'), final=False)
-        ChainOutput(chain='GreetingChain@on_error', data='Sorry, an error occurred: ...', final=True)
+        StreamOutput(stream='GreetingStream', data=Exception('Giving Alice a cold shoulder'), final=False)
+        StreamOutput(stream='GreetingStream@on_error', data='Sorry, an error occurred: ...', final=True)
         """
 
         next_name = f"{self.name}@on_error"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def on_error(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[Union[U, V]], Any]:
+        ) -> AsyncGenerator[StreamOutput[Union[U, V]], Any]:
             try:
                 async for output in self(input):
-                    yield cast(ChainOutput[Union[U, V]], output)
+                    yield cast(StreamOutput[Union[U, V]], output)
             except Exception as e:
-                yield cast(ChainOutput[Union[U, V]], self._output_wrap(e, final=False))
+                yield cast(StreamOutput[Union[U, V]], self._output_wrap(e, final=False))
                 async for output in self._wrap(handler(e), name=next_name):
-                    yield cast(ChainOutput[Union[U, V]], output)
+                    yield cast(StreamOutput[Union[U, V]], output)
 
-        return Chain[T, Union[U, V]](next_name, lambda input: on_error(input))
+        return Stream[T, Union[U, V]](next_name, lambda input: on_error(input))
 
 
-class SingleOutputChain(Chain[T, U]):
+class SingleOutputStream(Stream[T, U]):
     """"""
 
     _call: Callable[
-        [T], Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U]
+        [T], Union[AsyncGenerator[StreamOutput[U], Any], AsyncGenerator[U, Any], U]
     ]
 
     async def _reyield(
-        self, async_iterable: AsyncGenerator[ChainOutput[U], Any], at: str
-    ) -> AsyncGenerator[Tuple[Optional[U], ChainOutput[U]], Any]:
+        self, async_iterable: AsyncGenerator[StreamOutput[U], Any]
+    ) -> AsyncGenerator[Tuple[Optional[U], StreamOutput[U]], Any]:
         final_value: Optional[U] = None
         async for u in async_iterable:
             u_rewrapped = self._output_wrap(u, final=False)
             if u.final:
-                if final_value is not None:
-                    # TODO: try to make this happen with a bad use case, is it even breakable?
-                    raise Exception(
-                        f"Expected a single item at the end of SingleOutputChain, found multiple for {self.name}@{at}"
-                    )
                 final_value = u.data
             yield (final_value, u_rewrapped)
 
-    def map(self, fn: Callable[[U], V]) -> "SingleOutputChain[T, V]":
+    def map(self, fn: Callable[[U], V]) -> "SingleOutputStream[T, V]":
         """
-        Similar to `Chain.map`, this method applies a function to the final output of the chain, but returns a SingleOutputChain.
+        Similar to `Stream.map`, this method applies a function to the final output of the stream, but returns a SingleOutputStream.
 
         The `fn` parameter is a function that takes a value of type U and returns a value of type V.
 
-        For detailed examples, refer to the documentation of `Chain.map`.
+        For detailed examples, refer to the documentation of `Stream.map`.
         """
 
         next_name = f"{self.name}@map"
 
-        async def map(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
-            # Reyield previous chain so we never block the stream, and at the same time yield mapped values
+        async def map(input: T) -> AsyncGenerator[StreamOutput[V], Any]:
+            # Reyield previous stream so we never block the stream, and at the same time yield mapped values
             final_u: Optional[U] = None
-            async for value, to_reyield in self._reyield(self(input), "map"):
-                yield cast(ChainOutput[V], to_reyield)
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(StreamOutput[V], to_reyield)
                 final_u = value
 
-            if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@map"
-                )
-            yield self._output_wrap(fn(final_u), name=next_name)
+            yield self._output_wrap(fn(unwrap(final_u)), name=next_name)
+
+        return SingleOutputStream[T, V](next_name, lambda input: map(input))
+
+    def filter(self, fn: Callable[[U], bool]) -> "SingleOutputStream[T, Union[U, None]]":
+        """
+        Similar to `Stream.filter`, however, singe SingleOutputStream must always produce a value, this method simply replaces
+        the value with a None if the filter function returns False
+
+        The `fn` parameter is a function that takes a value of type U and returns a bool.
+
+        Example:
+
+        >>> from langstream import Stream, as_async_generator, collect_final_output
+        >>> import asyncio
+        ...
+        >>> async def example():
+        ...     numbers_stream = Stream[int, int]("NumbersStream", lambda input: as_async_generator(*range(0, input)))
+        ...     even_stream = numbers_stream.collect().filter(lambda numbers: all([n % 2 == 0 for n in numbers]))
+        ...     return await collect_final_output(even_stream(9))
+        ...
+        >>> asyncio.run(example())
+        [None]
+        """
+        next_name = f"{self.name}@filter"
+
+        async def filter(input: T) -> AsyncGenerator[StreamOutput[Union[U, None]], Any]:
+            # Reyield previous stream so we never block the stream, and at the same time yield filtered values
+            final_u: Optional[U] = None
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(StreamOutput[Union[U, None]], to_reyield)
+                final_u = value
 
-        return SingleOutputChain[T, V](next_name, lambda input: map(input))
+            yield self._output_wrap(
+                final_u if fn(unwrap(final_u)) else None, name=next_name
+            )
+
+        return SingleOutputStream[T, Union[U, None]](
+            next_name, lambda input: filter(input)
+        )
 
     def and_then(
         self,
         next: Callable[
             [U],
-            Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
+            Union[AsyncGenerator[StreamOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
-    ) -> "Chain[T, V]":
+    ) -> "Stream[T, V]":
         """
-        Similar to `Chain.and_then`, this method takes a function that receives the final output of this chain as its input and returns a new Chain.
+        Similar to `Stream.and_then`, this method takes a function that receives the final output of this stream as its input and returns a new Stream.
 
-        For detailed examples, refer to the documentation of `Chain.and_then`.
+        For detailed examples, refer to the documentation of `Stream.and_then`.
         """
         next_name = f"{self.name}@and_then"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def and_then(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[V], Any]:
-            # First, reyield previous chain so we never block the stream, and collect the last result when it is done
+        ) -> AsyncGenerator[StreamOutput[V], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the last result when it is done
             final_u: Optional[U] = None
-            async for value, to_reyield in self._reyield(self(input), "and_then"):
-                yield cast(ChainOutput[V], to_reyield)
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(StreamOutput[V], to_reyield)
                 final_u = value
 
-            if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@and_then"
-                )
-
-            # Then, call in the next chain
-            iter_v = self._wrap(next(final_u), name=next_name)
+            # Then, call in the next stream
+            iter_v = self._wrap(next(unwrap(final_u)), name=next_name)
             async for v in iter_v:
                 yield v
 
-        return Chain[T, V](next_name, and_then)
+        return Stream[T, V](next_name, and_then)
+
+    def pipe(
+        self,
+        fn: Callable[
+            [AsyncGenerator[U, Any]], AsyncGenerator[Union[StreamOutput[V], V], Any]
+        ],
+    ) -> "Stream[T, V]":
+        """
+        Similar to `Stream.pipe`, except that it takes a stream that will only even produce a single value, so it effectively works basically the same as `and_then`, only with a different interface.
+
+        For detailed examples, refer to the documentation of `Stream.pipe`.
+        """
+        next_name = f"{self.name}@pipe"
+        if hasattr(next, "name"):
+            next_name = next.name
+
+        async def pipe(
+            input: T,
+        ) -> AsyncGenerator[StreamOutput[V], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the last result when it is done
+            final_u: Optional[U] = None
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(StreamOutput[V], to_reyield)
+                final_u = value
+
+            # Then, call in the piping function
+            single_item_stream = as_async_generator(unwrap(final_u))
+            iter_v = self._wrap(fn(single_item_stream), name=next_name)
+            async for v in iter_v:
+                yield cast(StreamOutput[V], v)
+
+        return Stream[T, V](next_name, pipe)
 
     def gather(
-        self: "Union[SingleOutputChain[T, List[AsyncGenerator[ChainOutput[V], Any]]], SingleOutputChain[T, List[AsyncGenerator[V, Any]]]]",
-    ) -> "SingleOutputChain[T, List[List[V]]]":
+        self: "Union[SingleOutputStream[T, List[AsyncGenerator[StreamOutput[V], Any]]], SingleOutputStream[T, List[AsyncGenerator[V, Any]]]]",
+    ) -> "SingleOutputStream[T, List[List[V]]]":
         """
-        Similar to `Chain.gather`, this method waits for all the async generators in the list returned by the chain to finish and gathers their results in a list.
+        Similar to `Stream.gather`, this method waits for all the async generators in the list returned by the stream to finish and gathers their results in a list.
 
-        For detailed examples, refer to the documentation of `Chain.gather`.
+        For detailed examples, refer to the documentation of `Stream.gather`.
         """
 
         next_name = f"{self.name}@gather"
 
         async def gather(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[List[List[V]]], Any]:
-            # First, reyield previous chain so we never block the stream, and collect the last result when it is done
+        ) -> AsyncGenerator[StreamOutput[List[List[V]]], Any]:
+            # First, reyield previous stream so we never block the stream, and collect the last result when it is done
             final_u: Optional[
                 Union[
-                    List[AsyncGenerator[ChainOutput[V], Any]],
+                    List[AsyncGenerator[StreamOutput[V], Any]],
                     List[AsyncGenerator[V, Any]],
                 ]
             ] = None
 
             # TODO: try to work out why the type signature of self(input) is not fitting in there, it should
-            async for value, to_reyield in self._reyield(
-                cast(Any, self(input)), "gather"
-            ):
-                yield cast(ChainOutput[List[List[V]]], to_reyield)
+            async for value, to_reyield in self._reyield(cast(Any, self(input))):
+                yield cast(StreamOutput[List[List[V]]], to_reyield)
                 final_u = value
 
             if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@gather"
-                )
+                final_u = []
 
             async def consume_async_generator(
                 generator: AsyncGenerator[X, Any],
             ) -> Iterable[X]:
                 return [item async for item in generator]
 
             # TODO: should we really wait for everything to arrive before calling asyncio gather? Can we call it during the previous reyield?
             vss: Union[
-                List[List[ChainOutput[V]]], List[List[V]]
+                List[List[StreamOutput[V]]], List[List[V]]
             ] = await asyncio.gather(*(consume_async_generator(gen) for gen in final_u))
 
             clean_vss: List[List[V]] = []
             for vs in vss:
                 clean_vs: List[V] = []
                 for v in vs:
                     v_rewrapped = cast(
-                        ChainOutput[List[List[V]]],
+                        StreamOutput[List[List[V]]],
                         self._output_wrap(v, final=False),
                     )
-                    if isinstance(v, ChainOutput):
+                    if isinstance(v, StreamOutput):
                         yield v_rewrapped
                         if v.final:
                             clean_vs.append(v.data)
                     else:
                         clean_vs.append(v)
                 clean_vss.append(clean_vs)
 
             yield self._output_wrap(clean_vss, name=next_name)
 
-        return SingleOutputChain[T, List[List[V]]](next_name, gather)
+        return SingleOutputStream[T, List[List[V]]](next_name, gather)
 
     def on_error(
         self,
-        handler: Callable[[Exception], Union[AsyncGenerator[ChainOutput[V], Any], V]],
-    ) -> "SingleOutputChain[T, Union[U, V]]":
+        handler: Callable[[Exception], Union[AsyncGenerator[StreamOutput[V], Any], V]],
+    ) -> "SingleOutputStream[T, Union[U, V]]":
         """
-        Similar to `Chain.on_error`, this method handles any uncaught exceptions that might occur during the execution of the current chain.
+        Similar to `Stream.on_error`, this method handles any uncaught exceptions that might occur during the execution of the current stream.
 
-        For detailed examples, refer to the documentation of `Chain.gather`.
+        For detailed examples, refer to the documentation of `Stream.gather`.
         """
 
         next_name = f"{self.name}@on_error"
         if hasattr(next, "name"):
             next_name = next.name
 
         async def on_error(
             input: T,
-        ) -> AsyncGenerator[ChainOutput[Union[U, V]], Any]:
+        ) -> AsyncGenerator[StreamOutput[Union[U, V]], Any]:
             try:
                 async for output in self(input):
-                    yield cast(ChainOutput[Union[U, V]], output)
+                    yield cast(StreamOutput[Union[U, V]], output)
             except Exception as e:
                 async for output in self._wrap(handler(e), name=next_name):
-                    yield cast(ChainOutput[Union[U, V]], output)
+                    yield cast(StreamOutput[Union[U, V]], output)
 
-        return SingleOutputChain[T, Union[U, V]](
+        return SingleOutputStream[T, Union[U, V]](
             next_name, lambda input: on_error(input)
         )
```

### Comparing `langstream-0.1.5/setup.py` & `langstream-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,25 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="langstream",
-    version="0.1.5",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
-    keywords="chain llm ai stream functional programming",
-    url="https://github.com/rogeriochaves/litechain",
+    keywords="stream llm ai stream functional programming",
+    url="https://github.com/rogeriochaves/langstream",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
@@ -32,13 +32,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.6",
     project_urls={
-        "Documentation": "https://rogeriochaves.github.io/litechain/",
-        "Source Code": "https://github.com/rogeriochaves/litechain",
-        "Issue Tracker": "https://github.com/rogeriochaves/litechain/issues",
+        "Documentation": "https://rogeriochaves.github.io/langstream/",
+        "Source Code": "https://github.com/rogeriochaves/langstream",
+        "Issue Tracker": "https://github.com/rogeriochaves/langstream/issues",
     },
     include_package_data=True,
 )
```

