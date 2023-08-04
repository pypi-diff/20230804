# Comparing `tmp/rebelai-1.2.0-py2.py3-none-any.whl.zip` & `tmp/rebelai-2.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 23085 bytes, number of entries: 17
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-31 16:09 rebelai/__init__.py
--rw-r--r--  2.0 unx     2002 b- defN 23-Jul-30 19:36 rebelai/const.py
+Zip file size: 24470 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      129 b- defN 23-Aug-04 13:11 rebelai/__init__.py
+-rw-r--r--  2.0 unx     2250 b- defN 23-Aug-04 13:12 rebelai/const.py
 -rw-r--r--  2.0 unx     3555 b- defN 23-Jul-30 19:35 rebelai/enums.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/py.typed
 -rw-r--r--  2.0 unx       81 b- defN 23-Jul-31 14:47 rebelai/ai/__init__.py
--rw-r--r--  2.0 unx      810 b- defN 23-Jul-30 19:26 rebelai/ai/alpaca.py
--rw-r--r--  2.0 unx     1700 b- defN 23-Jul-30 19:27 rebelai/ai/deepai.py
--rw-r--r--  2.0 unx     4560 b- defN 23-Jul-31 16:08 rebelai/ai/gpt.py
--rw-r--r--  2.0 unx      720 b- defN 23-Jul-30 19:28 rebelai/ai/pollinations.py
--rw-r--r--  2.0 unx     2919 b- defN 23-Jul-30 19:29 rebelai/ai/prodia.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Aug-04 13:09 rebelai/ai/alpaca.py
+-rw-r--r--  2.0 unx     2016 b- defN 23-Aug-04 12:41 rebelai/ai/deepai.py
+-rw-r--r--  2.0 unx     4772 b- defN 23-Aug-04 13:22 rebelai/ai/gpt.py
+-rw-r--r--  2.0 unx     2338 b- defN 23-Aug-04 13:18 rebelai/ai/inferkit.py
+-rw-r--r--  2.0 unx     1034 b- defN 23-Aug-04 13:10 rebelai/ai/pollinations.py
+-rw-r--r--  2.0 unx     3063 b- defN 23-Aug-04 13:10 rebelai/ai/prodia.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/ai/py.typed
--rw-------  2.0 unx    35115 b- defN 23-Jul-31 16:09 rebelai-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3091 b- defN 23-Jul-31 16:09 rebelai-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-31 16:09 rebelai-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-31 16:09 rebelai-1.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-1.2.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1300 b- defN 23-Jul-31 16:09 rebelai-1.2.0.dist-info/RECORD
-17 files, 56101 bytes uncompressed, 20967 bytes compressed:  62.6%
+-rw-------  2.0 unx    35115 b- defN 23-Aug-04 13:23 rebelai-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3176 b- defN 23-Aug-04 13:23 rebelai-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-04 13:23 rebelai-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-04 13:23 rebelai-2.0.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-2.0.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Aug-04 13:23 rebelai-2.0.0.dist-info/RECORD
+18 files, 60089 bytes uncompressed, 22232 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -18,35 +18,38 @@
 
 Filename: rebelai/ai/deepai.py
 Comment: 
 
 Filename: rebelai/ai/gpt.py
 Comment: 
 
+Filename: rebelai/ai/inferkit.py
+Comment: 
+
 Filename: rebelai/ai/pollinations.py
 Comment: 
 
 Filename: rebelai/ai/prodia.py
 Comment: 
 
 Filename: rebelai/ai/py.typed
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/LICENSE
+Filename: rebelai-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/METADATA
+Filename: rebelai-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/WHEEL
+Filename: rebelai-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/top_level.txt
+Filename: rebelai-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/zip-safe
+Filename: rebelai-2.0.0.dist-info/zip-safe
 Comment: 
 
-Filename: rebelai-1.2.0.dist-info/RECORD
+Filename: rebelai-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rebelai/__init__.py

```diff
@@ -1,5 +1,5 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """rebelai -- providing free ai access to everyone"""
 
-__version__: str = "1.2.0"
+__version__: str = "2.0.0"
```

## rebelai/const.py

