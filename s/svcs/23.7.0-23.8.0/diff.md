# Comparing `tmp/svcs-23.7.0.tar.gz` & `tmp/svcs-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Aug  2 14:41:14 2023, max compression
+gzip compressed data, last modified: Fri Aug  4 20:16:10 2023, max compression
```

## Comparing `svcs-23.7.0.tar` & `svcs-23.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      125 2023-08-02 14:41:14.000000 svcs-23.7.0/.git_archival.txt
--rw-r--r--   0        0        0      131 2023-08-02 14:41:14.000000 svcs-23.7.0/.gitattributes
--rw-r--r--   0        0        0      732 2023-08-02 14:41:14.000000 svcs-23.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-08-02 14:41:14.000000 svcs-23.7.0/.python-version-default
--rw-r--r--   0        0        0     3288 2023-08-02 14:41:14.000000 svcs-23.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    18022 2023-08-02 14:41:14.000000 svcs-23.7.0/README.md
--rw-r--r--   0        0        0     1052 2023-08-02 14:41:14.000000 svcs-23.7.0/conftest.py
--rw-r--r--   0        0        0      840 2023-08-02 14:41:14.000000 svcs-23.7.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      285 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4136 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1642 2023-08-02 14:41:14.000000 svcs-23.7.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     1093 2023-08-02 14:41:14.000000 svcs-23.7.0/docs/_static/logo.svg
--rw-r--r--   0        0        0     2735 2023-08-02 14:41:14.000000 svcs-23.7.0/docs/_static/logo_with_name.svg
--rw-r--r--   0        0        0      650 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/__init__.py
--rw-r--r--   0        0        0    11383 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/_core.py
--rw-r--r--   0        0        0      234 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/exceptions.py
--rw-r--r--   0        0        0     3508 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/flask.py
--rw-r--r--   0        0        0        0 2023-08-02 14:41:14.000000 svcs-23.7.0/src/svcs/py.typed
--rw-r--r--   0        0        0       91 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/__init__.py
--rw-r--r--   0        0        0      405 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/fake_factories.py
--rw-r--r--   0        0        0      481 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/ifaces.py
--rw-r--r--   0        0        0     2394 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_container.py
--rw-r--r--   0        0        0     1663 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_fake_factories.py
--rw-r--r--   0        0        0     6457 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_flask.py
--rw-r--r--   0        0        0     8045 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_integration.py
--rw-r--r--   0        0        0     8089 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/test_registry.py
--rw-r--r--   0        0        0     1457 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/typing/core.py
--rw-r--r--   0        0        0     1018 2023-08-02 14:41:14.000000 svcs-23.7.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      112 2023-08-02 14:41:14.000000 svcs-23.7.0/.gitignore
--rw-r--r--   0        0        0     1098 2023-08-02 14:41:14.000000 svcs-23.7.0/LICENSE
--rw-r--r--   0        0        0     4845 2023-08-02 14:41:14.000000 svcs-23.7.0/pyproject.toml
--rw-r--r--   0        0        0     7535 2023-08-02 14:41:14.000000 svcs-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-04 20:16:10.000000 svcs-23.8.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-08-04 20:16:10.000000 svcs-23.8.0/.gitattributes
+-rw-r--r--   0        0        0      732 2023-08-04 20:16:10.000000 svcs-23.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-08-04 20:16:10.000000 svcs-23.8.0/.python-version-default
+-rw-r--r--   0        0        0     3558 2023-08-04 20:16:10.000000 svcs-23.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0    18592 2023-08-04 20:16:10.000000 svcs-23.8.0/README.md
+-rw-r--r--   0        0        0     1052 2023-08-04 20:16:10.000000 svcs-23.8.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-08-04 20:16:10.000000 svcs-23.8.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      285 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4110 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1730 2023-08-04 20:16:10.000000 svcs-23.8.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     4549 2023-08-04 20:16:10.000000 svcs-23.8.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0     3834 2023-08-04 20:16:10.000000 svcs-23.8.0/docs/_static/logo_with_name.svg
+-rw-r--r--   0        0        0      650 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/__init__.py
+-rw-r--r--   0        0        0    12105 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/_core.py
+-rw-r--r--   0        0        0      234 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/exceptions.py
+-rw-r--r--   0        0        0     3512 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/flask.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:16:10.000000 svcs-23.8.0/src/svcs/py.typed
+-rw-r--r--   0        0        0       91 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      405 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/fake_factories.py
+-rw-r--r--   0        0        0      481 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/ifaces.py
+-rw-r--r--   0        0        0     2394 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_container.py
+-rw-r--r--   0        0        0     1663 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_fake_factories.py
+-rw-r--r--   0        0        0     6883 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_flask.py
+-rw-r--r--   0        0        0     8309 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_integration.py
+-rw-r--r--   0        0        0     8089 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/test_registry.py
+-rw-r--r--   0        0        0     1486 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/typing/core.py
+-rw-r--r--   0        0        0     1056 2023-08-04 20:16:10.000000 svcs-23.8.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      112 2023-08-04 20:16:10.000000 svcs-23.8.0/.gitignore
+-rw-r--r--   0        0        0     1098 2023-08-04 20:16:10.000000 svcs-23.8.0/LICENSE
+-rw-r--r--   0        0        0     4845 2023-08-04 20:16:10.000000 svcs-23.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7974 2023-08-04 20:16:10.000000 svcs-23.8.0/PKG-INFO
```

### Comparing `svcs-23.7.0/.pre-commit-config.yaml` & `svcs-23.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/CHANGELOG.md` & `svcs-23.8.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svcs/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [23.8.0](https://github.com/hynek/svcs/compare/23.7.0...23.8.0) - 2023-08-04
+
+### Added
+
+- It's now possible to request multiple services at once by passing multiple types to `Container.get()` and `Container.aget()`.
+  [#15](https://github.com/hynek/svcs/pull/15)
+
+
+
 ## [23.7.0](https://github.com/hynek/svcs/compare/23.6.0...23.7.0) - 2023-08-02
 
 ### Added
 
 - Factories now may take a parameter called `svcs_container` or that is annotated to be `svcs.Container`.
   In this case the factory will receive the current container as a first positional argument.
   This allows for recursive factories without global state.
```

### Comparing `svcs-23.7.0/README.md` & `svcs-23.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!-- begin-logo -->
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="docs/_static/logo_with_name.svg" width="25%" alt="svcs logo showing a radar" />
+    <img src="docs/_static/logo_with_name.svg" width="35%" alt="svcs logo showing a radar" />
   </a>
 </p>
 
 <p align="center">
-  A Lightweight Service Locator for Python.
+  <em>A Lightweight Service Locator for Python.</em>
 </p>
 
 <!-- end-logo -->
 
 <p align="center">
   <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/svcs">
   <a href="./LICENSE">
@@ -24,62 +24,70 @@
   </a>
 </p>
 
 ---
 
 <!-- begin-pypi -->
 
-> [!WARNING] ☠️ Not ready yet! ☠️
+> [!WARNING]
+> ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
 ---
 
-**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way without worrying about *cleaning them up*.**
+**This allows you to configure and manage all your resources in *one central place*, access them in a *consistent* way without worrying about *cleaning them up* and achieve *loose coupling*.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
-If you follow the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
+If you follow the [**_Dependency Inversion Principle_**](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
+
+If you follow the [**_Hexagonal Architecture_**](https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)) (aka "*ports and adapters*"), the registered types are *ports* and the factories produce the *adapters*.
+*svcs* gives you a well-defined way to make your application *pluggable*.
 
 Benefits:
 
 - Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
-- simplifies **testing**,
+- simplifies **testing** through **loose coupling**,
 - and allows for easy **health checks** across *all* resources.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
     api = request.services.get(WebAPIClient)
 ```
 
-or, if you don't shy away from some global state, even:
+You can also ask for multiple services at once:
 
 ```python
-def view():
-    db = services.get(Database)
-    api = services.get(WebAPIClient)
+def view(request):
+    db, api = request.services.get(Database, WebAPIClient)
 ```
 
-The latter already works with [Flask](#flask) by utilizing the [`g` object](https://flask.palletsprojects.com/en/latest/api/#flask.g).
+Or, if you don't shy away from some global state and your web framework supports it, even:
+
+```python
+def view():
+    db, api = svcs.flask.get(Database, WebAPIClient)
+```
 
 You set it up like this:
 
 <!--
 ; skip: next
 -->
 
@@ -512,7 +520,9 @@
 
 
 ## Credits
 
 *svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](./LICENSE) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
+
+The [Bestagon](https://www.youtube.com/watch?v=thOifuHs6eY) locator logo is made by [Lynn Root](https://www.roguelynn.com), based on an [Font Awesome](https://fontawesome.com) Icon.
```

### Comparing `svcs-23.7.0/conftest.py` & `svcs-23.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/tox.ini` & `svcs-23.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/.github/CODE_OF_CONDUCT.md` & `svcs-23.8.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/.github/SECURITY.md` & `svcs-23.8.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/.github/workflows/ci.yml` & `svcs-23.8.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     tags: ["*"]
   pull_request:
     branches: [main]
   workflow_dispatch:
 
 env:
   FORCE_COLOR: "1" # Make tools pretty.
-  PYTHONIOENCODING: utf-8
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_PYTHON_VERSION_WARNING: "1"
 
 jobs:
   build-package:
     name: Build & verify package
     runs-on: ubuntu-latest
```

### Comparing `svcs-23.7.0/.github/workflows/codeql-analysis.yml` & `svcs-23.8.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/.github/workflows/pypi-package.yml` & `svcs-23.8.0/.github/workflows/pypi-package.yml`

 * *Files 22% similar despite different names*

```diff
@@ -10,46 +10,51 @@
       - published
   workflow_dispatch:
 
 permissions:
   contents: read
   id-token: write
 
+env:
+  FORCE_COLOR: "1" # Make tools pretty.
+  PIP_DISABLE_PIP_VERSION_CHECK: "1"
+  PIP_NO_PYTHON_VERSION_WARNING: "1"
+
 jobs:
   # Always build & lint package.
   build-package:
     name: Build & verify package
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
   # Upload to Test PyPI on every commit on main.
-  # release-test-pypi:
-  #   name: Publish in-dev package to test.pypi.org
-  #   environment: release-test-pypi
-  #   if: github.event_name == 'push' && github.ref == 'refs/heads/main'
-  #   runs-on: ubuntu-latest
-  #   needs: build-package
-
-  #   steps:
-  #     - name: Download packages built by build-and-inspect-python-package
-  #       uses: actions/download-artifact@v3
-  #       with:
-  #         name: Packages
-  #         path: dist
-
-  #     - name: Upload package to Test PyPI
-  #       uses: pypa/gh-action-pypi-publish@release/v1
-  #       with:
-  #         repository-url: https://test.pypi.org/legacy/
+  release-test-pypi:
+    name: Publish in-dev package to test.pypi.org
+    environment: release-test-pypi
+    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
+    runs-on: ubuntu-latest
+    needs: build-package
+
+    steps:
+      - name: Download packages built by build-and-inspect-python-package
+        uses: actions/download-artifact@v3
+        with:
+          name: Packages
+          path: dist
+
+      - name: Upload package to Test PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          repository-url: https://test.pypi.org/legacy/
 
   # Upload to real PyPI on GitHub Releases.
   release-pypi:
     name: Publish released package to pypi.org
     environment: release-pypi
     if: github.event.action == 'published'
     runs-on: ubuntu-latest
```

### Comparing `svcs-23.7.0/src/svcs/__init__.py` & `svcs-23.8.0/src/svcs/__init__.py`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/src/svcs/_core.py` & `svcs-23.8.0/src/svcs/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,63 +41,87 @@
 
     def __repr__(self) -> str:
         return (
             f"<Container(instantiated={len(self._instantiated)}, "
             f"cleanups={len(self._on_close)})>"
         )
 
-    def get(self, svc_type: type) -> Any:
+    def get(self, *svc_types: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it if necessary and register its cleanup.
 
         Returns:
-             :class:`typing.Any` until
+             If one service is requested, it's returned directly. If multiple
+             are requested, a sequence of services is returned.
+
+        Note:
+             Returns :class:`typing.Any` until
              https://github.com/python/mypy/issues/4717 is fixed.
         """
-        if (svc := self._instantiated.get(svc_type)) is not None:
-            return svc
+        rv = []
+        for svc_type in svc_types:
+            if (svc := self._instantiated.get(svc_type)) is not None:
+                rv.append(svc)
+                continue
+
+            rs = self.registry.get_registered_service_for(svc_type)
+            svc = rs.factory(self) if rs.takes_container else rs.factory()
+
+            if isinstance(svc, Generator):
+                self._on_close.append((rs.name, svc))
+                svc = next(svc)
 
-        rs = self.registry.get_registered_service_for(svc_type)
-        svc = rs.factory(self) if rs.takes_container else rs.factory()
+            self._instantiated[svc_type] = svc
 
-        if isinstance(svc, Generator):
-            self._on_close.append((rs.name, svc))
-            svc = next(svc)
+            rv.append(svc)
 
-        self._instantiated[svc_type] = svc
+        if len(rv) == 1:
+            return rv[0]
 
-        return svc
+        return rv
 
-    async def aget(self, svc_type: type) -> Any:
+    async def aget(self, *svc_types: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it asynchronously if necessary and register its cleanup.
 
         Returns:
-             :class:`typing.Any` until
+             If one service is requested, it's returned directly. If multiple
+             are requested, a sequence of services is returned.
+
+        Note:
+             Returns :class:`typing.Any` until
              https://github.com/python/mypy/issues/4717 is fixed.
         """
-        if (svc := self._instantiated.get(svc_type)) is not None:
-            return svc
+        rv = []
+        for svc_type in svc_types:
+            if (svc := self._instantiated.get(svc_type)) is not None:
+                rv.append(svc)
+                continue
+
+            rs = self.registry.get_registered_service_for(svc_type)
+            svc = rs.factory()
+
+            if isinstance(svc, AsyncGenerator):
+                self._on_close.append((rs.name, svc))
+                svc = await anext(svc)
+            elif isawaitable(svc):
+                svc = await svc
 
-        rs = self.registry.get_registered_service_for(svc_type)
-        svc = rs.factory()
+            self._instantiated[rs.svc_type] = svc
 
-        if isinstance(svc, AsyncGenerator):
-            self._on_close.append((rs.name, svc))
-            svc = await anext(svc)
-        elif isawaitable(svc):
-            svc = await svc
+            rv.append(svc)
 
-        self._instantiated[rs.svc_type] = svc
+        if len(rv) == 1:
+            return rv[0]
 
-        return svc
+        return rv
 
     def forget_about(self, svc_type: type) -> None:
         """
         Remove all traces of *svc_type* from ourselves.
         """
         with suppress(KeyError):
             del self._instantiated[svc_type]
```

### Comparing `svcs-23.7.0/src/svcs/flask.py` & `svcs-23.8.0/src/svcs/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 
     app.config["svcs_registry"] = registry
     app.teardown_appcontext(teardown)
 
     return app
 
 
-def get(svc_type: type) -> Any:
+def get(*svc_types: type) -> Any:
     """
     Same as :meth:`svcs.Container.get()`, but uses container on :obj:`flask.g`.
     """
     _, container = _ensure_req_data()
 
-    return container.get(svc_type)
+    return container.get(*svc_types)
 
 
 def register_factory(
     app: Flask,
     svc_type: type,
     factory: Callable,
     *,
```

### Comparing `svcs-23.7.0/tests/test_container.py` & `svcs-23.8.0/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/tests/test_fake_factories.py` & `svcs-23.8.0/tests/test_fake_factories.py`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/tests/test_flask.py` & `svcs-23.8.0/tests/test_flask.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,25 @@
 @pytest.fixture(name="container")
 def _container(clean_app_ctx):
     return svcs.flask._ensure_req_data()[1]
 
 
 @pytest.mark.usefixtures("clean_app_ctx")
 class TestFlask:
+    def test_register_value_multiple(self, app, registry):
+        """
+        register_value registers a service object on an app and get returns as
+        many values as are requeste.
+        """
+        registry.register_value(Service, 1)
+        registry.register_value(AnotherService, 2)
+
+        assert [1, 2] == svcs.flask.get(Service, AnotherService)
+        assert [1, 2] == svcs.flask.get(Service, AnotherService)
+
     def test_cleanup_added(self, registry):
         """
         get() handles the case where there is already a cleanup registered.
         """
 
         cleanup1 = Mock()
         cleanup2 = Mock()
```

### Comparing `svcs-23.7.0/tests/test_integration.py` & `svcs-23.8.0/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 
     svc = container.get(Service)
 
     assert isinstance(svc, Service)
     assert svc is container.get(Service)
 
 
-def test_register_value_get(registry, container, svc):
+def test_register_value_multiple(registry, container):
     """
-    register_value registers a service object and get returns it.
+    register_value registers a service object and get returns as many values as
+    are requeste.
     """
-    registry.register_value(Service, svc)
+    registry.register_value(Service, 1)
+    registry.register_value(AnotherService, 2)
 
-    assert svc is container.get(Service)
-    assert svc is container.get(Service)
+    assert [1, 2] == container.get(Service, AnotherService)
+    assert [1, 2] == container.get(Service, AnotherService)
 
 
 def test_get_not_found(container):
     """
     Asking for a service that isn't registered raises a ServiceNotFoundError.
     """
     with pytest.raises(svcs.exceptions.ServiceNotFoundError) as ei:
@@ -192,16 +194,18 @@
         assert Service() == (await container.aget(Service))
 
     async def test_aget_works_with_value(self, registry, container):
         """
         A value instead of a factory does not break aget().
         """
         registry.register_value(Service, 42)
+        registry.register_value(AnotherService, 23)
 
-        assert 42 == (await container.aget(Service))
+        assert [42, 23] == (await container.aget(Service, AnotherService))
+        assert [42, 23] == (await container.aget(Service, AnotherService))
 
     async def test_async_cleanup(self, registry, container):
         """
         Async cleanups are handled by aclose.
         """
         cleaned_up = False
```

### Comparing `svcs-23.7.0/tests/test_registry.py` & `svcs-23.8.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/tests/typing/core.py` & `svcs-23.8.0/tests/typing/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
 con = svcs.Container(reg)
 
 # The type checker believes whatever we tell it.
 o1: object = con.get(object)
 o2: int = con.get(object)
 
+o, i = con.get(object, int)
+
 con.close()
 
 with contextlib.closing(svcs.Container(reg)) as con:
     ...
 
 if sys.version_info >= (3, 10):
```

### Comparing `svcs-23.7.0/tests/typing/flask_.py` & `svcs-23.8.0/tests/typing/flask_.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 svcs.flask.register_factory(app, int, factory_with_cleanup)
 svcs.flask.register_value(app, str, str, ping=lambda: None)
 
 # The type checker believes whatever we tell it.
 o1: object = svcs.flask.get(object)
 o2: int = svcs.flask.get(object)
 
+o1, o2 = svcs.flask.get(object, int)
+
 svcs.flask.close_registry(app)
 
 
 class CustomApp(Flask):
     pass
```

### Comparing `svcs-23.7.0/LICENSE` & `svcs-23.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/pyproject.toml` & `svcs-23.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svcs-23.7.0/PKG-INFO` & `svcs-23.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.7.0
+Version: 23.8.0
 Summary: A Lightweight Service Locator
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
@@ -30,70 +30,78 @@
 Provides-Extra: typing
 Requires-Dist: flask; extra == 'typing'
 Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo_with_name.svg" width="25%" alt="svcs logo showing a radar"" />
+    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo_with_name.svg" width="35%" alt="svcs logo showing a radar"" />
   </a>
 </p>
 
 <p align="center">
-  A Lightweight Service Locator for Python.
+  <em>A Lightweight Service Locator for Python.</em>
 </p>
 
-> **WARNING** ☠️ Not ready yet! ☠️
+> **WARNING**
+> ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
 ---
 
-**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way without worrying about *cleaning them up*.**
+**This allows you to configure and manage all your resources in *one central place*, access them in a *consistent* way without worrying about *cleaning them up* and achieve *loose coupling*.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
-If you follow the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
+If you follow the [**_Dependency Inversion Principle_**](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [*abstract base class*](https://docs.python.org/3.11/library/abc.html).
+
+If you follow the [**_Hexagonal Architecture_**](https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)) (aka "*ports and adapters*"), the registered types are *ports* and the factories produce the *adapters*.
+*svcs* gives you a well-defined way to make your application *pluggable*.
 
 Benefits:
 
 - Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
-- simplifies **testing**,
+- simplifies **testing** through **loose coupling**,
 - and allows for easy **health checks** across *all* resources.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
     api = request.services.get(WebAPIClient)
 ```
 
-or, if you don't shy away from some global state, even:
+You can also ask for multiple services at once:
 
 ```python
-def view():
-    db = services.get(Database)
-    api = services.get(WebAPIClient)
+def view(request):
+    db, api = request.services.get(Database, WebAPIClient)
 ```
 
-The latter already works with [Flask](#flask) by utilizing the [`g` object](https://flask.palletsprojects.com/en/latest/api/#flask.g).
+Or, if you don't shy away from some global state and your web framework supports it, even:
+
+```python
+def view():
+    db, api = svcs.flask.get(Database, WebAPIClient)
+```
 
 You set it up like this:
 
 <!--
 ; skip: next
 -->
 
@@ -168,23 +176,24 @@
 For now, please refer to the [GitHub README](https://github.com/hynek/svcs/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
 ### Added
 
-- Factories now may take a parameter called `svcs_container` or that is annotated to be `svcs.Container`.
-  In this case the factory will receive the current container as a first positional argument.
-  This allows for recursive factories without global state.
-  [#10](https://github.com/hynek/svcs/pull/10)
+- It's now possible to request multiple services at once by passing multiple types to `Container.get()` and `Container.aget()`.
+  [#15](https://github.com/hynek/svcs/pull/15)
+
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svcs/blob/main/CHANGELOG.md)
 
 
 ## Credits
 
 *svcs* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://github.com/hynek/svcs/blob/main/LICENSE) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
+
+The [Bestagon](https://www.youtube.com/watch?v=thOifuHs6eY) locator logo is made by [Lynn Root](https://www.roguelynn.com), based on an [Font Awesome](https://fontawesome.com) Icon.
```

