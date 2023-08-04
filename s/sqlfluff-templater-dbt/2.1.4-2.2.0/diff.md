# Comparing `tmp/sqlfluff-templater-dbt-2.1.4.tar.gz` & `tmp/sqlfluff-templater-dbt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-3jz2muzp/sqlfluff-templater-dbt-2.1.4.tar", last modified: Tue Jul 25 10:29:05 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-wn484wkj/sqlfluff-templater-dbt-2.2.0.tar", last modified: Fri Aug  4 16:59:17 2023, max compression
```

## Comparing `sqlfluff-templater-dbt-2.1.4.tar` & `sqlfluff-templater-dbt-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 10:28:47.000000 sqlfluff-templater-dbt-2.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 10:28:47.000000 sqlfluff-templater-dbt-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-25 10:28:47.000000 sqlfluff-templater-dbt-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 10:28:47.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-07-25 10:28:47.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 10:29:05.000000 sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 16:59:02.000000 sqlfluff-templater-dbt-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-04 16:59:02.000000 sqlfluff-templater-dbt-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-04 16:59:02.000000 sqlfluff-templater-dbt-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-04 16:59:02.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30107 2023-08-04 16:59:02.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 16:59:17.000000 sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-2.1.4/LICENSE.md` & `sqlfluff-templater-dbt-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.1.4/PKG-INFO` & `sqlfluff-templater-dbt-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.4
+Version: 2.2.0
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-templater-dbt-2.1.4/setup.cfg` & `sqlfluff-templater-dbt-2.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 2.1.4
+version = 2.2.0
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -61,15 +61,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	sqlfluff==2.1.4
+	sqlfluff==2.2.0
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt/templater.py` & `sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt/templater.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,72 @@
-"""Defines the templaters."""
+"""Defines the dbt templater.
+
+NOTE: The dbt python package adds a significant overhead to import.
+This module is also loaded on every run of SQLFluff regardless of
+whether the dbt templater is selected in the configuration.
+
+The templater is however only _instantiated_ when selected, and as
+such, all imports of the dbt libraries are contained within the
+DbtTemplater class and so are only imported when necessary.
+"""
 
 from collections import deque
 from contextlib import contextmanager
 import os
 import os.path
 import logging
-from typing import List, Optional, Iterator, Tuple, Any, Dict, Deque, Union
+from typing import (
+    Callable,
+    List,
+    Optional,
+    Iterator,
+    Tuple,
+    Any,
+    Dict,
+    Deque,
+    Union,
+    TYPE_CHECKING,
+)
 
 from dataclasses import dataclass
 
-from dbt.version import get_installed_version
-from dbt.config import read_user_config
-from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
-from dbt.adapters.factory import register_adapter, get_adapter
-from dbt.compilation import Compiler as DbtCompiler
-
-# From dbt 1.3 onwards, the default_profiles_dir resolver is
-# available. Before that version we use the flags module
-try:
-    from dbt.cli.resolvers import default_profiles_dir
-except ImportError:
-    default_profiles_dir = None
-
-# After this PR on dbt-core, we need to inject context variables
-# directly. This change was backported and so exists in some versions
-# but not others. When not present, no additional action is needed.
-# https://github.com/dbt-labs/dbt-core/pull/7949
-# On the 1.5.x branch this was between 1.5.1 and 1.5.2
-try:
-    from dbt.task.contextvars import cv_project_root
-except ImportError:
-    cv_project_root = None
-
-try:
-    from dbt.exceptions import (
-        CompilationException as DbtCompilationException,
-        FailedToConnectException as DbtFailedToConnectException,
-        DbtProjectError,
-    )
-except ImportError:
-    from dbt.exceptions import (
-        CompilationError as DbtCompilationException,
-        FailedToConnectError as DbtFailedToConnectException,
-        DbtProjectError,
-    )
-
-from dbt import flags
 from jinja2 import Environment
 from jinja2_simple_tags import StandaloneTag
 
-from sqlfluff.cli.formatters import OutputStreamFormatter
-from sqlfluff.core import FluffConfig
 from sqlfluff.core.cached_property import cached_property
 from sqlfluff.core.errors import SQLTemplaterError, SQLFluffSkipFile, SQLFluffUserError
 
 from sqlfluff.core.templaters.base import TemplatedFile, large_file_check
 
 from sqlfluff.core.templaters.jinja import JinjaTemplater
 
+if TYPE_CHECKING:  # pragma: no cover
+    from dbt.semver import VersionSpecifier
+    from sqlfluff.core import FluffConfig
+    from sqlfluff.cli.formatters import OutputStreamFormatter
+
 # Instantiate the templater logger
 templater_logger = logging.getLogger("sqlfluff.templater")
 
 
