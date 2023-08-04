# Comparing `tmp/dagger_io-0.8.0.tar.gz` & `tmp/dagger_io-0.8.1.tar.gz`

## Comparing `dagger_io-0.8.0.tar` & `dagger_io-0.8.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dagger_io-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/client.rst
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/conf.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/connection.rst
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/exceptions.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/index.rst
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 dagger_io-0.8.0/docs/_ext/dagger_ext.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_config.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_connection.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_exceptions.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_managers.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/__init__.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/cli.py
--rw-r--r--   0        0        0    28844 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_codegen/generator.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/_version.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/conn.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/download.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/progress.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/_engine/session.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/__init__.py
--rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_core.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_guards.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_session.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/conn.py
--rw-r--r--   0        0        0    92472 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/gen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_transport/__init__.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/client/_transport/httpx.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/__main__.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_commands.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_context.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_converter.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_exceptions.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_server.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/_util.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dagger_io-0.8.0/src/dagger/server/cli.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_codegen.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_connection_errors.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_execute_errors.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_inputs.py
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_integration.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/client/test_response.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/engine/test_cli.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 dagger_io-0.8.0/tests/engine/test_download.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.8.0/.gitignore
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.8.0/LICENSE
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 dagger_io-0.8.0/README.md
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 dagger_io-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 dagger_io-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 dagger_io-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/client.rst
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/connection.rst
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/exceptions.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/index.rst
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 dagger_io-0.8.1/docs/_ext/dagger_ext.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_config.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_connection.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_exceptions.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_managers.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_codegen/__init__.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_codegen/cli.py
+-rw-r--r--   0        0        0    28844 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_codegen/generator.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/_version.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/conn.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/download.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/progress.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/_engine/session.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/__init__.py
+-rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/_core.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/_guards.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/_session.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/conn.py
+-rw-r--r--   0        0        0    92472 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/gen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/_transport/__init__.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/client/_transport/httpx.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_commands.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_context.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_converter.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_exceptions.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_server.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/_util.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dagger_io-0.8.1/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_codegen.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_connection_errors.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_execute_errors.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_inputs.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_integration.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/client/test_response.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/engine/test_cli.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 dagger_io-0.8.1/tests/engine/test_download.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.8.1/.gitignore
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 dagger_io-0.8.1/README.md
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 dagger_io-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 dagger_io-0.8.1/PKG-INFO
```

### Comparing `dagger_io-0.8.0/CHANGELOG.md` & `dagger_io-0.8.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html),
 and is generated by [Changie](https://github.com/miniscruff/changie).
 
 
 
+## sdk/python/v0.8.1 - 2023-08-04
+
+This SDK uses 🚙 Engine + 🚗 CLI version `v0.8.1`. [See what changed in that release](https://github.com/dagger/dagger/releases/tag/v0.8.1).
+
+🐍 https://pypi.org/project/dagger-io/v0.8.1/
+📖 https://dagger-io.readthedocs.io/en/sdk-python-v0.8.1/
+
+
+### Dependencies
+- Bump Engine to v0.8.1 by @github-actions in https://github.com/dagger/dagger/pull/5581
+
+### What to do next
+- Read the [documentation](https://docs.dagger.io/sdk/python)
+- Join our [Discord server](https://discord.gg/dagger-io)
+- Follow us on [Twitter](https://twitter.com/dagger_io)
+
+
+
 ## sdk/python/v0.8.0 - 2023-08-03
 
 This SDK uses 🚙 Engine + 🚗 CLI version `v0.8.0`. [See what changed in that release](https://github.com/dagger/dagger/releases/tag/v0.8.0).
 
 🐍 https://pypi.org/project/dagger-io/v0.8.0/
 📖 https://dagger-io.readthedocs.io/en/sdk-python-v0.8.0/
```

### Comparing `dagger_io-0.8.0/docs/conf.py` & `dagger_io-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/docs/exceptions.rst` & `dagger_io-0.8.1/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/docs/index.rst` & `dagger_io-0.8.1/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
    exceptions
 
 
 Project links
 =============
 
 * `PyPI Project <https://pypi.org/project/dagger-io/>`_
+* `Conda Package <https://anaconda.org/conda-forge/dagger-io>`_
 * `Documentation <https://docs.dagger.io/sdk/python>`_
 * `Source code <https://github.com/dagger/dagger/tree/main/sdk/python>`_
 * `Release Notes <https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0>`_
 
 
 Indices and tables
 ==================
```

### Comparing `dagger_io-0.8.0/docs/_ext/dagger_ext.py` & `dagger_io-0.8.1/docs/_ext/dagger_ext.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/__init__.py` & `dagger_io-0.8.1/src/dagger/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_config.py` & `dagger_io-0.8.1/src/dagger/_config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_connection.py` & `dagger_io-0.8.1/src/dagger/_connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_exceptions.py` & `dagger_io-0.8.1/src/dagger/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_managers.py` & `dagger_io-0.8.1/src/dagger/_managers.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/log.py` & `dagger_io-0.8.1/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_codegen/cli.py` & `dagger_io-0.8.1/src/dagger/_codegen/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_codegen/generator.py` & `dagger_io-0.8.1/src/dagger/_codegen/generator.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_engine/conn.py` & `dagger_io-0.8.1/src/dagger/_engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_engine/download.py` & `dagger_io-0.8.1/src/dagger/_engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_engine/progress.py` & `dagger_io-0.8.1/src/dagger/_engine/progress.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/_engine/session.py` & `dagger_io-0.8.1/src/dagger/_engine/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/_core.py` & `dagger_io-0.8.1/src/dagger/client/_core.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/_guards.py` & `dagger_io-0.8.1/src/dagger/client/_guards.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/_session.py` & `dagger_io-0.8.1/src/dagger/client/_session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/base.py` & `dagger_io-0.8.1/src/dagger/client/base.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/conn.py` & `dagger_io-0.8.1/src/dagger/client/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/gen.py` & `dagger_io-0.8.1/src/dagger/client/gen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/client/_transport/httpx.py` & `dagger_io-0.8.1/src/dagger/client/_transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/server/_commands.py` & `dagger_io-0.8.1/src/dagger/server/_commands.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/server/_context.py` & `dagger_io-0.8.1/src/dagger/server/_context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/server/_converter.py` & `dagger_io-0.8.1/src/dagger/server/_converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/server/_server.py` & `dagger_io-0.8.1/src/dagger/server/_server.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/src/dagger/server/cli.py` & `dagger_io-0.8.1/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_codegen.py` & `dagger_io-0.8.1/tests/client/test_codegen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_connection_errors.py` & `dagger_io-0.8.1/tests/client/test_connection_errors.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_execute_errors.py` & `dagger_io-0.8.1/tests/client/test_execute_errors.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_inputs.py` & `dagger_io-0.8.1/tests/client/test_inputs.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_integration.py` & `dagger_io-0.8.1/tests/client/test_integration.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/client/test_response.py` & `dagger_io-0.8.1/tests/client/test_response.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/engine/test_cli.py` & `dagger_io-0.8.1/tests/engine/test_cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/tests/engine/test_download.py` & `dagger_io-0.8.1/tests/engine/test_download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/LICENSE` & `dagger_io-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/README.md` & `dagger_io-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/pyproject.toml` & `dagger_io-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagger_io-0.8.0/PKG-INFO` & `dagger_io-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.8.0
+Version: 0.8.1
 Summary: A client package for running Dagger pipelines in Python.
 Project-URL: Homepage, https://dagger.io
 Project-URL: Documentation, https://docs.dagger.io/sdk/python
 Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
 Project-URL: Tracker, https://github.com/dagger/dagger/issues
 Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
 Project-URL: Community, https://discord.gg/ufnyBtc8uY
```

