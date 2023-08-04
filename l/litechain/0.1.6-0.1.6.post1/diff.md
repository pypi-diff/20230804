# Comparing `tmp/litechain-0.1.6.tar.gz` & `tmp/litechain-0.1.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.6.tar", last modified: Sun Jul 30 05:55:08 2023, max compression
+gzip compressed data, was "litechain-0.1.6.post1.tar", last modified: Fri Aug  4 06:05:11 2023, max compression
```

## Comparing `litechain-0.1.6.tar` & `litechain-0.1.6.post1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.751570 litechain-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 05:54:53.000000 litechain-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:54:53.000000 litechain-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-30 05:55:08.747570 litechain-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-30 05:54:53.000000 litechain-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30343 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-30 05:54:53.000000 litechain-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:55:08.751570 litechain-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 05:54:53.000000 litechain-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/tests/__init__.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.610833 litechain-0.1.6.post1/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     1070 2023-07-03 19:03:14.000000 litechain-0.1.6.post1/LICENSE
+-rw-r--r--   0 rchavesferna   (502) staff       (20)       24 2023-07-06 16:19:10.000000 litechain-0.1.6.post1/MANIFEST.in
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     1397 2023-08-04 06:05:11.610566 litechain-0.1.6.post1/PKG-INFO
+-rw-r--r--   0 rchavesferna   (502) staff       (20)      104 2023-08-04 05:51:24.000000 litechain-0.1.6.post1/README.md
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.593357 litechain-0.1.6.post1/litechain/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     5009 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/__init__.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.598528 litechain-0.1.6.post1/litechain/contrib/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)      740 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/contrib/__init__.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.603323 litechain-0.1.6.post1/litechain/contrib/llms/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     2950 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)    14052 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.605618 litechain-0.1.6.post1/litechain/core/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/core/__init__.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)    30343 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/core/chain.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.608026 litechain-0.1.6.post1/litechain/utils/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/utils/__init__.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)      151 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/utils/_typing.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     4609 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/utils/async_generator.py
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     6924 2023-08-04 05:50:30.000000 litechain-0.1.6.post1/litechain/utils/chain.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.597767 litechain-0.1.6.post1/litechain.egg-info/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     1397 2023-08-04 06:05:11.000000 litechain-0.1.6.post1/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 rchavesferna   (502) staff       (20)      564 2023-08-04 06:05:11.000000 litechain-0.1.6.post1/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 rchavesferna   (502) staff       (20)        1 2023-08-04 06:05:11.000000 litechain-0.1.6.post1/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 rchavesferna   (502) staff       (20)       93 2023-08-04 06:05:11.000000 litechain-0.1.6.post1/litechain.egg-info/requires.txt
+-rw-r--r--   0 rchavesferna   (502) staff       (20)       16 2023-08-04 06:05:11.000000 litechain-0.1.6.post1/litechain.egg-info/top_level.txt
+-rw-r--r--   0 rchavesferna   (502) staff       (20)      147 2023-07-29 17:50:38.000000 litechain-0.1.6.post1/requirements.txt
+-rw-r--r--   0 rchavesferna   (502) staff       (20)       38 2023-08-04 06:05:11.610898 litechain-0.1.6.post1/setup.cfg
+-rw-r--r--   0 rchavesferna   (502) staff       (20)     1678 2023-08-04 06:05:02.000000 litechain-0.1.6.post1/setup.py
+drwxr-xr-x   0 rchavesferna   (502) staff       (20)        0 2023-08-04 06:05:11.610154 litechain-0.1.6.post1/tests/
+-rw-r--r--   0 rchavesferna   (502) staff       (20)        0 2023-06-23 07:11:41.000000 litechain-0.1.6.post1/tests/__init__.py
```

### Comparing `litechain-0.1.6/LICENSE` & `litechain-0.1.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/__init__.py` & `litechain-0.1.6.post1/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/contrib/__init__.py` & `litechain-0.1.6.post1/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.6.post1/litechain/contrib/llms/gpt4all_chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/contrib/llms/open_ai.py` & `litechain-0.1.6.post1/litechain/contrib/llms/open_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
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
```

### Comparing `litechain-0.1.6/litechain/core/chain.py` & `litechain-0.1.6.post1/litechain/core/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/utils/async_generator.py` & `litechain-0.1.6.post1/litechain/utils/async_generator.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain/utils/chain.py` & `litechain-0.1.6.post1/litechain/utils/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/litechain.egg-info/SOURCES.txt` & `litechain-0.1.6.post1/litechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litechain-0.1.6/setup.py` & `litechain-0.1.6.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.6",
+    version="0.1.6.post1",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

