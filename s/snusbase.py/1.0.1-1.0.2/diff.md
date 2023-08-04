# Comparing `tmp/snusbase.py-1.0.1.tar.gz` & `tmp/snusbase.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snusbase.py-1.0.1.tar", last modified: Wed Jul 26 06:54:26 2023, max compression
+gzip compressed data, was "snusbase.py-1.0.2.tar", last modified: Fri Aug  4 10:12:07 2023, max compression
```

## Comparing `snusbase.py-1.0.1.tar` & `snusbase.py-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1072 2023-07-26 06:27:18.000000 snusbase.py-1.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-07-26 06:19:01.000000 snusbase.py-1.0.1/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2010 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1103 2023-07-26 06:54:01.000000 snusbase.py-1.0.1/README.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-07-26 06:37:49.000000 snusbase.py-1.0.1/requirements.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1628 2023-07-26 06:50:32.000000 snusbase.py-1.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.487921 snusbase.py-1.0.1/snusbase/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      214 2023-07-26 06:54:18.000000 snusbase.py-1.0.1/snusbase/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6522 2023-07-26 06:44:44.000000 snusbase.py-1.0.1/snusbase/client.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      195 2023-07-26 06:43:50.000000 snusbase.py-1.0.1/snusbase/errors.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/snusbase.py.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2010 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      289 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-04 10:12:07.216525 snusbase.py-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-08-04 09:32:09.000000 snusbase.py-1.0.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1815 2023-08-04 10:12:07.212525 snusbase.py-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      739 2023-08-04 09:55:32.000000 snusbase.py-1.0.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1367 2023-08-04 09:51:04.000000 snusbase.py-1.0.2/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-04 10:12:07.216525 snusbase.py-1.0.2/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-04 10:12:07.212525 snusbase.py-1.0.2/snusbase/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-08-04 10:11:10.000000 snusbase.py-1.0.2/snusbase/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5201 2023-08-04 09:47:03.000000 snusbase.py-1.0.2/snusbase/api.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-04 10:12:07.212525 snusbase.py-1.0.2/snusbase.py.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1815 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      281 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-08-04 10:12:07.000000 snusbase.py-1.0.2/snusbase.py.egg-info/top_level.txt
```

### Comparing `snusbase.py-1.0.1/LICENSE` & `snusbase.py-1.0.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 ignacio leandro
+Copyright (c) 2023 Jordan Ignacio
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `snusbase.py-1.0.1/PKG-INFO` & `snusbase.py-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,41 @@
 Metadata-Version: 2.1
 Name: snusbase.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: an un-official async wrapper for the Snusbase API
-Author: igna
-License: MIT
-Project-URL: Website, https://snusbase.com
-Project-URL: Issue tracker, https://github.com/obstructive/snusbase.py
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Author-email: igna <igna@shiro.wtf>
+Maintainer-email: igna <igna@shiro.wtf>
+Project-URL: Homepage, https://snusbase.com
+Project-URL: Bug Reports, https://github.com/obstructive/snusbase.py/issues
+Project-URL: Source, https://github.com/obstructive/snusbase.py
+Keywords: snusbase,osint
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
-snusbase.py
-================
-
-   an un-official async wrapper for the Snusbase API
-
-Features
-========
-
-- none. just easier to use instead of ugly non-async examples
-
-Install
-=======
-
-.. code:: sh
-
-   # Linux/macOS
-   python3 -m pip install -U snusbase.py
-
-   # Windows
-   py -3 -m pip install -U snusbase.py
-
-To install the development version, do the following:
-
-.. code:: sh
-
-    $ pip install -U git+https://github.com/obstructive/snusbase.py
-
-Optional Packages
------------------
-
--  `aiodns <https://pypi.org/project/aiodns>`__,
-   `brotlipy <https://pypi.org/project/brotlipy>`__,
-   `cchardet <https://pypi.org/project/cchardet>`__ (for aiohttp
-   speedup)
-
-Quick Example
-=============
-
-.. code:: py
-
-   from snusbase import SnusbaseAPI
-   from asyncio import get_event_loop
-
-   client = SnusbaseAPI("token")
-
-
-   async def main():
-       result = await client.search_by_username("example")
-       print(result)
-
-
-   loop = get_event_loop()
-   loop.run_until_complete(main())
+# snusbase.py
 