-DBT_VERSION = get_installed_version()
-DBT_VERSION_STRING = DBT_VERSION.to_version_string()
-DBT_VERSION_TUPLE = (int(DBT_VERSION.major), int(DBT_VERSION.minor))
-
-if DBT_VERSION_TUPLE >= (1, 3):
-    COMPILED_SQL_ATTRIBUTE = "compiled_code"
-    RAW_SQL_ATTRIBUTE = "raw_code"
-else:  # pragma: no cover
-    COMPILED_SQL_ATTRIBUTE = "compiled_sql"
-    RAW_SQL_ATTRIBUTE = "raw_sql"
-
-
 @dataclass
 class DbtConfigArgs:
     """Arguments to load dbt runtime config."""
 
     project_dir: Optional[str] = None
     profiles_dir: Optional[str] = None
     profile: Optional[str] = None
     target: Optional[str] = None
     threads: int = 1
     single_threaded: bool = False
     # dict in 1.5.x onwards, json string before.
-    vars: Optional[Union[Dict, str]] = None if DBT_VERSION_TUPLE >= (1, 5) else ""
+    # NOTE: We always set this value when instantiating this
+    # class. If we rely on defaults, this should default to
+    # an empty string pre 1.5.x
+    vars: Optional[Union[Dict, str]] = None
     # NOTE: The `which` argument here isn't covered in tests, but many
     # dbt packages assume that it will have been set.
     # https://github.com/sqlfluff/sqlfluff/issues/4861
     # https://github.com/sqlfluff/sqlfluff/issues/4965
     which: Optional[str] = "compile"
 
 
@@ -105,27 +82,50 @@
         self.formatter = None
         self.project_dir = None
         self.profiles_dir = None
         self.working_dir = os.getcwd()
         self._sequential_fails = 0
         super().__init__(**kwargs)
 
-    def config_pairs(self):  # pragma: no cover TODO?
+    def config_pairs(self):
         """Returns info about the given templater for output by the cli."""
         return [("templater", self.name), ("dbt", self.dbt_version)]
 
-    @property
-    def dbt_version(self):  # pragma: no cover
+    @cached_property
+    def _dbt_version(self) -> "VersionSpecifier":
+        """Fetches the installed dbt version.
+
+        This is cached in the raw dbt format.
+
+        NOTE: We do this only on demand to reduce the amount of loading
+        required to discover the templater.
+        """
+        from dbt.version import get_installed_version
+
+        return get_installed_version()
+
+    @cached_property
+    def dbt_version(self):
         """Gets the dbt version."""
-        return DBT_VERSION_STRING
+        return self._dbt_version.to_version_string()
+
+    @cached_property
+    def dbt_version_tuple(self):
+        """Gets the dbt version."""
+        return int(self._dbt_version.major), int(self._dbt_version.minor)
 
     @cached_property
     def dbt_config(self):
         """Loads the dbt config."""
-        if DBT_VERSION_TUPLE >= (1, 5):
+        from dbt import flags
+        from dbt.config import read_user_config
+        from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
+        from dbt.adapters.factory import register_adapter
+
+        if self.dbt_version_tuple >= (1, 5):
             user_config = None
             # 1.5.x+ this is a dict.
             cli_vars = self._get_cli_vars()
         else:
             # Here, we read flags.PROFILE_DIR directly, prior to calling
             # set_from_args(). Apparently, set_from_args() sets PROFILES_DIR
             # to a lowercase version of the value, and the profile wouldn't be
@@ -158,20 +158,24 @@
         )
         register_adapter(self.dbt_config)
         return self.dbt_config
 
     @cached_property
     def dbt_compiler(self):
         """Loads the dbt compiler."""
+        from dbt.compilation import Compiler as DbtCompiler
+
         self.dbt_compiler = DbtCompiler(self.dbt_config)
         return self.dbt_compiler
 
     @cached_property
     def dbt_manifest(self):
         """Loads the dbt manifest."""
+        from dbt.exceptions import DbtProjectError
+
         # Set dbt not to run tracking. We don't load
         # a full project and so some tracking routines
         # may fail.
         from dbt.tracking import do_not_track
 
         do_not_track()
 
@@ -181,21 +185,21 @@
         old_cwd = os.getcwd()
         try:
             # Changing cwd temporarily as dbt is not using project_dir to
             # read/write `target/partial_parse.msgpack`. This can be undone when
             # https://github.com/dbt-labs/dbt-core/issues/6055 is solved.
             # For dbt 1.4+ this isn't necessary, but it is required for 1.3
             # and before.
