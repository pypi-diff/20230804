# Comparing `tmp/supabase-1.0.3.tar.gz` & `tmp/supabase-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-1.0.3.tar", max compression
+gzip compressed data, was "supabase-1.0.4.tar", max compression
```

## Comparing `supabase-1.0.3.tar` & `supabase-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1065 2022-10-07 07:13:21.470655 supabase-1.0.3/LICENSE
--rw-r--r--   0        0        0     7749 2023-02-21 06:46:45.922881 supabase-1.0.3/README.md
--rw-r--r--   0        0        0     1788 2023-04-03 15:27:50.496977 supabase-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      392 2022-10-07 07:15:58.814523 supabase-1.0.3/supabase/__init__.py
--rw-r--r--   0        0        0       22 2023-04-03 15:27:58.128577 supabase-1.0.3/supabase/__version__.py
--rw-r--r--   0        0        0     8648 2023-04-03 15:26:27.587025 supabase-1.0.3/supabase/client.py
--rw-r--r--   0        0        0      100 2022-10-07 07:13:21.476307 supabase-1.0.3/supabase/lib/__init__.py
--rw-r--r--   0        0        0     1072 2023-02-21 06:46:45.925419 supabase-1.0.3/supabase/lib/auth_client.py
--rw-r--r--   0        0        0     3102 2023-04-03 15:26:27.587283 supabase-1.0.3/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2022-12-13 07:30:28.897213 supabase-1.0.3/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0      382 2022-10-07 07:13:21.476876 supabase-1.0.3/supabase/lib/storage_client.py
--rw-r--r--   0        0        0        0 2022-10-07 07:13:21.476931 supabase-1.0.3/supabase/py.typed
--rw-r--r--   0        0        0     8908 1970-01-01 00:00:00.000000 supabase-1.0.3/setup.py
--rw-r--r--   0        0        0     8875 1970-01-01 00:00:00.000000 supabase-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-04 08:35:29.207782 supabase-1.0.4/LICENSE
+-rw-r--r--   0        0        0    11009 2023-08-04 08:35:29.207942 supabase-1.0.4/README.md
+-rw-r--r--   0        0        0     1752 2023-08-04 09:09:36.429820 supabase-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-08-04 08:35:29.209093 supabase-1.0.4/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-04 09:09:47.954581 supabase-1.0.4/supabase/__version__.py
+-rw-r--r--   0        0        0     8334 2023-08-04 08:35:29.209235 supabase-1.0.4/supabase/client.py
+-rw-r--r--   0        0        0      100 2023-08-04 08:35:29.209331 supabase-1.0.4/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     1135 2023-08-04 08:35:29.209400 supabase-1.0.4/supabase/lib/auth_client.py
+-rw-r--r--   0        0        0     3102 2023-08-04 08:35:29.209467 supabase-1.0.4/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2023-08-04 08:35:29.209535 supabase-1.0.4/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0      382 2023-08-04 08:35:29.209593 supabase-1.0.4/supabase/lib/storage_client.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:35:29.209619 supabase-1.0.4/supabase/py.typed
+-rw-r--r--   0        0        0    12037 1970-01-01 00:00:00.000000 supabase-1.0.4/PKG-INFO
```

### Comparing `supabase-1.0.3/LICENSE` & `supabase-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-1.0.3/README.md` & `supabase-1.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -81,47 +81,64 @@
 ```
 
 ### See issues for what to work on
 
 Rough roadmap:
 
 - [x] Wrap [Postgrest-py](https://github.com/supabase-community/postgrest-py/)
+  - [ ] Add remaining filters
+  - [ ] Add support for EXPLAIN
+  - [ ] Add proper error handling
 - [ ] Wrap [Realtime-py](https://github.com/supabase-community/realtime-py)
+    - [ ]  Integrate with Supabase-py
+    - [ ]  Support WALRUS
+    - [ ]  Support broadcast (to check if already supported)
 - [x] Wrap [Gotrue-py](https://github.com/supabase-community/gotrue-py)
+    - [ ] Remove references to GoTrue-js v1 and do a proper release
+    - [ ] Test and document common flows (e.g. sign in with OAuth, sign in with OTP)
+    - [ ] Add MFA methods and SSO methods
 - [x] Wrap [storage-py](https://github.com/supabase-community/storage-py)
+    - [ ]  Support resumable uploads
+    - [ ]  Setup testing environment
+    - [ ]  Document how to properly upload different file types (e.g. jpeg/png and download it)
 - [x] Wrap [functions-py](https://github.com/supabase-community/functions-py)
 
+Overall Tasks:
+- [ ] Add async support across the entire library
+- [ ] Add FastAPI helper library (external to supabase-py)
+- [ ] Add `django-supabase-postgrest` (external to supabase-py)
+
 ### Client Library
 
 ## Authenticate
 
 ```python
 from supabase import create_client, Client
 
 url: str = os.environ.get("SUPABASE_TEST_URL")
 key: str = os.environ.get("SUPABASE_TEST_KEY")
 supabase: Client = create_client(url, key)
 # Create a random user login email and password.
 random_email: str = "3hf82fijf92@supamail.com"
 random_password: str = "fqj13bnf2hiu23h"