-Links
-=====
--  `Issues <https://github.com/obstructive/snusbase.py>`__
--  `Snusbase API <https://docs.snusbase.com/>`__
+[![PyPI - Python][python-badge]][python-link]
+[![PyPI - License][license-badge]](LICENSE)
+[![PyPI - Version][version-badge]][semver-link]
+[![PyPI - Status][status-badge]][pypi-link]
+
+[python-badge]:  https://img.shields.io/pypi/pyversions/snusbase.py?style=flat-square&label=Python%20version
+[python-link]:   https://python.org
+[license-badge]: https://img.shields.io/pypi/l/snusbase.py?style=flat-square&label=License
+[version-badge]: https://img.shields.io/pypi/v/snusbase.py?style=flat-square&label=PyPI%20package%20version
+[semver-link]:   https://semver.org
+[status-badge]:  https://img.shields.io/pypi/status/snusbase.py?style=flat-square&&label=PyPI%20Status
+[pypi-link]:     https://pypi.python.org/pypi/snusbase.py
```

### Comparing `snusbase.py-1.0.1/snusbase/client.py` & `snusbase.py-1.0.2/snusbase/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,175 @@
-import aiohttp
-import orjson
-from typing import List, Dict, Union
-from pydantic import BaseModel
-from .errors import NoResponse
-
-
-class SearchResult(BaseModel):
-    """A class representing a search result."""
-
-    username: str
-    email: str
-    name: str
-    created: str
-    followers: str
-    hash: str
-    uid: str
-    regdate: str
-    lastip: str
-    id: str
-    date: str
-    salt: str
-
-
-class SearchResults(BaseModel):
-    """A class representing a collection of search results."""
-
-    results: Dict[str, List[SearchResult]]
-
-
-class SnusbaseAPI:
-    """A class for interacting with the Snusbase API."""
-
-    def __init__(self, api_key: str):
-        """
-        Initialize the SnusbaseAPI instance.
-
-        Args:
-            api_key (str): The API key for authentication.
-        """
-        self.api_key = api_key
-        self.base_url = 'https://api-experimental.snusbase.com'
-        self.headers = {
-            'Auth': self.api_key,
-            'Content-Type': 'application/json',
-        }
-
-    async def _request(
-        self, method: str, endpoint: str, params=None, data=None
-    ) -> Dict[str, Union[str, List[SearchResult]]]:
-        """
-        Send a request to the Snusbase API.
-
-        Args:
-            method (str): The HTTP method for the request (e.g., 'GET', 'POST').
-            endpoint (str): The API endpoint to access.
-            params (dict, optional): Query parameters for the request.
-            data (dict, optional): JSON data for the request payload.
-
-        Returns:
-            dict: The response data as a dictionary.
-
-        Raises:
-            aiohttp.ClientError: If there is an error in the request.
-        """
-        url = f'{self.base_url}{endpoint}'
-        async with aiohttp.ClientSession() as session:
-            async with session.request(
-                method, url, headers=self.headers, params=params, json=data
-            ) as response:
-                if not response:
-                    raise NoResponse(
-                        "The API didn't return anything or got no response."
-                    )
-                return await response.json(loads=orjson.loads)
-
-    async def search(self, term: str, search_type: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a term.
-
-        Args:
-            term (str): The term to search for.
-            search_type (str): The type of search to perform (e.g., 'username', 'password').
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        endpoint = '/data/search'
-        data = {'terms': [term], 'types': [search_type]}
-        return SearchResults(
-            results=await self._request('POST', endpoint, data=data)
-        )
-
-    async def hash_lookup(self, _hash: str) -> SearchResults:
-        """
-        Lookup a hash in the Snusbase database.
-
-        Args:
-            hash (str): The hash to lookup.
-
-        Returns:
-            SearchResults: The response data containing the hash lookup results.
-        """
-        endpoint = '/tools/hash-lookup'
-        data = {
-            'terms': [_hash],
-            'types': ['hash'],
-        }
-        return SearchResults(
-            results=await self._request('POST', endpoint, data=data)
-        )
-
-    async def ip_lookup(self, ip: str) -> SearchResults:
-        """
-        Lookup an IP address in the Snusbase database.
-
-        Args:
-            ip (str): The IP address to lookup.
-
-        Returns:
-            SearchResults: The response data containing the IP address lookup results.
-        """
-        endpoint = '/tools/ip-whois'
-        data = {
-            'terms': [ip],
-        }
-        return SearchResults(
-            results=await self._request('POST', endpoint, data=data)
-        )
-
-    async def search_by_username(self, username: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a username.
-
-        Args:
-            username (str): The username to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(username, 'username')
-
-    async def search_by_password(self, password: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a password.
-
-        Args:
-            password (str): The password to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(password, 'password')
-
-    async def search_by_email(self, email: str) -> SearchResults:
-        """
-        Search Snusbase for data related to an email address.
-
-        Args:
-            email (str): The email address to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(email, 'email')
-
-    async def search_by_ip(self, ip: str) -> SearchResults:
-        """
-        Search Snusbase for data related to an IP address.
-
-        Args:
-            ip (str): The IP address to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(ip, 'lastip')
-
-    async def search_by_name(self, name: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a name.
-
-        Args:
-            name (str): The name to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(name, 'name')
-
-    async def search_by_hash(self, _hash: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a hash.
-
-        Args:
-            hash (str): The hash to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(_hash, 'hash')
-
-    async def search_by_wildcard(self, wildcard: str) -> SearchResults:
-        """
-        Search Snusbase for data related to a wildcard.
-
-        Args:
-            wildcard (str): The wildcard to search for.
-
-        Returns:
-            SearchResults: The response data containing the search results.
-        """
-        return await self.search(wildcard, 'wildcard')
+import httpx
+import orjson
+
+
+class SnusbaseClient:
+    """A class for interacting with the Snusbase API."""
+
+    def __init__(self, api_key: str) -> None:
+        """
+        Initialize the SnusbaseClient instance.
+
+        Args:
+            api_key (str): The API key for authentication.
+        """
+        self.api_key = api_key
+        self.base_url = "https://api.snusbase.com"
+        self.headers = {
+            "Auth": self.api_key,
+            "Content-Type": "application/json",
+        }
+        self.session = httpx.AsyncClient(headers=self.headers, timeout=30)
+
+    async def _request(
+        self, method: str, endpoint: str, params=None, data=None
+    ) -> dict:
+        """
+        Send a request to the Snusbase API.
+
+        Args:
+            method (str): The HTTP method for the request (e.g., 'GET', 'POST').
+            endpoint (str): The API endpoint to access.
+            params (dict, optional): Query parameters for the request.
+            data (dict, optional): JSON data for the request payload.
+
+        Returns:
+            dict: The response data as a dictionary.
+
+        Raises:
+            aiohttp.ClientError: If there is an error in the request.
+        """
+        url = f"{self.base_url}{endpoint}"
+        request = await self.session.request(method, url, params=params, json=data)
+        return orjson.loads(request.content)
+
+    async def search(self, term: str, search_type: str) -> dict:
+        """
+        Search Snusbase for data related to a term.
+
+        Args:
+            term (str): The term to search for.
+            search_type (str): The type of search to perform.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        endpoint = "/data/search"
+        data = {"terms": [term], "types": [search_type]}
+        return await self._request("POST", endpoint, data=data)
+
+    async def hash_lookup(self, _hash: str) -> dict:
+        """
+        Search Snusbase for data related to a hash.
+
+        Args:
+            hash (str): The hash to lookup.
+
+        Returns:
+            dict: The response data containing the hash lookup results.
+        """
+        endpoint = "/tools/hash-lookup"
+        data = {
+            "terms": [_hash],
+            "types": ["hash"],
+        }
+        return await self._request("POST", endpoint, data=data)
+
+    async def ip_lookup(self, ip: str) -> dict:
+        """
+        Search Snusbase for data related to an IP address.
+
+        Args:
+            ip (str): The IP address to lookup.
+
+        Returns:
+            dict: The response data containing the IP address lookup results.
+        """
+        endpoint = "/tools/ip-whois"
+        data = {
+            "terms": [ip],
+        }
+        return await self._request("POST", endpoint, data=data)
+
+    async def search_by_username(self, username: str) -> dict:
+        """
+        Search Snusbase for data related to a username.
+
+        Args:
+            username (str): The username to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(username, "username")
+
+    async def search_by_password(self, password: str) -> dict:
+        """
+        Search Snusbase for data related to a password.
+
+        Args:
+            password (str): The password to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(password, "password")
+
+    async def search_by_email(self, email: str) -> dict:
+        """
+        Search Snusbase for data related to an email address.
+
+        Args:
+            email (str): The email address to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(email, "email")
+
+    async def search_by_ip(self, ip: str) -> dict:
+        """
+        Search Snusbase for data related to an IP address.
+
+        Args:
+            ip (str): The IP address to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(ip, "lastip")
+
+    async def search_by_name(self, name: str) -> dict:
+        """
+        Search Snusbase for data related to a name.
+
+        Args:
+            name (str): The name to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(name, "name")
+
+    async def search_by_hash(self, _hash: str) -> dict:
+        """
+        Search Snusbase for data related to a hash.
+
+        Args:
+            hash (str): The hash to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(_hash, "hash")
+
+    async def search_by_wildcard(self, wildcard: str) -> dict:
+        """
+        Search Snusbase for data related to a wildcard.
+
+        Args:
+            wildcard (str): The wildcard to search for.
+
+        Returns:
+            dict: The response data containing the search results.
+        """
+        return await self.search(wildcard, "wildcard")
```

### Comparing `snusbase.py-1.0.1/snusbase.py.egg-info/PKG-INFO` & `snusbase.py-1.0.2/snusbase.py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,41 @@
 Metadata-Version: 2.1
 Name: snusbase.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: an un-official async wrapper for the Snusbase API
-Author: igna
-License: MIT
-Project-URL: Website, https://snusbase.com
-Project-URL: Issue tracker, https://github.com/obstructive/snusbase.py
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Author-email: igna <igna@shiro.wtf>
+Maintainer-email: igna <igna@shiro.wtf>
+Project-URL: Homepage, https://snusbase.com
+Project-URL: Bug Reports, https://github.com/obstructive/snusbase.py/issues
+Project-URL: Source, https://github.com/obstructive/snusbase.py
+Keywords: snusbase,osint
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
-snusbase.py
-================
-
-   an un-official async wrapper for the Snusbase API
-
-Features
-========
-
-- none. just easier to use instead of ugly non-async examples
-
-Install
-=======
-
-.. code:: sh
-
-   # Linux/macOS
-   python3 -m pip install -U snusbase.py
-
-   # Windows
-   py -3 -m pip install -U snusbase.py
-
-To install the development version, do the following:
-
-.. code:: sh
-
-    $ pip install -U git+https://github.com/obstructive/snusbase.py
-
-Optional Packages
------------------
-
--  `aiodns <https://pypi.org/project/aiodns>`__,
-   `brotlipy <https://pypi.org/project/brotlipy>`__,
-   `cchardet <https://pypi.org/project/cchardet>`__ (for aiohttp
-   speedup)
-
-Quick Example
-=============
-
-.. code:: py
-
-   from snusbase import SnusbaseAPI
-   from asyncio import get_event_loop
-
-   client = SnusbaseAPI("token")
-
-
-   async def main():
-       result = await client.search_by_username("example")
-       print(result)
-
-
-   loop = get_event_loop()
-   loop.run_until_complete(main())
+# snusbase.py
 
-Links
-=====
--  `Issues <https://github.com/obstructive/snusbase.py>`__
--  `Snusbase API <https://docs.snusbase.com/>`__
+[![PyPI - Python][python-badge]][python-link]
+[![PyPI - License][license-badge]](LICENSE)
+[![PyPI - Version][version-badge]][semver-link]
+[![PyPI - Status][status-badge]][pypi-link]
+
+[python-badge]:  https://img.shields.io/pypi/pyversions/snusbase.py?style=flat-square&label=Python%20version
+[python-link]:   https://python.org
+[license-badge]: https://img.shields.io/pypi/l/snusbase.py?style=flat-square&label=License
+[version-badge]: https://img.shields.io/pypi/v/snusbase.py?style=flat-square&label=PyPI%20package%20version
+[semver-link]:   https://semver.org
+[status-badge]:  https://img.shields.io/pypi/status/snusbase.py?style=flat-square&&label=PyPI%20Status
+[pypi-link]:     https://pypi.python.org/pypi/snusbase.py
```