-            if DBT_VERSION_TUPLE < (1, 4):
+            if self.dbt_version_tuple < (1, 4):
                 os.chdir(self.project_dir)
             self.dbt_manifest = ManifestLoader.get_full_manifest(self.dbt_config)
         except DbtProjectError as err:  # pragma: no cover
             raise SQLFluffUserError(f"DbtProjectError: {err}")
         finally:
-            if DBT_VERSION_TUPLE < (1, 4):
+            if self.dbt_version_tuple < (1, 4):
                 os.chdir(old_cwd)
 
         return self.dbt_manifest
 
     @cached_property
     def dbt_selector_method(self):
         """Loads the dbt selector method."""
@@ -231,14 +235,24 @@
         support a change of default in the future, as well
         as to support the same overwriting mechanism as
         dbt (currently an environment variable).
         """
         # Where default_profiles_dir is available, use it. For dbt 1.2 and
         # earlier, it is not, so fall back to the flags option which should
         # still be available in those versions.
+
+        from dbt import flags
+
+        # From dbt 1.3 onwards, the default_profiles_dir resolver is
+        # available. Before that version we use the flags module
+        try:
+            from dbt.cli.resolvers import default_profiles_dir
+        except ImportError:
+            default_profiles_dir = None
+
         default_dir = (
             default_profiles_dir()
             if default_profiles_dir is not None
             else flags.PROFILES_DIR
         )
 
         dbt_profiles_dir = os.path.abspath(
@@ -375,16 +389,16 @@
 
     @large_file_check
     def process(
         self,
         *,
         fname: str,
         in_str: Optional[str] = None,
-        config: Optional[FluffConfig] = None,
-        formatter: Optional[OutputStreamFormatter] = None,
+        config: Optional["FluffConfig"] = None,
+        formatter: Optional["OutputStreamFormatter"] = None,
     ):
         """Compile a dbt model and return the compiled SQL.
 
         Args:
             fname: Path to dbt model(s)
             in_str: fname contents using configured encoding
             config: A specific config to use for this
@@ -395,14 +409,25 @@
         self.formatter = formatter
         self.sqlfluff_config = config
         self.project_dir = self._get_project_dir()
         self.profiles_dir = self._get_profiles_dir()
         fname_absolute_path = os.path.abspath(fname)
 
         try:
+            from dbt.exceptions import (
+                CompilationException as DbtCompilationException,
+                FailedToConnectException as DbtFailedToConnectException,
+            )
+        except ImportError:
+            from dbt.exceptions import (
+                CompilationError as DbtCompilationException,
+                FailedToConnectError as DbtFailedToConnectException,
+            )
+
+        try:
             os.chdir(self.project_dir)
             processed_result = self._unsafe_process(fname_absolute_path, in_str, config)
             # Reset the fail counter
             self._sequential_fails = 0
             return processed_result
         except DbtCompilationException as e:
             # Increment the counter
@@ -490,42 +515,61 @@
         # - Jinja Environment object
         # - Jinja "globals" dictionary
         #
         # This info is captured by the "make_template()" function, which in
         # turn is used by our parent class' (JinjaTemplater) slice_file()
         # function.
         old_from_string = Environment.from_string
-        make_template = None
+        # Start with render_func undefined. We need to know whether it has been
+        # overwritten.
+        render_func: Optional[Callable[[str], str]] = None
+
+        if self.dbt_version_tuple >= (1, 3):
+            compiled_sql_attribute = "compiled_code"
+            raw_sql_attribute = "raw_code"
+        else:  # pragma: no cover
+            compiled_sql_attribute = "compiled_sql"
+            raw_sql_attribute = "raw_sql"
 
         def from_string(*args, **kwargs):
             """Replaces (via monkeypatch) the jinja2.Environment function."""
-            nonlocal make_template
+            nonlocal render_func
             # Is it processing the node corresponding to fname?
             globals = kwargs.get("globals")
             if globals:
                 model = globals.get("model")
                 if model:
                     if model.get("original_file_path") == original_file_path:
                         # Yes. Capture the important arguments and create
-                        # a make_template() function.
+                        # a render_func() closure with overwrites the variable
+                        # from within _unsafe_process when from_string is run.
                         env = args[0]
                         globals = args[2] if len(args) >= 3 else kwargs["globals"]
 
-                        def make_template(in_str):
+                        # Overwrite the outer render_func
+                        def render_func(in_str):
                             env.add_extension(SnapshotExtension)
-                            return env.from_string(in_str, globals=globals)
+                            template = env.from_string(in_str, globals=globals)
+                            return template.render()
 
             return old_from_string(*args, **kwargs)
 
         # NOTE: We need to inject the project root here in reaction to the
         # breaking change upstream with dbt. Coverage works in 1.5.2, but
         # appears to no longer be covered in 1.5.3.
