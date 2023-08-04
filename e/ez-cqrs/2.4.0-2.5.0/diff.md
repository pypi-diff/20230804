# Comparing `tmp/ez_cqrs-2.4.0.tar.gz` & `tmp/ez_cqrs-2.5.0.tar.gz`

## Comparing `ez_cqrs-2.4.0.tar` & `ez_cqrs-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.5.0/PKG-INFO
```

### Comparing `ez_cqrs-2.4.0/.github/workflows/release.yml` & `ez_cqrs-2.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/.github/workflows/test.yml` & `ez_cqrs-2.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/.vscode/settings.json` & `ez_cqrs-2.5.0/.vscode/settings.json`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "editor.wordBasedSuggestions": false
     },
     "python.analysis.autoImportCompletions": true,
     "python.analysis.extraCommitChars": false,
     "python.analysis.inlayHints.callArgumentNames": false,
     "python.analysis.inlayHints.pytestParameters": false,
     "python.analysis.inlayHints.functionReturnTypes": false,
-    "python.analysis.inlayHints.variableTypes": false,
+    "python.analysis.inlayHints.variableTypes": true,
     "python.analysis.typeCheckingMode": "basic",
     "python.analysis.userFileIndexingLimit": 200,
     "python.testing.unittestEnabled": false,
     "python.testing.pytestEnabled": true,
     "python.analysis.diagnosticMode": "workspace",
     "[toml]": {"editor.formatOnSave": true},
     "json.format.enable": true,
```

### Comparing `ez_cqrs-2.4.0/ez_cqrs/acid_exec.py` & `ez_cqrs-2.5.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/ez_cqrs/components.py` & `ez_cqrs-2.5.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/ez_cqrs/error.py` & `ez_cqrs-2.5.0/ez_cqrs/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,10 +44,9 @@
 
     def __init__(self, unexpected_error: Exception) -> None:  # noqa: D107
         super().__init__(f"Unexpected error {unexpected_error}")
 
 
 ExecutionError: TypeAlias = Union[
     DomainError,
-    DatabaseError,
     UnexpectedError,
 ]
```

### Comparing `ez_cqrs-2.4.0/ez_cqrs/handler.py` & `ez_cqrs-2.5.0/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.5.0/ez_cqrs/framework/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Ez-Cqrs Framwork."""
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, final
 
-from result import Ok
+from result import Err, Ok
 
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import OUT, C, E
+from ez_cqrs.error import UnexpectedError
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import ACID
-    from ez_cqrs.error import DatabaseError, ExecutionError
+    from ez_cqrs.error import DatabaseError, DomainError, ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
 
 T = TypeVar("T")
 
 
 @final
 @dataclass(repr=True, frozen=True, eq=False)
@@ -31,15 +32,15 @@
 
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         app_database: ACID | None,
         event_registry: list[E],
-    ) -> Result[OUT, ExecutionError | pydantic.ValidationError]:
+    ) -> Result[OUT, ExecutionError | pydantic.ValidationError | DatabaseError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         if max_transactions > 0 and not app_database:
             msg = "You are not setting a database to commit transactions"
@@ -56,31 +57,38 @@
         execution_result_or_err = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
                 ops_registry=ops_registry,
                 event_registry=event_registry,
             ),
         )
+        execution_err: DomainError | None = None
+        if not isinstance(execution_result_or_err, Ok):
+            execution_error = execution_result_or_err.err()
+            if isinstance(execution_error, UnexpectedError):
+                return Err(execution_error)
+            execution_err = execution_error
+
         commited_or_err = self._commit_existing_transactions(
             max_transactions=max_transactions,
             ops_registry=ops_registry,
             app_database=app_database,
         )
         if not isinstance(commited_or_err, Ok):
             return commited_or_err
 
-        if not isinstance(execution_result_or_err, Ok):
-            return execution_result_or_err
-
         event_dispatch_tasks = (
             self.event_dispatcher.dispatch(x) for x in event_registry
         )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
+        if execution_err:
+            return Err(execution_err)
+
         return Ok(execution_result_or_err.unwrap())
 
     def _commit_existing_transactions(
         self,
         max_transactions: int,
         ops_registry: OpsRegistry[Any],
         app_database: ACID | None,
```

### Comparing `ez_cqrs-2.4.0/ez_cqrs/framework/testing.py` & `ez_cqrs-2.5.0/ez_cqrs/framework/testing.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.5.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/requirements/dev.txt` & `ez_cqrs-2.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/scripts/new_release.py` & `ez_cqrs-2.5.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/tests/conftest.py` & `ez_cqrs-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/tests/test_acid_exec.py` & `ez_cqrs-2.5.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/tests/test_framework.py` & `ez_cqrs-2.5.0/tests/test_framework.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/.gitignore` & `ez_cqrs-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/LICENSE` & `ez_cqrs-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.4.0/pyproject.toml` & `ez_cqrs-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.4.0"
+version = "2.5.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.4.0/PKG-INFO` & `ez_cqrs-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.4.0
+Version: 2.5.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

