# Comparing `tmp/jeeves_shell-2.1.9.tar.gz` & `tmp/jeeves_shell-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.9.tar", max compression
+gzip compressed data, was "jeeves_shell-2.2.0.tar", max compression
```

## Comparing `jeeves_shell-2.1.9.tar` & `jeeves_shell-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.9/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.9/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.9/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.9/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.9/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.9/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.9/jeeves_shell/errors.py
--rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.9/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.9/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1719 2023-05-18 20:15:19.119192 jeeves_shell-2.1.9/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 jeeves_shell-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.2.0/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.2.0/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.2.0/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3830 2023-05-24 21:27:35.336409 jeeves_shell-2.2.0/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.2.0/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.2.0/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.2.0/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.2.0/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1838 2023-08-04 11:58:24.637797 jeeves_shell-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 jeeves_shell-2.2.0/PKG-INFO
```

### Comparing `jeeves_shell-2.1.9/README.md` & `jeeves_shell-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.9/jeeves_shell/cli.py` & `jeeves_shell-2.2.0/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.9/jeeves_shell/discover.py` & `jeeves_shell-2.2.0/jeeves_shell/discover.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 logger = logging.getLogger('jeeves')
 
 
 def list_installed_plugins() -> List[Tuple[str, Jeeves]]:
     """Find installed plugins."""
     return [
-        (entry_point.name, entry_point.load())
-        for entry_point in entry_points(group='jeeves')
+        (entry_point.name, entry_point.load())  # type: ignore
+        for entry_point in entry_points(group='jeeves')  # type: ignore
     ]
 
 
 def _construct_app_from_plugins() -> Jeeves:   # pragma: nocover
     if os.getenv('JEEVES_DISABLE_PLUGINS'):
         plugins = []
     else:
@@ -64,17 +64,25 @@
     if not directory.exists():
         return
 
     try:
         jeeves_module = import_by_path(
             path=directory,
         )
-    except ImportError as err:
-        logger.debug('Cannot import: %s', err)
-        return
+
+    except ImportError as err:    # pragma: nocover
+        # We could not import something.
+        if err.name == 'jeeves':
+            # We couldn't import jeeves module. We can skip that.
+            logger.debug('Module not found: %s', err)
+            return
+
+        # Something that `jeeves` module is importing can't be imported, that is
+        # a problem.
+        raise
 
     for name, command in vars(jeeves_module).items():  # noqa: WPS421
         if not _is_name_suitable(name):
             continue
 
         if _is_function(command) or _is_typer(command):
             yield name, command
@@ -113,12 +121,15 @@
     app.callback()(_root_app_callback)
     return app
 
 
 def construct_app(current_directory: Optional[Path] = None) -> Jeeves:
     """Discover plugins and construct a Typer app."""
     if current_directory is None:       # pragma: no cover
-        current_directory = Path.cwd()
+        if directory_from_environment := os.environ.get('JEEVES_ROOT'):
+            current_directory = Path(directory_from_environment)
+        else:
+            current_directory = Path.cwd()
 
     app = _construct_app_from_plugins()
     app = _configure_callback(app)
     return _augment_app_with_jeeves_file(app=app, path=current_directory)
```

### Comparing `jeeves_shell-2.1.9/pyproject.toml` & `jeeves_shell-2.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.1.9"
+version = "2.2.0"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
@@ -27,15 +27,15 @@
 
 [tool.poetry.scripts]
 j = "jeeves_shell.cli:app"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-typer = "^0.7.0"
+typer = "^0.9.0"
 documented = "^0.1.1"
 more-itertools = "^9.0.0"
 sh = {version = "^2.0.4", optional = true}
 rich = {version = "^13.3.5", optional = true}
 
 [tool.poetry.extras]
 all = ["sh", "rich"]
@@ -45,15 +45,20 @@
 mkdocstrings = "^0.19.1"
 
 markupsafe = "<2.1"   # Otherwise, `jinja2` will fail
 importlib-metadata = "<5.0"
 mkdocs-macros-plugin = "^0.7.0"
 dominate = "^2.7.0"
 iolanta-tables = "^0.1.7"
-jeeves-yeti-pyproject = "^0.2.16"
+mkdocs-awesome-pages-plugin = "^2.9.1"
+mkdocs-material = "^9.1.13"
+mkdocs-iolanta = "^0.1.5"
+sh = "^2.0.4"
+iolanta-roadmap = "^0.1.0"
+urllib3 = "<2.0.0"
 
 [tool.flakeheaven.exceptions."jeeves_shell/jeeves.py"]
 wemake-python-styleguide = [
   "-WPS115",
   "-WPS600",
 ]
```

### Comparing `jeeves_shell-2.1.9/PKG-INFO` & `jeeves_shell-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.1.9
+Version: 2.2.0
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Requires-Dist: documented (>=0.1.1,<0.2.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0) ; extra == "all"
 Requires-Dist: sh (>=2.0.4,<3.0.0) ; extra == "all"
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jeeves-sh/jeeves-shell
 Description-Content-Type: text/markdown
 
 # Jeeves Shell
 
 [![Build Status](https://github.com/jeeves-sh/jeeves-shell/workflows/test/badge.svg?branch=master&event=push)](https://github.com/jeeves-sh/jeeves-shell/actions?query=workflow%3Atest)
 [![codecov](https://codecov.io/gh/jeeves-sh/jeeves-shell/branch/master/graph/badge.svg)](https://codecov.io/gh/jeeves-sh/jeeves-shell)
```