+        # This change was backported and so exists in some versions
+        # but not others. When not present, no additional action is needed.
         # https://github.com/dbt-labs/dbt-core/pull/7949
-        if cv_project_root is not None:  # pragma: no cover
-            cv_project_root.set(self.project_dir)
+        # On the 1.5.x branch this was between 1.5.1 and 1.5.2
+        try:
+            from dbt.task.contextvars import cv_project_root
+
+            cv_project_root.set(self.project_dir)  # pragma: no cover
+        except ImportError:
+            cv_project_root = None
 
         node = self._find_node(fname, config)
         templater_logger.debug(
             "_find_node for path %r returned object of type %s.", fname, type(node)
         )
 
         save_ephemeral_nodes = dict(
@@ -562,17 +606,17 @@
 
             if hasattr(node, "injected_sql"):
                 # If injected SQL is present, it contains a better picture
                 # of what will actually hit the database (e.g. with tests).
                 # However it's not always present.
                 compiled_sql = node.injected_sql  # pragma: no cover
             else:
-                compiled_sql = getattr(node, COMPILED_SQL_ATTRIBUTE)
+                compiled_sql = getattr(node, compiled_sql_attribute)
 
-            raw_sql = getattr(node, RAW_SQL_ATTRIBUTE)
+            raw_sql = getattr(node, raw_sql_attribute)
 
             if not compiled_sql:  # pragma: no cover
                 raise SQLTemplaterError(
                     "dbt templater compilation failed silently, check your "
                     "configuration by running `dbt compile` directly."
                 )
             source_dbt_sql = in_str
@@ -611,29 +655,44 @@
             #    1. Check for trailing newlines before compiling by looking at the
             #       raw SQL in the source dbt file. Remember the count of trailing
             #       newlines.
             #    2. Set node.raw_sql/node.raw_code to the original source file contents.
             #    3. Append the count from #1 above to compiled_sql. (In
             #       production, slice_file() does not usually use this string,
             #       but some test scenarios do.
-            setattr(node, RAW_SQL_ATTRIBUTE, source_dbt_sql)
-            compiled_sql = compiled_sql + "\n" * n_trailing_newlines
+            setattr(node, raw_sql_attribute, source_dbt_sql)
+
+            # So for files that have no templated elements in them, render_func
+            # will still be null at this point. If so, we replace it with a lambda
+            # which just directly returns the input , but _also_ reset the trailing
+            # newlines counter because they also won't have been stripped.
+            if render_func is None:
+                # NOTE: In this case, we shouldn't re-add newlines, because they
+                # were never taken away.
+                n_trailing_newlines = 0
+
+                # Overwrite the render_func placeholder.
+                def render_func(in_str):
+                    """A render function which just returns the input."""
+                    return in_str
+
+            # At this point assert that we _have_ a render_func
+            assert render_func is not None
 
             # TRICKY: dbt configures Jinja2 with keep_trailing_newline=False.
             # As documented (https://jinja.palletsprojects.com/en/3.0.x/api/),
             # this flag's behavior is: "Preserve the trailing newline when
             # rendering templates. The default is False, which causes a single
             # newline, if present, to be stripped from the end of the template."
             #
             # Below, we use "append_to_templated" to effectively "undo" this.
             raw_sliced, sliced_file, templated_sql = self.slice_file(
                 source_dbt_sql,
-                compiled_sql,
+                render_func=render_func,
                 config=config,
-                make_template=make_template,
                 append_to_templated="\n" if n_trailing_newlines else "",
             )
         # :HACK: If calling compile_node() compiled any ephemeral nodes,
         # restore them to their earlier state. This prevents a runtime error
         # in the dbt "_inject_ctes_into_sql()" function that occurs with
         # 2nd-level ephemeral model dependencies (e.g. A -> B -> C, where
         # both B and C are ephemeral). Perhaps there is a better way to do
@@ -652,14 +711,16 @@
             # No violations returned in this way.
             [],
         )
 
     @contextmanager
     def connection(self):
         """Context manager that manages a dbt connection, if needed."""
+        from dbt.adapters.factory import get_adapter
+
         # We have to register the connection in dbt >= 1.0.0 ourselves
         # In previous versions, we relied on the functionality removed in
         # https://github.com/dbt-labs/dbt-core/pull/4062.
         adapter = self.adapters.get(self.project_dir)
         if adapter is None:
             adapter = get_adapter(self.dbt_config)
             self.adapters[self.project_dir] = adapter
```

### Comparing `sqlfluff-templater-dbt-2.1.4/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff-templater-dbt-2.2.0/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.4
+Version: 2.2.0
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