```diff
@@ -36,7 +36,14 @@
 DEFAULT_PRODIA_SLEEP: Final[int] = 1
 
 DEFAULT_DEEPAI_USER_AGENT: Final[
     str
 ] = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, \
 like Gecko) Chrome/111.0.0.0 Safari/537.36"
 DEFAULT_DEEPAI_API: Final[str] = "https://api.deepai.org/api"
+
+DEFAULT_INFERKIT_STARNDARD_API: Final[
+    str
+] = "https://api.inferkit.com/v1/models/standard/generate?useDemoCredits=true"
+DEFAULT_INFERKIT_LEN: Final[int] = 200
+DEFAULT_INFERKIT_TEMP: Final[float] = 1
+DEFAULT_INFERKIT_PROB: Final[float] = 0.9
```

## rebelai/ai/alpaca.py

```diff
@@ -1,34 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """alpaca models"""
 
 import typing
 
-import requests
+import aiohttp
 
 from .. import const
 
 
-def alpaca_7b(
+async def alpaca_7b(
     prompt: str,
     api: str = const.DEFAULT_ALPACA_7B_API,
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
+    session_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> typing.Optional[str]:
-    """alpaca ( 7 bilion neuron ) access
+    """alpaca generation model ( 7 bilion neuron ) access
 
     *prompt(str): the prompt passed to the ai
     api(str): api url for the alpaca model
-    request_args(dict[str, Any] | None): arguments passed to `requests.post()`
+    request_args(dict[str, Any] | None): arguments passed to `session.post()`
+    session_args(dict[str, Any] | None): arguments passed to `aiohttp.ClientSession()`
 
     return(str | None): the ai output as a string or nothing if no output was
                         generated"""
 
-    return (
-        requests.post(
-            api,
-            json={"prompt": prompt},
-            **(request_args or {}),
-        )
-        .json()
-        .get("completion")
-    )
+    async with aiohttp.ClientSession(**(session_args or {})) as session:
+        async with session.post(
+            api, json={"prompt": prompt}, **(request_args or {})
+        ) as response:
+            return (await response.json()).get("completion")
```

## rebelai/ai/deepai.py

```diff
@@ -2,49 +2,53 @@
 # -*- coding: utf-8 -*-
 """deepai models"""
 
 import random
 import typing
 from hashlib import md5
 
-import requests
+import aiohttp
 
 from .. import const, enums
 
 
-def deepai(
+async def deepai(
     model: enums.DeepAIModel,
     data: typing.Dict[str, typing.Any],
     api_key: typing.Optional[str] = None,
     user_agent: str = const.DEFAULT_DEEPAI_USER_AGENT,
     headers: typing.Optional[typing.Dict[str, typing.Any]] = None,
     api: str = const.DEFAULT_DEEPAI_API,
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
+    session_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> typing.Dict[str, typing.Any]:
     """multiple deepai model access ( proxies highly suggested )
 
-    *model(..enums.DeepAIModel): the deepai model youre using
+    *model(..enums.DeepAIModel): the deepai model you're using
     *data(dict[str, Any]): the form posted to the api ( usually 'text' for prompts )
-    api_key(str | None): optional api key to use, otherwise its generated automatically
+    api_key(str | None): optional api key to use, otherwise it's generated automatically
     user_agent(str): user agent posted in the headers
     headers(dict[str, Any] | None): any other headers
     api(str): the deepai api url
-    request_args(dict[str, Any] | None): arguments passed to `requests.post()`
+    request_args(dict[str, Any] | None): arguments passed to `session.post()`
+    session_args(dict[str, Any] | None): arguments passed to `aiohttp.ClientSession()`
 
-    return(dict[str, Any]): the ai api response as json, `output` is what ur
+    return(dict[str, Any]): the ai api response as json, `output` is what you're
                             looking for usually"""
 
     if api_key is None:
 
         def rev_md5(val: str) -> str:
             return md5(val.encode()).hexdigest()[::-1]
 
         k: int = round(1e11 * random.random())
         api_key = f"tryit-{k}-\
 {rev_md5(user_agent + rev_md5( user_agent + rev_md5(user_agent + str(k) + 'x')))}"
 
-    return requests.post(
-        f"{api}/{model.value}",
-        headers={"api-key": api_key, "user-agent": user_agent, **(headers or {})},
-        **(request_args or {}),
-        data=data,
-    ).json()
+    async with aiohttp.ClientSession(**(session_args or {})) as session:
+        async with session.post(
+            f"{api}/{model.value}",
+            headers={"api-key": api_key, "user-agent": user_agent, **(headers or {})},
+            **(request_args or {}),
+            data=data,
+        ) as response:
+            return await response.json()
```

