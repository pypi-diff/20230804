# Comparing `tmp/bygg-0.1.0.tar.gz` & `tmp/bygg-0.1.1.tar.gz`

## Comparing `bygg-0.1.0.tar` & `bygg-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bygg-0.1.0/.tool-versions
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bygg-0.1.0/_version.py
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bygg-0.1.0/bootstrap.sh
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 bygg-0.1.0/mypy.sh
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 bygg-0.1.0/noxfile.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements-dev.in
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements.in
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 bygg-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.1.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 bygg-0.1.0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.1.0/.vscode/extensions.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bygg-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile.yml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile1.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/Byggfile2.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements1.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/environments/requirements2.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/.gitignore
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/Byggfile.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/Byggfile.yml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/parametric/README.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/taskrunner/Byggfile.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/Byggfile.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/Byggfile.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/input1.txt
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/more_things/MoreActions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/examples/trivial/more_things/__init__.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 bygg-0.1.0/schemas/Byggfile_yml_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/__init__.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/action.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/apply_configuration.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/cache.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/common_types.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/configuration.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/dag.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/digest.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/py.typed
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/runner.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/scaffolding.py
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/scheduler.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/status_display.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bygg-0.1.0/src/bygg/util.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_action.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_cache.py
--rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_scheduler.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bygg-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.1.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.1.0/LICENSE
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 bygg-0.1.0/README.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 bygg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 bygg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bygg-0.1.1/.tool-versions
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bygg-0.1.1/_version.py
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bygg-0.1.1/bootstrap.sh
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 bygg-0.1.1/mypy.sh
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 bygg-0.1.1/noxfile.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bygg-0.1.1/requirements-dev.in
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 bygg-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 bygg-0.1.1/requirements.in
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 bygg-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.1.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 bygg-0.1.1/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.1.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bygg-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/Byggfile.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/Byggfile.yml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/Byggfile1.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/Byggfile2.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/requirements1.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/environments/requirements2.txt
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/only_python/Byggfile.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/parametric/.gitignore
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/parametric/Byggfile.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/parametric/Byggfile.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/parametric/README.md
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/taskrunner/Byggfile.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/trivial/Byggfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/trivial/Byggfile.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/trivial/input1.txt
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/trivial/more_things/MoreActions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.1/examples/trivial/more_things/__init__.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 bygg-0.1.1/schemas/Byggfile_yml_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/__init__.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/action.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/apply_configuration.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/cache.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/common_types.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/configuration.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/dag.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/digest.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/py.typed
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/runner.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/scaffolding.py
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/scheduler.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/status_display.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bygg-0.1.1/src/bygg/util.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bygg-0.1.1/tests/test_action.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bygg-0.1.1/tests/test_cache.py
+-rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 bygg-0.1.1/tests/test_scheduler.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 bygg-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 bygg-0.1.1/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 bygg-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 bygg-0.1.1/PKG-INFO
```

### Comparing `bygg-0.1.0/noxfile.py` & `bygg-0.1.1/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     session.run("bygg", "--help", silent=True)
 
 
 @nox.session(python=["3.11"])
 def examples(session):
     session.install(".")
 
+    with session.chdir("examples/only_python"):
+        session.run("bygg")
+        session.run("bygg", "--clean")
+
     with session.chdir("examples/parametric"):
         session.run("bygg")
         session.run("bygg", "--clean")
 
     with session.chdir("examples/taskrunner"):
         session.run("bygg")
         session.run("bygg", "--clean")
