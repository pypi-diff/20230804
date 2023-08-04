# Comparing `tmp/ez_cqrs-2.3.2.tar.gz` & `tmp/ez_cqrs-2.4.0.tar.gz`

## Comparing `ez_cqrs-2.3.2.tar` & `ez_cqrs-2.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/error.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/py.typed
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.4.0/PKG-INFO
```

### Comparing `ez_cqrs-2.3.2/.github/workflows/release.yml` & `ez_cqrs-2.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/.github/workflows/test.yml` & `ez_cqrs-2.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/.vscode/settings.json` & `ez_cqrs-2.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/acid_exec.py` & `ez_cqrs-2.4.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/components.py` & `ez_cqrs-2.4.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/error.py` & `ez_cqrs-2.4.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/handler.py` & `ez_cqrs-2.4.0/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.4.0/ez_cqrs/framework/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ez_cqrs.components import OUT, C, E
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import ACID
-    from ez_cqrs.error import ExecutionError
+    from ez_cqrs.error import DatabaseError, ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
 
 T = TypeVar("T")
 
 
 @final
 @dataclass(repr=True, frozen=True, eq=False)
@@ -56,29 +56,44 @@
         execution_result_or_err = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
                 ops_registry=ops_registry,
                 event_registry=event_registry,
             ),
         )
+        commited_or_err = self._commit_existing_transactions(
+            max_transactions=max_transactions,
+            ops_registry=ops_registry,
+            app_database=app_database,
+        )
+        if not isinstance(commited_or_err, Ok):
+            return commited_or_err
+
         if not isinstance(execution_result_or_err, Ok):
             return execution_result_or_err
 
+        event_dispatch_tasks = (
+            self.event_dispatcher.dispatch(x) for x in event_registry
+        )
+
+        asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
+
+        return Ok(execution_result_or_err.unwrap())
+
+    def _commit_existing_transactions(
+        self,
+        max_transactions: int,
+        ops_registry: OpsRegistry[Any],
+        app_database: ACID | None,
+    ) -> Result[None, DatabaseError]:
         if app_database and max_transactions > 0:
             if ops_registry.storage_length() > 0:
                 commited_or_err = app_database.commit_as_transaction(
                     ops_registry=ops_registry,
                 )
                 if not isinstance(commited_or_err, Ok):
                     return commited_or_err
 
             if not ops_registry.is_empty():
                 msg = "Ops registry didn't came empty after transactions commit."
                 raise RuntimeError(msg)
-
-        event_dispatch_tasks = (
-            self.event_dispatcher.dispatch(x) for x in event_registry
-        )
-
-        asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
-
-        return Ok(execution_result_or_err.unwrap())
+        return Ok(None)
```

### Comparing `ez_cqrs-2.3.2/ez_cqrs/framework/testing.py` & `ez_cqrs-2.4.0/ez_cqrs/framework/testing.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.4.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/requirements/dev.txt` & `ez_cqrs-2.4.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/scripts/new_release.py` & `ez_cqrs-2.4.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/tests/conftest.py` & `ez_cqrs-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/tests/test_acid_exec.py` & `ez_cqrs-2.4.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/tests/test_framework.py` & `ez_cqrs-2.4.0/tests/test_framework.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/.gitignore` & `ez_cqrs-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/LICENSE` & `ez_cqrs-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.3.2/pyproject.toml` & `ez_cqrs-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.3.2"
+version = "2.4.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.3.2/PKG-INFO` & `ez_cqrs-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.3.2
+Version: 2.4.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