## rebelai/ai/gpt.py

```diff
@@ -3,110 +3,110 @@
 """gpt models"""
 
 import json
 import typing
 from re import Pattern
 from uuid import uuid4
 
-import requests
-import requests.structures
+import aiohttp
 import tls_client  # type: ignore
 
 from .. import const
 
 
-def gpt3(
+async def gpt3(
     prompt: str,
     api: str = const.DEFAULT_GPT3_API,
     role: str = "user",
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
+    session_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> typing.Optional[str]:
-    """access to the gpt3 model ( proxies suggested )
+    """access to the gpt3 generation model ( proxies suggested )
 
     *prompt(str): the prompt passed to the ai
     role(str): role of the prompt ( usually system or user )
     api(str): api url for the alpaca model
-    request_args(dict[str, Any] | None): arguments passed to `requests.post()`
+    request_args(dict[str, Any] | None): arguments passed to `session.post()`
+    session_args(dict[str, Any] | None): arguments passed to `aiohttp.ClientSession()`
 
     return(str | None): the ai output as a string or nothing if no output was
                         generated"""
 
     content: str = ""
 
-    for line in requests.post(
-        api,
-        json={
-            "stream": True,
-            "messages": [
-                {
-                    "role": role,
-                    "content": prompt,
-                }
-            ],
-        },
-        stream=True,
-        **(request_args or {}),
-    ).iter_lines():
-        line = line.decode()
-
-        if not line.startswith("data:"):
-            continue
-
-        json_data: typing.Dict[str, typing.Any] = json.loads(
-            line.removeprefix("data: ")
-        )
-
-        if "choices" not in json_data:
-            continue
-
-        for choice in json_data["choices"]:
-            if choice.get("finish_reason") == "stop":
-                break
+    async with aiohttp.ClientSession(**(session_args or {})) as session:
+        async with session.post(
+            api,
+            json={
+                "stream": True,
+                "messages": [
+                    {
+                        "role": role,
+                        "content": prompt,
+                    }
+                ],
+            },
+            **(request_args or {}),
+        ) as response:
+            async for line in response.content:
+                ln = line.decode()
+
+                if not ln.startswith("data:"):
+                    continue
+
+                json_data: typing.Dict[str, typing.Any] = json.loads(
+                    line.removeprefix("data: ")  # type: ignore
+                )
+
+                if "choices" not in json_data:
+                    continue
+
+                for choice in json_data["choices"]:
+                    if choice.get("finish_reason") == "stop":
+                        break
 
-            if "delta" in choice and "content" in choice["delta"]:
-                content += choice["delta"]["content"]
+                    if "delta" in choice and "content" in choice["delta"]:
+                        content += choice["delta"]["content"]
 
     return content or None
 
 
-def gpt4(
+async def gpt4(
     prompt: str,
     pattern: Pattern[str] = const.GPT4_PATTERN,
     you_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
     tls_client_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
     client_headers: typing.Optional[typing.Dict[str, typing.Any]] = None,
     client_proxies: typing.Optional[typing.Dict[str, typing.Any]] = None,
     api: str = const.DEFAULT_GPT4_API,
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> typing.Optional[str]:
-    """access to the gpt4 model
+    """access to the gpt4 generation model
 
     *prompt(str): the prompt passed to the ai
     pattern(Pattern[str]): pattern to find all output pieces
     you_params(dict[str, Any] | None): params passed to you.com api
     tls_client_args(dict[str, Any] | None): args passed to `tls_client.Session()`
     client_headers(dict[str, Any] | None): tls client headers in requests
     client_proxies(dict[str, Any] | None): tls client proxies in requests
     api(str): api url for the alpaca model
-    request_args(dict[str, Any] | None): arguments passed to `requests.post()`
-                                         and `requests.get()`
+    request_args(dict[str, Any] | None): arguments passed to `session.post()`
+                                         and `session.get()`
 
     return(str | None): the ai output as a string or nothing if no output was
                         generated"""
 
     client: tls_client.Session = tls_client.Session(
-        client_identifier="chrome_100", **(tls_client_args or {})
+        client_identifier="chrome112", **(tls_client_args or {})
     )
 
-    client.headers = requests.structures.CaseInsensitiveDict(  # type: ignore
+    client.headers = tls_client.sessions.CaseInsensitiveDict(
         {
-            "accept": "text/event-stream",
-            "referer": "https://you.com/search?q=youchat&tbm=youchat",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) \
-AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
+            "referer": "u",
+            "user-agent": "u",
             **(client_headers or {}),
         }
     )
 
     client.proxies = client_proxies or {}
 
     return (
@@ -118,16 +118,16 @@
                         params={
                             "q": prompt,
                             "page": 1,
                             "count": 10,
                             "safeSearch": "Off",
                             "onShoppingPage": False,
                             "mkt": "",
-                            "responseFilter": "WebPages,Translations,TimeZone,Computation,\
-RelatedSearches",
+                            "responseFilter": "WebPages,Translations,TimeZone,\
+Computation,RelatedSearches",
                             "domain": "youchat",
                             "queryTraceId": str(uuid4()),
                             "chat": [],
                             **(you_params or {}),
                         },
                         **(request_args or {}),
                     ).text
```