```

### Comparing `bygg-0.1.0/requirements-dev.txt` & `bygg-0.1.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/requirements.txt` & `bygg-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/.github/workflows/pypi_publish.yml` & `bygg-0.1.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/.github/workflows/run_tests.yml` & `bygg-0.1.1/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/examples/environments/Byggfile.yml` & `bygg-0.1.1/examples/environments/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/examples/parametric/Byggfile.py` & `bygg-0.1.1/examples/parametric/Byggfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/examples/trivial/Byggfile.py` & `bygg-0.1.1/examples/trivial/Byggfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/examples/trivial/input1.txt` & `bygg-0.1.1/examples/trivial/input1.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/examples/trivial/more_things/MoreActions.py` & `bygg-0.1.1/examples/trivial/more_things/MoreActions.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/schemas/Byggfile_yml_schema.json` & `bygg-0.1.1/schemas/Byggfile_yml_schema.json`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/action.py` & `bygg-0.1.1/src/bygg/action.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/apply_configuration.py` & `bygg-0.1.1/src/bygg/apply_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,42 +92,42 @@
 
 def apply_configuration(
     configuration: ByggFile | None,
     environment_name: str | None,
     is_restarted_with_env: str | None,
 ) -> str | None:
     """Returns the path of the bygg install to restart with if a restart is needed."""
-    if not configuration:
-        return None
-
-    if not is_restarted_with_env and environment_name:
-        if environment_name in configuration.environments:
-            environment = configuration.environments[environment_name]
-            setup_environment(environment)
-
-            restart_with = should_restart_with(environment)
-            if restart_with is not None:
-                return restart_with
-
-    for action in configuration.actions:
-        # TODO Hack until we can iterate over the dependency graph in scheduler.prepare_run:
-        if is_restarted_with_env and action.environment != is_restarted_with_env:
-            continue
-
-        shell_command = (
-            create_shell_command(action.shell, action.message) if action.shell else None
-        )
-        Action(
-            action.name,
-            is_entrypoint=bool(action.is_entrypoint),
-            inputs=action.inputs,
-            outputs=action.outputs,
-            dependencies=action.dependencies,
-            command=shell_command,
-        )
+    if configuration:
+        if not is_restarted_with_env and environment_name:
+            if environment_name in configuration.environments:
+                environment = configuration.environments[environment_name]
+                setup_environment(environment)
+
+                restart_with = should_restart_with(environment)
+                if restart_with is not None:
+                    return restart_with
+
+        for action in configuration.actions:
+            # TODO Hack until we can iterate over the dependency graph in scheduler.prepare_run:
+            if is_restarted_with_env and action.environment != is_restarted_with_env:
+                continue
+
+            shell_command = (
+                create_shell_command(action.shell, action.message)
+                if action.shell
+                else None
+            )
+            Action(
+                action.name,
+                is_entrypoint=bool(action.is_entrypoint),
+                inputs=action.inputs,
+                outputs=action.outputs,
+                dependencies=action.dependencies,
+                command=shell_command,
+            )
 
     # Evaluate the Python build file:
 
     python_build_file = PYTHON_INPUTFILE
     if configuration and environment_name:
         environment = configuration.environments.get(environment_name, None)
         if environment:
```

### Comparing `bygg-0.1.0/src/bygg/cache.py` & `bygg-0.1.1/src/bygg/cache.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/configuration.py` & `bygg-0.1.1/src/bygg/configuration.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/dag.py` & `bygg-0.1.1/src/bygg/dag.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/digest.py` & `bygg-0.1.1/src/bygg/digest.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/main.py` & `bygg-0.1.1/src/bygg/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,20 @@
         rich.print("No build files found.")
         sys.exit(1)
 
     configuration = read_config_file()
     action_partitions = partition_actions(configuration, args.actions)
 
     if not action_partitions:
-        status = print_no_actions_text(configuration)
+        if os.path.isfile(PYTHON_INPUTFILE):
+            # No configuration file, so load the Python build file directly.
+            apply_configuration(None, None, None)
+            status = do_dispatch(args, args.actions)
+        else:
+            status = print_no_actions_text(configuration)
         if status:
             sys.exit(0)
         sys.exit(1)
 
     for partition in action_partitions:
         env = partition.environment_name
         # Check if we should restart with another Python interpreter (e.g. from a
@@ -214,28 +219,33 @@
             except FileNotFoundError:
                 rich.print(
                     f"[red]Error: Could not restart with '{restart_with}'.[/red]\n"
                     f"[yellow]Please make sure that bygg is in your pip requirements list for this environment.[/yellow]"
                 )
                 sys.exit(1)
         else:
-            if args.check:
-                status = check(args.actions)
-            elif args.clean:
-                status = clean(args.actions)
-            elif args.list:
-                status = list_actions()
-            else:
-                jobs = int(args.jobs) if args.jobs else None
-                status = build(partition.actions, jobs, args.always_make)
-
+            status = do_dispatch(args, partition.actions)
             if not status:
                 sys.exit(1)
 
 
+def do_dispatch(args: argparse.Namespace, actions: List[str]) -> bool:
+    if args.list or not actions:
+        status = list_actions()
+    elif args.check:
+        status = check(actions)
+    elif args.clean:
+        status = clean(actions)
+    else:
+        jobs = int(args.jobs) if args.jobs else None
+        status = build(actions, jobs, args.always_make)
+
+    return status
+
+
 @dataclass
 class ActionPartition:
     """
     environment_name: The name of the environment that the actions should be run in.
     None means the implicit default environment, i.e. typically the base process.
 
     actions: The actions that should be run in the environment.
```

### Comparing `bygg-0.1.0/src/bygg/runner.py` & `bygg-0.1.1/src/bygg/runner.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/scheduler.py` & `bygg-0.1.1/src/bygg/scheduler.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/status_display.py` & `bygg-0.1.1/src/bygg/status_display.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/src/bygg/util.py` & `bygg-0.1.1/src/bygg/util.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/tests/test_action.py` & `bygg-0.1.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/tests/test_cache.py` & `bygg-0.1.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/tests/test_scheduler.py` & `bygg-0.1.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/tests/test_utils.py` & `bygg-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/LICENSE` & `bygg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/README.md` & `bygg-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/pyproject.toml` & `bygg-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bygg-0.1.0/PKG-INFO` & `bygg-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bygg
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small build system
 Project-URL: Homepage, https://github.com/rikardg/bygg
 Project-URL: Bug Tracker, https://github.com/rikardg/bygg/issues
 Author-email: Rikard Gillemyr <rikard.gillemyr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 rikardg
```