-user = supabase.auth.sign_up(email=random_email, password=random_password)
+user = supabase.auth.sign_up({ "email": random_email, "password": random_password })
 ```
 
 ## Sign-in
 
 ```python
 from supabase import create_client, Client
 
 url: str = os.environ.get("SUPABASE_TEST_URL")
 key: str = os.environ.get("SUPABASE_TEST_KEY")
 supabase: Client = create_client(url, key)
 # Sign in using the user email and password.
 random_email: str = "3hf82fijf92@supamail.com"
 random_password: str = "fqj13bnf2hiu23h"
-user = supabase.auth.sign_in(email=random_email, password=random_password)
+user = supabase.auth.sign_in_with_password({ "email": random_email, "password": random_password })
 ```
 
 ## Managing Data
 
 ### Insertion of Data
 
 ```python
@@ -154,14 +171,32 @@
 
 url: str = os.environ.get("SUPABASE_TEST_URL")
 key: str = os.environ.get("SUPABASE_TEST_KEY")
 supabase: Client = create_client(url, key)
 data = supabase.table("countries").update({"country": "Indonesia", "capital_city": "Jakarta"}).eq("id", 1).execute()
 ```
 
+### Update data of duplicate keys
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+country = {
+  "country": "United Kingdom",
+  "capital_city": "London" # this was missing when it was added
+}
+
+data = supabase.table("countries").upsert(country).execute()
+assert len(data.data) > 0
+```
+
 ### Deletion of Data
 
 ```python
 from supabase import create_client, Client
 
 url: str = os.environ.get("SUPABASE_TEST_URL")
 key: str = os.environ.get("SUPABASE_TEST_KEY")
@@ -185,17 +220,96 @@
     return resp
 
 loop = asyncio.get_event_loop()
 resp = loop.run_until_complete(test_func(loop))
 loop.close()
 ```
 