## rebelai/ai/pollinations.py

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """pollinations image ai"""
 
 import random
 import typing
 
-import requests
+import aiohttp
 
 from .. import const
 
 
-def pollinations(
+async def pollinations(
     prompt: str,
     api: str = const.DEFAULT_POLLINATIONS_API,
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
+    session_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> bytes:
-    """pollinations api access ( proxies suggested + watermark )
+    """pollinations generation model access ( proxies suggested + watermark )
 
     *prompt(str): the prompt passed to the ai
     api(str): api url for the alpaca model
-    request_args(dict[str, Any] | None): arguments passed to `requests.get()`
+    request_args(dict[str, Any] | None): arguments passed to `session.get()`
+    session_args(dict[str, Any] | None): arguments passed to `aiohttp.ClientSession()`
 
     return(bytes): jpeg image as bytes"""
 
-    return requests.get(
-        f"{api}/{prompt}{random.randint(0, 9999999999999)}",
-        **(request_args or {}),
-    ).content
+    async with aiohttp.ClientSession(**(session_args or {})) as session:
+        async with session.get(
+            f"{api}/{prompt}{random.randint(0, 9999999999999)}",
+            **(request_args or {}),
+        ) as response:
+            return await response.read()
```

## rebelai/ai/prodia.py

```diff
@@ -1,85 +1,78 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """prodia image generation api"""
 
+import asyncio
 import random
-import time
 import typing
 
-import requests
+import aiohttp
 
 from .. import const, enums
 
 
-def prodia(
+async def prodia(
     prompt: str,
     model: enums.ProdiaModel = enums.ProdiaModel.REALISTIC_VISION_V5_0,
     steps: int = const.DEFAULT_PRODIA_STEPS,
     cfg: float = const.DEFAULT_PRODIA_CFG,
     seed: int = -1,
     sampler: enums.ProdiaSampler = enums.ProdiaSampler.EULER,
     negative: bool = True,
     negative_prompt: str = const.DEFAULT_PRODIA_NEG,
     image: bool = True,
     sleep: float = const.DEFAULT_PRODIA_SLEEP,
     api: str = const.DEFAULT_PRODIA_API,
     request_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
     session_args: typing.Optional[typing.Dict[str, typing.Any]] = None,
 ) -> bytes:
-    """prodia image api ( proxies dont work + limited uses )
+    """prodia image generation model access ( proxies dont work + limited uses )
 
     *prompt(str): the prompt passed to the ai
     model(..enums.ProdiaModel): the prodia model to use to generate images
     steps(int): generation steps
     cfg(float): how strongly the image should conform to the text
     seed(int): seed to use to generate image ( <0 = random )
     sampler(..enums.ProdiaSampler): algorithm to use to generate the image
     negative(bool): enable / disable negative output filtering
     negative_prompt(str): filter / profile for the negative output
     image(bool): if set to true returns the image as bytes, if not returns the
                  url encoded in bytes ( use `str.decode()` to decode it )
     sleep(float): how much time to sleep between every ping request to the job
     api(str): api url for the alpaca model
-    request_args(dict[str, Any] | None): arguments passed to `requests.get()`
+    request_args(dict[str, Any] | None): arguments passed to `session.get()`
+    session_args(dict[str, Any] | None): arguments passed to `aiohttp.ClientSession()`
 
     return(bytes): jpeg image as bytes if `image` is `True` else image url
                    encoded in utf-8"""
 
     request_args = request_args or {}
-    session: requests.Session = requests.Session(**(session_args or {}))
 
-    job_id: str = session.get(
-        f"{api}/generate",
-        params={
+    async with aiohttp.ClientSession(**(session_args or {})) as session:
+        params = {
             "new": "true",
             "prompt": prompt,
             "model": model.value,
             "negative_prompt": negative_prompt if negative else "",
             "steps": steps,
             "cfg": cfg,
             "seed": random.randint(0, 9999999999999) if seed < 0 else seed,
             "sampler": sampler.value,
             "aspect_ratio": "square",
-        },
-        **request_args,
-    ).json()["job"]
-
-    while True:
-        if (
-            session.get(
-                f"{api}/job/{job_id}",
-                **request_args,
-            ).json()["status"]
-            == "succeeded"
-        ):
-            url: str = f"https://images.prodia.xyz/{job_id}.png?download=1"
-            return (
-                session.get(
-                    url,
-                    **request_args,
-                ).content
-                if image
-                else url.encode()
-            )
+        }
 
-        time.sleep(sleep)
+        async with session.get(
+            f"{api}/generate", params=params, **request_args
+        ) as response:
+            job_id = (await response.json())["job"]
+
+        while True:
+            async with session.get(f"{api}/job/{job_id}", **request_args) as response:
+                status = (await response.json())["status"]
+
+            if status == "succeeded":
+                url = f"https://images.prodia.xyz/{job_id}.png?download=1"
+                async with session.get(url, **request_args) as response:
+                    return await response.read() if image else url.encode()
+
+            await asyncio.sleep(sleep)
```

## Comparing `rebelai-1.2.0.dist-info/LICENSE` & `rebelai-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rebelai-1.2.0.dist-info/METADATA` & `rebelai-2.0.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebelai
-Version: 1.2.0
+Version: 2.0.0
 Summary: providing free access to proprietary ai models in python
 Home-page: https://ari-web.xyz/gh/rebelai
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,api,https,ai,machine learning,openai
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: types-requests
+Requires-Dist: aiohttp
 Requires-Dist: tls-client
 
 # rebelai
 
 > free access to multiple proprietary ai models in python
 
 # mission
@@ -62,13 +61,15 @@
         -   `gpt` -- access to "open"ai models ( kinda )
             -   `gpt3` -- access to gpt3 model
             -   `gpt4` -- access to gpt3 model ( youchat )
         -   `pollinations` -- access to pollinations image generation api
             -   `pollinations` -- access to the generation model
         -   `prodia` -- access to prodia image generation api ( limited access and proxies dont seem to work :( )
             -   `prodia` -- generic function to access prodia api, takes `ProdiaModel` and `ProdiaSampler`, see doc string
+        -   `inferkit` -- access inferkit text completion model
+            -   `standard` -- standard model access
 
 # tips
 
 -   use proxies ( for example gimmeproxy api,, https://gimmeproxy.com/api/getProxy?post=true&get=true&user-agent=true&supportsHttps=true&protocol=http&minSpeed=20&curl=true )
     -   dont forget to test if theyre responsive by making a proxies request to for example https://example.com/
 -   check docstrings, they have info about arguments and proxies
```

## Comparing `rebelai-1.2.0.dist-info/RECORD` & `rebelai-2.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-rebelai/__init__.py,sha256=bfvP2FjJpVkeUyRlX3jz1tUHJzUb5xV4K5pySqjN2rk,129
-rebelai/const.py,sha256=Hb06cmLY_zdHrSI-yQOZPSXvZuYvBZZpAegDLqbWVYc,2002
+rebelai/__init__.py,sha256=-swSl-UBiecvJDE9o5hcAfDDtBbGpBaIE3iYoZXicTE,129
+rebelai/const.py,sha256=4Ewbq3Hn2hEfA0wWrfomf0TfsP_1fbQz6TieYTfGCLM,2250
 rebelai/enums.py,sha256=ehaDobrl6JrhUrX4hd6RPl17UphiMMpBy8WFIeaG72w,3555
 rebelai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rebelai/ai/__init__.py,sha256=wyciqW63L5Z6Sr1SDtNz7Z431UH-J-eejMGeTAaFxBw,81
-rebelai/ai/alpaca.py,sha256=JJQ4bsdoUU0NqdD-1JGOJZX_oB1J9DN7IpkNll1NZxg,810
-rebelai/ai/deepai.py,sha256=3DkuJfB-3S6J2Kyooqv45Q0jOwNla-F6s11SPu5kryk,1700
-rebelai/ai/gpt.py,sha256=VVrsxVW2Lgfvm-02YSVzowkaPmI8LPRj52xvNL_A5Mk,4560
-rebelai/ai/pollinations.py,sha256=TZoHBvo96ZHEo3sOvleefImrh8pq54xBc0Tn5W_70Uo,720
-rebelai/ai/prodia.py,sha256=KOmug7xChH_UoRO49FYQvvsZN2b_XW6nv_nWUHIT7VQ,2919
+rebelai/ai/alpaca.py,sha256=MiKVARRmWXmjm8ZbWdgyoHZyMq4XeIuLgzQkcNDw1UE,1060
+rebelai/ai/deepai.py,sha256=8d8K1zhHAhreiCBivQDYmlq1KjEdlOJgmPfOjpEl0vg,2016
+rebelai/ai/gpt.py,sha256=12hxyDydJCHPlQyQ_FlVfNCd3wckZpJ_KpCunQeA1kE,4772
+rebelai/ai/inferkit.py,sha256=ximoohg7FKwr2uM7blaIijsndMnJ9u3MEK4d3FwOyFA,2338
+rebelai/ai/pollinations.py,sha256=LI68q_TSTwugMPb2dldR5SzTXVZJxIR1qloOjoIAFkY,1034
+rebelai/ai/prodia.py,sha256=nLna4y4lOKPT85VgUNlD_TseQXuxc9wzRLM9y9VZ8lE,3063
 rebelai/ai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rebelai-1.2.0.dist-info/LICENSE,sha256=Rgc3Ns1SKdwsPGFZc5xrgE6-VV8DXkUUgP5FRclaUvk,35115
-rebelai-1.2.0.dist-info/METADATA,sha256=mE6b5fzIHpIRZGZGuQ1kQaFwNTrhVF6j8qRVApkCOIU,3091
-rebelai-1.2.0.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
-rebelai-1.2.0.dist-info/top_level.txt,sha256=rgLyT5avUbh1GgLMKFze_THimdNRD3ht3aiMAF8ysA0,8
-rebelai-1.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-rebelai-1.2.0.dist-info/RECORD,,
+rebelai-2.0.0.dist-info/LICENSE,sha256=Rgc3Ns1SKdwsPGFZc5xrgE6-VV8DXkUUgP5FRclaUvk,35115
+rebelai-2.0.0.dist-info/METADATA,sha256=QApXCNnmgENt_VQOxb__3LI0ReJT6wm3c_b14JCYuUQ,3176
+rebelai-2.0.0.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
+rebelai-2.0.0.dist-info/top_level.txt,sha256=rgLyT5avUbh1GgLMKFze_THimdNRD3ht3aiMAF8ysA0,8
+rebelai-2.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+rebelai-2.0.0.dist-info/RECORD,,
```