+## Storage
+
+### Download a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+
+data = supabase.storage.from_(bucket_name).download("photo1.png)
+```
+
+### Upload a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+new_file = getUserFile()
+
+data = supabase.storage.from_(bucket_name).upload("/user1/profile.png", new_file)
+```
+
+### Delete a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+
+data = supabase.storage.from_(bucket_name).delete(["old_photo.png", "image5.jpg"])
+```
+
+### List all files
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "charts"
+
+data = supabase.storage.from_(bucket_name).list()
+```
+
+### Move and rename file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "charts"
+old_file_path: str = "generic/graph1.png"
+new_file_path: str = "important/revenue.png"
+
+data = supabase.storage.from_(bucket_name).move(old_file_path, new_file_path)
+```
+
+
 ## Realtime Changes
 
 Realtime changes are unfortunately still a WIP. Feel free to file PRs to [realtime-py](https://github.com/supabase-community/realtime-py)
 
 See [Supabase Docs](https://supabase.com/docs/guides/client-libraries) for full list of examples
 
+## NOTE: RLS does not work out of the box right now
+After you sign a user in, the user's access token is _not_ being used by the library for any of the API calls, and therefore RLS does not work right now. See [related issue and discussion](https://github.com/supabase-community/supabase-py/issues/185)
+
 ## Python and Supabase Resources
 
 - [Python data loading with Supabase](https://supabase.com/blog/loading-data-supabase-python)
 - [Visualizing Supabase Data using Metabase](https://supabase.com/blog/visualizing-supabase-data-using-metabase)
```

### Comparing `supabase-1.0.3/pyproject.toml` & `supabase-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "1.0.3"
+version = "1.0.4"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
@@ -12,31 +12,30 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-postgrest = "^0.10.6"
+postgrest = "^0.10.8"
 realtime = "^1.0.0"
-gotrue = "^1.0.1"
-httpx = "^0.23.0"
-storage3 = "^0.5.2"
-supafunc = "^0.2.2"
-python-semantic-release = "7.33.2"
+gotrue = "^1.0.3"
+httpx = "^0.24.0"
+storage3 = "^0.5.3"
+supafunc = "^0.2.3"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^3.2.1"
-black = "^23.1"
-pytest = "^7.2.2"
+pre-commit = "^3.3.3"
+black = "^23.7"
+pytest = "^7.4.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
-pytest-cov = "^4.0.0"
-commitizen = "^2.42.0"
-python-semantic-release = "^7.33.2"
+pytest-cov = "^4.1.0"
+commitizen = "^3.5.2"
+python-semantic-release = "^7.34.6"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.scripts]
 tests = 'poetry_scripts:run_tests'
 
 [tool.semantic_release]
 version_variable = "supabase/__version__.py:__version__"
```

### Comparing `supabase-1.0.3/supabase/client.py` & `supabase-1.0.4/supabase/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,20 @@
             r"^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$", supabase_key
         ):
             raise SupabaseException("Invalid API key")
 
         self.supabase_url = supabase_url
         self.supabase_key = supabase_key
         options.headers.update(self._get_auth_headers())
-        self.rest_url: str = f"{supabase_url}/rest/v1"
-        self.realtime_url: str = f"{supabase_url}/realtime/v1".replace("http", "ws")
-        self.auth_url: str = f"{supabase_url}/auth/v1"
+        self.rest_url = f"{supabase_url}/rest/v1"
+        self.realtime_url = f"{supabase_url}/realtime/v1".replace("http", "ws")
+        self.auth_url = f"{supabase_url}/auth/v1"
         self.storage_url = f"{supabase_url}/storage/v1"
-        is_platform = re.search(r"(supabase\.co)|(supabase\.in)", supabase_url)
-        if is_platform:
-            url_parts = supabase_url.split(".")
-            self.functions_url = (
-                f"{url_parts[0]}.functions.{url_parts[1]}.{url_parts[2]}"
-            )
-
-        else:
-            self.functions_url = f"{supabase_url}/functions/v1"
-        self.schema: str = options.schema
+        self.functions_url = f"{supabase_url}/functions/v1"
+        self.schema = options.schema
 
         # Instantiate clients.
         self.auth = self._init_supabase_auth_client(
             auth_url=self.auth_url,
             client_options=options,
         )
         # TODO: Bring up to parity with JS client.
```

### Comparing `supabase-1.0.3/supabase/lib/auth_client.py` & `supabase-1.0.4/supabase/lib/auth_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union
+from typing import Dict, Optional
 
 from gotrue import SyncGoTrueClient, SyncMemoryStorage, SyncSupportedStorage
 
 # TODO - export this from GoTrue-py in next release
 from httpx import Client as BaseClient
 
 
@@ -14,22 +14,25 @@
 class SupabaseAuthClient(SyncGoTrueClient):
     """SupabaseAuthClient"""
 
     def __init__(
         self,
         *,
         url: str,
-        headers: Dict[str, str] = {},
-        storage_key: Union[str, None] = None,
+        headers: Optional[Dict[str, str]] = None,
+        storage_key: Optional[str] = None,
         auto_refresh_token: bool = True,
         persist_session: bool = True,
         storage: SyncSupportedStorage = SyncMemoryStorage(),
-        http_client: Union[SyncClient, None] = None,
+        http_client: Optional[SyncClient] = None,
     ):
         """Instantiate SupabaseAuthClient instance."""
+        if headers is None:
+            headers = {}
+
         SyncGoTrueClient.__init__(
             self,
             url=url,
             headers=headers,
             storage_key=storage_key,
             auto_refresh_token=auto_refresh_token,
             persist_session=persist_session,
```

### Comparing `supabase-1.0.3/supabase/lib/client_options.py` & `supabase-1.0.4/supabase/lib/client_options.py`

 * *Files identical despite different names*

### Comparing `supabase-1.0.3/supabase/lib/realtime_client.py` & `supabase-1.0.4/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-1.0.3/setup.py` & `supabase-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,342 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: supabase
+Version: 1.0.4
+Summary: Supabase client for Python.
+Home-page: https://github.com/supabase-community/supabase-py
+License: MIT
+Author: Joel Lee
+Author-email: joel@joellee.org
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gotrue (>=1.0.3,<2.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: postgrest (>=0.10.8,<0.11.0)
+Requires-Dist: realtime (>=1.0.0,<2.0.0)
+Requires-Dist: storage3 (>=0.5.3,<0.6.0)
+Requires-Dist: supafunc (>=0.2.3,<0.3.0)
+Project-URL: Documentation, https://github.com/supabase-community/supabase-py
+Project-URL: Repository, https://github.com/supabase-community/supabase-py
+Description-Content-Type: text/markdown
 
-packages = \
-['supabase', 'supabase.lib']
+# supabase-py
 
-package_data = \
-{'': ['*']}
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
+[![CI](https://github.com/supabase-community/supabase-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/supabase-py/actions/workflows/ci.yml)
+[![Python](https://img.shields.io/pypi/pyversions/supabase)](https://pypi.org/project/supabase)
+[![Version](https://img.shields.io/pypi/v/supabase?color=%2334D058)](https://pypi.org/project/supabase)
+[![Codecov](https://codecov.io/gh/supabase-community/supabase-py/branch/develop/graph/badge.svg)](https://codecov.io/gh/supabase-community/supabase-py)
+[![Last commit](https://img.shields.io/github/last-commit/supabase-community/supabase-py.svg?style=flat)](https://github.com/supabase-community/supabase-py/commits)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/supabase-py)](https://github.com/supabase-community/supabase-py/commits)
+[![Github Stars](https://img.shields.io/github/stars/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py/stargazers)
+[![Github Forks](https://img.shields.io/github/forks/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py/network/members)
+[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py)
+[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/supabase-py)](https://github.com/supabase-community/supabase-py/graphs/contributors)
 
-install_requires = \
-['gotrue>=1.0.1,<2.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'postgrest>=0.10.6,<0.11.0',
- 'python-semantic-release==7.33.2',
- 'realtime>=1.0.0,<2.0.0',
- 'storage3>=0.5.2,<0.6.0',
- 'supafunc>=0.2.2,<0.3.0']
-
-entry_points = \
-{'console_scripts': ['tests = poetry_scripts:run_tests']}
-
-setup_kwargs = {
-    'name': 'supabase',
-    'version': '1.0.3',
-    'description': 'Supabase client for Python.',
-    'long_description': '# supabase-py\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/supabase-community/supabase-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/supabase-py/actions/workflows/ci.yml)\n[![Python](https://img.shields.io/pypi/pyversions/supabase)](https://pypi.org/project/supabase)\n[![Version](https://img.shields.io/pypi/v/supabase?color=%2334D058)](https://pypi.org/project/supabase)\n[![Codecov](https://codecov.io/gh/supabase-community/supabase-py/branch/develop/graph/badge.svg)](https://codecov.io/gh/supabase-community/supabase-py)\n[![Last commit](https://img.shields.io/github/last-commit/supabase-community/supabase-py.svg?style=flat)](https://github.com/supabase-community/supabase-py/commits)\n[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/supabase-py)](https://github.com/supabase-community/supabase-py/commits)\n[![Github Stars](https://img.shields.io/github/stars/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py/stargazers)\n[![Github Forks](https://img.shields.io/github/forks/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py/network/members)\n[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/supabase-py?style=flat&logo=github)](https://github.com/supabase-community/supabase-py)\n[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/supabase-py)](https://github.com/supabase-community/supabase-py/graphs/contributors)\n\nSupabase client for Python. This mirrors the design of [supabase-js](https://github.com/supabase/supabase-js/blob/master/README.md)\n\n| Status | Stability | Goal |\n| ------ | ------ | ---- |\n| ✅ | Alpha | We are testing Supabase with a closed set of customers |\n| ✅ | Public Alpha | Anyone can sign up over at [app.supabase.io](https://app.supabase.com). But go easy on us, there are a few kinks. |\n| 🚧 | Public Beta | Stable enough for most non-enterprise use-cases |\n| ❌ | Public | Production-ready |\n\nWe are currently in Public Alpha. Watch "releases" of this repo to get notified of major updates.\n\n\n## Installation\n\n**Recomended:** First activate your virtual environment, with your favourite system. For example, we like `poetry` and `conda`!\n\n### PyPi installation\n\nNow install the package. (for > Python 3.7)\n\n```bash\n# with pip\npip install supabase\n\n# with conda\nconda install -c conda-forge supabase\n```\n\n### Local installation\n\nYou can also install locally after cloning this repo. Install Development mode with ``pip install -e``, which makes it so when you edit the source code the changes will be reflected in your python module.\n\n## Usage\n\nIt\'s usually best practice to set your api key environment variables in some way that version control doesn\'t track them, e.g don\'t put them in your python modules! Set the key and url for the supabase instance in the shell, or better yet, use a dotenv file. Heres how to set the variables in the shell.\n\n```bash\nexport SUPABASE_URL="my-url-to-my-awesome-supabase-instance"\nexport SUPABASE_KEY="my-supa-dupa-secret-supabase-api-key"\n```\n\nWe can then read the keys in the python source code.\n\n```python\nimport os\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_URL")\nkey: str = os.environ.get("SUPABASE_KEY")\nsupabase: Client = create_client(url, key)\n```\n\nUse the supabase client to interface with your database.\n\n### Running Tests\n\nCurrently the test suites are in a state of flux. We are expanding our clients tests to ensure things are working, and for now can connect to this test instance, that is populated with the following table:\n\n<p align="center">\n  <img width="720" height="481" src="https://i.ibb.co/Bq7Kdty/db.png">\n</p>\n\nThe above test database is a blank supabase instance that has populated the `countries` table with the built in countries script that can be found in the supabase UI. You can launch the test scripts and point to the above test database by running\n\n```bash\n./test.sh\n```\n\n### See issues for what to work on\n\nRough roadmap:\n\n- [x] Wrap [Postgrest-py](https://github.com/supabase-community/postgrest-py/)\n- [ ] Wrap [Realtime-py](https://github.com/supabase-community/realtime-py)\n- [x] Wrap [Gotrue-py](https://github.com/supabase-community/gotrue-py)\n- [x] Wrap [storage-py](https://github.com/supabase-community/storage-py)\n- [x] Wrap [functions-py](https://github.com/supabase-community/functions-py)\n\n### Client Library\n\n## Authenticate\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\n# Create a random user login email and password.\nrandom_email: str = "3hf82fijf92@supamail.com"\nrandom_password: str = "fqj13bnf2hiu23h"\nuser = supabase.auth.sign_up(email=random_email, password=random_password)\n```\n\n## Sign-in\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\n# Sign in using the user email and password.\nrandom_email: str = "3hf82fijf92@supamail.com"\nrandom_password: str = "fqj13bnf2hiu23h"\nuser = supabase.auth.sign_in(email=random_email, password=random_password)\n```\n\n## Managing Data\n\n### Insertion of Data\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\ndata = supabase.table("countries").insert({"name":"Germany"}).execute()\nassert len(data.data) > 0\n```\n\n### Selection of Data\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\ndata = supabase.table("countries").select("*").eq("country", "IL").execute()\n# Assert we pulled real data.\nassert len(data.data) > 0\n```\n\n### Update of Data\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\ndata = supabase.table("countries").update({"country": "Indonesia", "capital_city": "Jakarta"}).eq("id", 1).execute()\n```\n\n### Deletion of Data\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\ndata = supabase.table("countries").delete().eq("id", 1).execute()\n```\n\n### Supabase Functions\n\n```python\nfrom supabase import create_client, Client\n\nurl: str = os.environ.get("SUPABASE_TEST_URL")\nkey: str = os.environ.get("SUPABASE_TEST_KEY")\nsupabase: Client = create_client(url, key)\nfunc = supabase.functions()\n\n@asyncio.coroutine\nasync def test_func(loop):\n    resp = await func.invoke("hello-world",invoke_options={\'body\':{}})\n    return resp\n\nloop = asyncio.get_event_loop()\nresp = loop.run_until_complete(test_func(loop))\nloop.close()\n```\n\n## Realtime Changes\n\nRealtime changes are unfortunately still a WIP. Feel free to file PRs to [realtime-py](https://github.com/supabase-community/realtime-py)\n\nSee [Supabase Docs](https://supabase.com/docs/guides/client-libraries) for full list of examples\n\n## Python and Supabase Resources\n\n- [Python data loading with Supabase](https://supabase.com/blog/loading-data-supabase-python)\n- [Visualizing Supabase Data using Metabase](https://supabase.com/blog/visualizing-supabase-data-using-metabase)\n',
-    'author': 'Joel Lee',
-    'author_email': 'joel@joellee.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/supabase-community/supabase-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+Supabase client for Python. This mirrors the design of [supabase-js](https://github.com/supabase/supabase-js/blob/master/README.md)
+
+| Status | Stability | Goal |
+| ------ | ------ | ---- |
+| ✅ | Alpha | We are testing Supabase with a closed set of customers |
+| ✅ | Public Alpha | Anyone can sign up over at [app.supabase.io](https://app.supabase.com). But go easy on us, there are a few kinks. |
+| 🚧 | Public Beta | Stable enough for most non-enterprise use-cases |
+| ❌ | Public | Production-ready |
+
+We are currently in Public Alpha. Watch "releases" of this repo to get notified of major updates.
+
+
+## Installation
+
+**Recomended:** First activate your virtual environment, with your favourite system. For example, we like `poetry` and `conda`!
+
+### PyPi installation
+
+Now install the package. (for > Python 3.7)
+
+```bash
+# with pip
+pip install supabase
+
+# with conda
+conda install -c conda-forge supabase
+```
+
+### Local installation
+
+You can also install locally after cloning this repo. Install Development mode with ``pip install -e``, which makes it so when you edit the source code the changes will be reflected in your python module.
+
+## Usage
+
+It's usually best practice to set your api key environment variables in some way that version control doesn't track them, e.g don't put them in your python modules! Set the key and url for the supabase instance in the shell, or better yet, use a dotenv file. Heres how to set the variables in the shell.
+
+```bash
+export SUPABASE_URL="my-url-to-my-awesome-supabase-instance"
+export SUPABASE_KEY="my-supa-dupa-secret-supabase-api-key"
+```
+
+We can then read the keys in the python source code.
+
+```python
+import os
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_URL")
+key: str = os.environ.get("SUPABASE_KEY")
+supabase: Client = create_client(url, key)
+```
+
+Use the supabase client to interface with your database.
+
+### Running Tests
+
+Currently the test suites are in a state of flux. We are expanding our clients tests to ensure things are working, and for now can connect to this test instance, that is populated with the following table:
+
+<p align="center">
+  <img width="720" height="481" src="https://i.ibb.co/Bq7Kdty/db.png">
+</p>
+
+The above test database is a blank supabase instance that has populated the `countries` table with the built in countries script that can be found in the supabase UI. You can launch the test scripts and point to the above test database by running
+
+```bash
+./test.sh
+```
+
+### See issues for what to work on
+
+Rough roadmap:
+
+- [x] Wrap [Postgrest-py](https://github.com/supabase-community/postgrest-py/)
+  - [ ] Add remaining filters
+  - [ ] Add support for EXPLAIN
+  - [ ] Add proper error handling
+- [ ] Wrap [Realtime-py](https://github.com/supabase-community/realtime-py)
+    - [ ]  Integrate with Supabase-py
+    - [ ]  Support WALRUS
+    - [ ]  Support broadcast (to check if already supported)
+- [x] Wrap [Gotrue-py](https://github.com/supabase-community/gotrue-py)
+    - [ ] Remove references to GoTrue-js v1 and do a proper release
+    - [ ] Test and document common flows (e.g. sign in with OAuth, sign in with OTP)
+    - [ ] Add MFA methods and SSO methods
+- [x] Wrap [storage-py](https://github.com/supabase-community/storage-py)
+    - [ ]  Support resumable uploads
+    - [ ]  Setup testing environment
+    - [ ]  Document how to properly upload different file types (e.g. jpeg/png and download it)
+- [x] Wrap [functions-py](https://github.com/supabase-community/functions-py)
+
+Overall Tasks:
+- [ ] Add async support across the entire library
+- [ ] Add FastAPI helper library (external to supabase-py)
+- [ ] Add `django-supabase-postgrest` (external to supabase-py)
+
+### Client Library
+
+## Authenticate
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+# Create a random user login email and password.
+random_email: str = "3hf82fijf92@supamail.com"
+random_password: str = "fqj13bnf2hiu23h"
+user = supabase.auth.sign_up({ "email": random_email, "password": random_password })
+```
+
+## Sign-in
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+# Sign in using the user email and password.
+random_email: str = "3hf82fijf92@supamail.com"
+random_password: str = "fqj13bnf2hiu23h"
+user = supabase.auth.sign_in_with_password({ "email": random_email, "password": random_password })
+```
+
+## Managing Data
+
+### Insertion of Data
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+data = supabase.table("countries").insert({"name":"Germany"}).execute()
+assert len(data.data) > 0
+```
+
+### Selection of Data
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+data = supabase.table("countries").select("*").eq("country", "IL").execute()
+# Assert we pulled real data.
+assert len(data.data) > 0
+```
+
+### Update of Data
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+data = supabase.table("countries").update({"country": "Indonesia", "capital_city": "Jakarta"}).eq("id", 1).execute()
+```
+
+### Update data of duplicate keys
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+country = {
+  "country": "United Kingdom",
+  "capital_city": "London" # this was missing when it was added
 }
 
+data = supabase.table("countries").upsert(country).execute()
+assert len(data.data) > 0
+```
+
+### Deletion of Data
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+data = supabase.table("countries").delete().eq("id", 1).execute()
+```
+
+### Supabase Functions
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+func = supabase.functions()
+
+@asyncio.coroutine
+async def test_func(loop):
+    resp = await func.invoke("hello-world",invoke_options={'body':{}})
+    return resp
+
+loop = asyncio.get_event_loop()
+resp = loop.run_until_complete(test_func(loop))
+loop.close()
+```
+
+## Storage
+
+### Download a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+
+data = supabase.storage.from_(bucket_name).download("photo1.png)
+```
+
+### Upload a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+new_file = getUserFile()
+
+data = supabase.storage.from_(bucket_name).upload("/user1/profile.png", new_file)
+```
+
+### Delete a file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "photos"
+
+data = supabase.storage.from_(bucket_name).delete(["old_photo.png", "image5.jpg"])
+```
+
+### List all files
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "charts"
+
+data = supabase.storage.from_(bucket_name).list()
+```
+
+### Move and rename file
+
+```python
+from supabase import create_client, Client
+
+url: str = os.environ.get("SUPABASE_TEST_URL")
+key: str = os.environ.get("SUPABASE_TEST_KEY")
+supabase: Client = create_client(url, key)
+
+bucket_name: str = "charts"
+old_file_path: str = "generic/graph1.png"
+new_file_path: str = "important/revenue.png"
+
+data = supabase.storage.from_(bucket_name).move(old_file_path, new_file_path)
+```
+
+
+## Realtime Changes
+
+Realtime changes are unfortunately still a WIP. Feel free to file PRs to [realtime-py](https://github.com/supabase-community/realtime-py)
+
+See [Supabase Docs](https://supabase.com/docs/guides/client-libraries) for full list of examples
+
+## NOTE: RLS does not work out of the box right now
+After you sign a user in, the user's access token is _not_ being used by the library for any of the API calls, and therefore RLS does not work right now. See [related issue and discussion](https://github.com/supabase-community/supabase-py/issues/185)
+
+## Python and Supabase Resources
+
+- [Python data loading with Supabase](https://supabase.com/blog/loading-data-supabase-python)
+- [Visualizing Supabase Data using Metabase](https://supabase.com/blog/visualizing-supabase-data-using-metabase)
 
-setup(**setup_kwargs)
```

