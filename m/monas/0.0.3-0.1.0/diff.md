# Comparing `tmp/monas-0.0.3.tar.gz` & `tmp/monas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monas-0.0.3.tar", last modified: Sun Apr 17 10:09:46 2022, max compression
+gzip compressed data, was "monas-0.1.0.tar", last modified: Fri Aug  4 01:51:56 2023, max compression
```

## Comparing `monas-0.0.3.tar` & `monas-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-17 10:09:38.609634 monas-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-04-17 10:09:38.609634 monas-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-04-17 10:09:38.613634 monas-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/bump.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/changed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/metadata/pep621.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/metadata/setupcfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4962 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/questions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-04-17 10:09:38.613634 monas-0.0.3/src/monas/vcs.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-04-17 10:09:38.613634 monas-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_add.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_changed.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_install.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_new.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-04-17 10:09:38.613634 monas-0.0.3/tests/cli/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-04-17 10:09:38.613634 monas-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-04-17 10:09:38.613634 monas-0.0.3/tests/test_utils.py
--rw-------   0 runner    (1001) docker     (121)     2704 2022-04-17 10:09:46.561667 monas-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-04 01:51:39.737038 monas-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1644 2023-08-04 01:51:39.737038 monas-0.1.0/README.md
+-rw-r--r--   0        0        0     1754 2023-08-04 01:51:56.373176 monas-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/__init__.py
+-rw-r--r--   0        0        0      113 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/__main__.py
+-rw-r--r--   0        0        0     1482 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/cli.py
+-rw-r--r--   0        0        0        0 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/__init__.py
+-rw-r--r--   0        0        0     1598 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/add.py
+-rw-r--r--   0        0        0     4996 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/bump.py
+-rw-r--r--   0        0        0      928 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/changed.py
+-rw-r--r--   0        0        0     2894 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/common.py
+-rw-r--r--   0        0        0     2069 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/init.py
+-rw-r--r--   0        0        0     2108 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/install.py
+-rw-r--r--   0        0        0      616 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/list.py
+-rw-r--r--   0        0        0     2426 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/new.py
+-rw-r--r--   0        0        0     3457 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/publish.py
+-rw-r--r--   0        0        0     1658 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/commands/remove.py
+-rw-r--r--   0        0        0     3165 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/config.py
+-rw-r--r--   0        0        0      250 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/metadata/__init__.py
+-rw-r--r--   0        0        0     1658 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/metadata/base.py
+-rw-r--r--   0        0        0     3762 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/metadata/pep621.py
+-rw-r--r--   0        0        0     4267 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/metadata/setupcfg.py
+-rw-r--r--   0        0        0     5435 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/project.py
+-rw-r--r--   0        0        0     2708 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/questions.py
+-rw-r--r--   0        0        0     2691 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/utils.py
+-rw-r--r--   0        0        0     2306 2023-08-04 01:51:39.737038 monas-0.1.0/src/monas/vcs.py
+-rw-r--r--   0        0        0       31 2023-08-04 01:51:39.737038 monas-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4742 2023-08-04 01:51:39.737038 monas-0.1.0/tests/cli/test_add.py
+-rw-r--r--   0        0        0      623 2023-08-04 01:51:39.737038 monas-0.1.0/tests/cli/test_bump.py
+-rw-r--r--   0        0        0      652 2023-08-04 01:51:39.737038 monas-0.1.0/tests/cli/test_changed.py
+-rw-r--r--   0        0        0      593 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_init.py
+-rw-r--r--   0        0        0     1255 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_install.py
+-rw-r--r--   0        0        0     1426 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_list.py
+-rw-r--r--   0        0        0     3462 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_new.py
+-rw-r--r--   0        0        0      526 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_publish.py
+-rw-r--r--   0        0        0      968 2023-08-04 01:51:39.741039 monas-0.1.0/tests/cli/test_remove.py
+-rw-r--r--   0        0        0     2030 2023-08-04 01:51:39.741039 monas-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      920 2023-08-04 01:51:39.741039 monas-0.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 monas-0.1.0/PKG-INFO
```

### Comparing `monas-0.0.3/LICENSE` & `monas-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/README.md` & `monas-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 **Monas** is a tool to manage multiple Python projects in a single repository, or the so called ["Monorepo"](https://en.wikipedia.org/wiki/Monorepo).
 It is mainly inspired by [Lerna](https://lerna.js.org/). In a monorepo, some dependencies are shared across packages while others are different. When you change the code of one of these shared dependencies, you may want to run the test suite across all dependant packages. Monas makes the workflow easier.
 
 <!--index end-->
 
 ## Installation
 
-**Monas** requires Python >=3.7.
+**Monas** requires Python >=3.8.
 
 It is recommended to install with `pipx`, if `pipx` haven't been installed yet, refer to the [pipx's docs](https://github.com/pipxproject/pipx)
 
 ```bash
 pipx install monas
 ```
```

### Comparing `monas-0.0.3/src/monas/cli.py` & `monas-0.1.0/src/monas/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
+import importlib.metadata
+
 import rich_click as click
 from rich import traceback
 
 from monas.commands.add import add
 from monas.commands.bump import bump
 from monas.commands.changed import changed
 from monas.commands.init import init
 from monas.commands.install import install
 from monas.commands.list import list_command
 from monas.commands.new import new
 from monas.commands.publish import publish
 from monas.commands.remove import remove
 from monas.utils import err_console
 
-__version__ = "0.0.3"
+__version__ = importlib.metadata.version(__package__)
 
 click.rich_click.USE_RICH_MARKUP = True
 traceback.install(console=err_console)
 
 
 class AliasGroup(click.RichGroup):
     def __init__(self, *args, **kwargs):
```

### Comparing `monas-0.0.3/src/monas/commands/add.py` & `monas-0.1.0/src/monas/commands/add.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     exclude: Collection[str],
     **kwargs: Any,
 ):
     """Add a dependency(PEP 508 string) to specified packages."""
     try:
         req = Requirement(dependency)
     except InvalidRequirement:
-        raise click.BadParameter(f"Invalid dependency {dependency}")
+        raise click.BadParameter(f"Invalid dependency {dependency}") from None
 
-    exclude = list(exclude) + [req.name]
+    exclude = [*list(exclude), req.name]
     packages = list(filter_packages(config, exclude=exclude, **kwargs))
     if not packages:
         info("[notice]No package is found[/]")
         return
 
     info(
         f"Adding dependency [succ]{dependency}[/] to "
```

### Comparing `monas-0.0.3/src/monas/commands/bump.py` & `monas-0.1.0/src/monas/commands/bump.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,15 @@
             part, tag = None, part
 
         version = bump_version(version, part, tag)
 
     info(f"Will bump version for [primary]{len(packages)}[/] package(s)")
     for pkg in packages:
         console.print(
-            f"  [primary]{pkg.path.name}[/] [succ]{pkg.version}[/] -> "
-            f"[succ]{version}[/]"
+            f"  [primary]{pkg.name}[/] [succ]{pkg.version}[/] -> " f"[succ]{version}[/]"
         )
     if not Confirm.ask("Continue?", console=console, default=True):
         ctx.abort()
     for pkg in packages:
         pkg.set_version(version)
     config.set_version(version)
     info("[succ]Version updated[/]")
```

### Comparing `monas-0.0.3/src/monas/commands/changed.py` & `monas-0.1.0/src/monas/commands/changed.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/src/monas/commands/common.py` & `monas-0.1.0/src/monas/commands/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,25 +62,25 @@
 
 def list_packages(
     packages: Iterable[PyPackage], *, long: bool = False, json: bool = False
 ) -> None:
     """List the packages."""
     if json:
         data = [
-            {"name": pkg.path.name, "version": pkg.version, "path": pkg.path.as_posix()}
+            {"name": pkg.name, "version": pkg.version, "path": pkg.path.as_posix()}
             for pkg in packages
         ]
         console.print_json(data=data)
         return
     table = Table.grid("Name", padding=(0, 1))
     if long:
         table.add_column("Version")
         table.add_column("Path", overflow="fold")
     for pkg in packages:
-        row = [f"[primary]{pkg.path.name}[/]"]
+        row = [f"[primary]{pkg.name}[/]"]
         if long:
             row.append(f"[succ]{pkg.version}[/]")
             row.append(f"[info]{pkg.path.relative_to(pkg.config.path).as_posix()}[/]")
         table.add_row(*row)
     console.print(table)
```

### Comparing `monas-0.0.3/src/monas/commands/init.py` & `monas-0.1.0/src/monas/commands/init.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/src/monas/commands/install.py` & `monas-0.1.0/src/monas/commands/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from concurrent.futures import Future
 from concurrent.futures import ThreadPoolExecutor as Pool
+from shlex import join as sh_join
 from typing import Any
 
 import rich_click as click
 
 from monas.commands.common import concurrency_option, filter_options, filter_packages
 from monas.config import Config, pass_config
 from monas.project import PyPackage
 from monas.utils import err_console as console
-from monas.utils import info, pip_install, sh_join
+from monas.utils import info, pip_install
 
 
 @click.command()
 @concurrency_option
 @click.option(
     "--root",
     is_flag=True,
@@ -41,20 +42,18 @@
             pip_install(config.root_venv, requirements)
         info("[succ]Installation done[/]")
         return
     errors: list[BaseException] = []
 
     def _on_complete(project: PyPackage, future: Future) -> None:
         if future.exception():
-            console.print(
-                f" [red bold]FAIL[/] {project.path.name} {future.exception()}"
-            )
+            console.print(f" [red bold]FAIL[/] {project.name} {future.exception()}")
             errors.append(future.exception())
         else:
-            console.print(f" [succ]SUCC[/] {project.path.name}")
+            console.print(f" [succ]SUCC[/] {project.name}")
 
     with console.status(
         f"Installing [primary]{package_count}[/] package(s)", spinner="point"
     ):
         with Pool(concurrency) as executor:
             for pkg in packages:
                 future = executor.submit(pkg.install)
```

### Comparing `monas-0.0.3/src/monas/commands/list.py` & `monas-0.1.0/src/monas/commands/list.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/src/monas/commands/new.py` & `monas-0.1.0/src/monas/commands/new.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import rich_click as click
 from click.decorators import pass_context
 from rich.prompt import Confirm
 
 from monas.config import Config, pass_config
 from monas.project import InputMetadata, PyPackage, get_metadata_class_for_backend
 from monas.questions import ask_for, package_questions
-from monas.utils import console, info
+from monas.utils import console, err_console, info
 
 
 @click.command()
 @click.argument("package", required=True)
 @click.argument("location", required=False)
 @pass_config
 @pass_context
@@ -24,15 +24,15 @@
 
     The package name must be locally unique and available on PyPI.
 
     If location isn't given, it defaults to the first location of `packages` config.
     """
     if location is None:
         location = config.package_paths[0]
-    if any(package == pkg.path.name for pkg in config.iter_packages()):
+    if any(package == pkg.name for pkg in config.iter_packages()):
         raise click.BadParameter(f"{package} already exists")
     package_path = Path(location, package).absolute()
     repo = config.get_repo()
 
     default_values = {
         "name": package,
         "version": config.version,
@@ -45,16 +45,21 @@
 
     inputs = InputMetadata(
         remote_repo=repo.get_remote_url(),
         **ask_for(package_questions, **default_values),
     )
     metadata_cls = get_metadata_class_for_backend(inputs.build_backend)
     metadata_contents = metadata_cls.create(inputs)
-    info(f"Writing pyproject.toml at [primary]{metadata_cls.filename}[/]:")
+    info(f"Writing metadata at [primary]{metadata_cls.filename}[/]:")
     console.print(metadata_contents.replace("[", "\\["))
+    if "setup.cfg" in inputs.build_backend:
+        err_console.print(
+            "[notice]The latest version of setuptools supports pyproject.toml "
+            "metadata, we highly recommend using it.[/]"
+        )
     if not Confirm.ask("Is this OK?", console=console, default=True):
         ctx.abort()
     package_path.mkdir(parents=True)
     with package_path.joinpath(metadata_cls.filename).open("w", encoding="utf-8") as f:
         f.write(metadata_contents)
     info("Creating project files")
     PyPackage.create(config, package_path, inputs)
```

### Comparing `monas-0.0.3/src/monas/commands/publish.py` & `monas-0.1.0/src/monas/commands/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         repo_args = ["--repository-url", repository]
         index = f"[link]{repository}[/]"
     else:
         repo_args = ["--repository", repository]
         index = f"[succ]{repository}[/]"
     info(f"The following packages are to be built and published to {index}:")
     for pkg in packages_to_publish:
-        console.print(f"  [primary]{pkg.path.name}[/] [succ]{pkg.version}[/]")
+        console.print(f"  [primary]{pkg.name}[/] [succ]{pkg.version}[/]")
     if not Confirm.ask("Continue?", console=console, default=True):
         ctx.abort()
     dist = config.path / "dist"
     if dist.exists():
         shutil.rmtree(dist)
     dist.mkdir()
     with err_console.status(
```

### Comparing `monas-0.0.3/src/monas/commands/remove.py` & `monas-0.1.0/src/monas/commands/remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     exclude: Collection[str],
     **kwargs: Any,
 ):
     """Remove a dependency from specified packages."""
     try:
         req = Requirement(dependency)
     except InvalidRequirement:
-        raise click.BadParameter(f"Invalid dependency {dependency}")
+        raise click.BadParameter(f"Invalid dependency {dependency}") from None
 
-    exclude = list(exclude) + [req.name]
+    exclude = [*list(exclude), req.name]
     packages = list(filter_packages(config, exclude=exclude, **kwargs))
     if not packages:
         info("[notice]No package is found[/]")
         return
 
     info(
         f"Removing dependency [succ]{req.name}[/] from "
```

### Comparing `monas-0.0.3/src/monas/config.py` & `monas-0.1.0/src/monas/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,11 +86,15 @@
     def iter_packages(self) -> Iterable[PyPackage]:
         """Iterate over the packages in the monorepo"""
         from monas.project import PyPackage
 
         for p in self.package_paths:
             for package in p.iterdir():
                 if package.is_dir():
-                    yield PyPackage(self, package)
+                    pypackage = PyPackage(self, package)
+                    if not pypackage.metadata.path.is_file():
+                        # directory has no python metadata file, ignore
+                        continue
+                    yield pypackage
 
 
 pass_config = click.make_pass_decorator(Config, ensure=True)
```

### Comparing `monas-0.0.3/src/monas/metadata/base.py` & `monas-0.1.0/src/monas/metadata/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,24 @@
 
     @abc.abstractproperty
     def version(self) -> str:
         """Get the project version"""
         pass
 
     @version.setter
+    @abc.abstractmethod
     def version(self, value: str) -> None:
         """Set the project version"""
         pass
 
+    @abc.abstractproperty
+    def package_name(self) -> str:
+        """Get the project version"""
+        pass
+
     @abc.abstractclassmethod
     def create(cls, inputs: InputMetadata) -> str:
         """Create the project metadata and return the content"""
         pass
 
     @abc.abstractmethod
     def add_dependency(self, dependency: str) -> None:
```

### Comparing `monas-0.0.3/src/monas/metadata/pep621.py` & `monas-0.1.0/src/monas/metadata/pep621.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     def _write(self) -> None:
         TOMLFile(self.path).write(self._data)
 
     @property
     def version(self) -> str:
         return self._data["project"]["version"]
 
+    @property
+    def package_name(self) -> str:
+        return self._data["project"]["name"]
+
     @version.setter
     def version(self, value: str) -> None:
         self._data["project"]["version"] = value
         self._write()
 
     @classmethod
     def create(cls, inputs: InputMetadata) -> str:
```

### Comparing `monas-0.0.3/src/monas/metadata/setupcfg.py` & `monas-0.1.0/src/monas/metadata/setupcfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         with open(self.path, "w", encoding="utf-8") as f:
             self._parser.write(f)
 
     @property
     def version(self) -> str:
         return self._parser.get("metadata", "version")
 
+    @property
+    def package_name(self) -> str:
+        return self._parser.get("metadata", "name")
+
     @version.setter
     def version(self, value: str) -> None:
         self._parser["metadata"]["version"] = value
         self._write()
 
     @classmethod
     def create(cls, inputs: InputMetadata) -> str:
```

### Comparing `monas-0.0.3/src/monas/project.py` & `monas-0.1.0/src/monas/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 import textwrap
 from pathlib import Path
+from shlex import join as sh_join
 from typing import Type, cast
 
 import tomlkit
 from packaging.utils import canonicalize_name
 from tomlkit.toml_file import TOMLFile
 
 from monas.config import Config
 from monas.metadata import ALL_METADATA_CLASSES, Metadata
 from monas.questions import InputMetadata
-from monas.utils import pip_install, sh_join
+from monas.utils import pip_install
 
 BUILD_BACKENDS = {
     "setuptools": {
         "requires": ["setuptools>=61", "wheel"],
         "build-backend": "setuptools.build_meta",
     },
-    "pdm": {"requires": ["pdm-pep517"], "build-backend": "pdm.pep517.api"},
+    "pdm": {"requires": ["pdm-backend"], "build-backend": "pdm.backend"},
     "flit": {"requires": ["flit_core>=3.2,<4"], "build-backend": "flit_core.buildapi"},
     "hatch": {"requires": ["hatchling>=0.22.0"], "build-backend": "hatchling.build"},
 }
 
 FILE_TEMPLATES = {
     "README.md": textwrap.dedent(
         """\
@@ -55,15 +56,15 @@
 
 
 def get_build_system_for_backend(name: str) -> dict:
     name = name.split("(")[0]
     return BUILD_BACKENDS[name]
 
 
-def get_metadata_class_for_backend(name: str) -> Type[Metadata]:
+def get_metadata_class_for_backend(name: str) -> type[Metadata]:
     backend, _, extra = name.partition("(")
     if backend == "setuptools":
         class_name = "pep621" if extra.rstrip(")") == "pyproject.toml" else "setupcfg"
     else:
         class_name = "pep621"
     result = next((cls for cls in ALL_METADATA_CLASSES if cls.name == class_name), None)
     if result is None:
@@ -88,17 +89,22 @@
             (cls for cls in ALL_METADATA_CLASSES if cls.match(pyproject_data)), None
         )
         if result is None:
             raise ValueError("Can't determine a metadata type from the pyproject.toml")
         return cast(Type[Metadata], result)(self.path)
 
     @property
+    def name(self) -> str:
+        """Get the project name"""
+        return self.metadata.package_name
+
+    @property
     def canonical_name(self) -> str:
         """Get the project name"""
-        return canonicalize_name(self.path.name)
+        return canonicalize_name(self.name)
 
     @property
     def version(self) -> str:
         """Get the project version"""
         return self.metadata.version
 
     def set_version(self, version: str) -> None:
@@ -145,15 +151,22 @@
         Args:
             dependency: A canonicalized requirement name
         """
         self.metadata.remove_dependency(dependency)
 
     def install(self) -> None:
         """Bootstrap the package and link depending packages in the monorepo"""
-        dependency_names = self.metadata.get_dependency_names()
-        packages = [
-            pkg
-            for pkg in self.config.iter_packages()
-            if pkg.canonical_name in dependency_names
-        ] + [self]
-        requirements = [sh_join(["-e", pkg.path.as_posix()]) for pkg in packages]
+        local_dependencies = [*self.get_local_dependencies(), self]
+        requirements = [
+            sh_join(["-e", pkg.path.as_posix()]) for pkg in local_dependencies
+        ]
         pip_install(self.path / ".venv", requirements)
+
+    def get_local_dependencies(self) -> list[PyPackage]:
+        """Return list of local dependencies."""
+        dependency_names = self.metadata.get_dependency_names()
+        local_dependencies = []
+        local_packages = list(self.config.iter_packages())
+        for pkg in local_packages:
+            if pkg.canonical_name in dependency_names:
+                local_dependencies += [*pkg.get_local_dependencies(), pkg]
+        return local_dependencies
```

### Comparing `monas-0.0.3/src/monas/questions.py` & `monas-0.1.0/src/monas/questions.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,25 +49,25 @@
     "name": Question("package name:"),
     "version": Question("version:", default="0.0.0"),
     "description": Question("description:", default=""),
     "license_expr": Question("license:", default="MIT", instruction="SPDX identifier"),
     "author": Question("author", ""),
     "author_email": Question("author email:", ""),
     "homepage": Question("homepage:", ""),
-    "requires_python": Question("requires_python:", default=">=3.7"),
+    "requires_python": Question("requires_python:", default=">=3.8"),
     "build_backend": Question(
         "Build backend:",
         choices=[
-            "setuptools(setup.cfg)",
-            "setuptools(pyprojec.toml)",
             "pdm",
             "flit",
             "hatch",
+            "setuptools(pyproject.toml)",
+            "setuptools(setup.cfg)",
         ],
-        default="setuptools(setup.cfg)",
+        default="pdm",
     ),
 }
 
 
 def ask_for(questions: dict[str, Question], **kwargs: str) -> dict[str, str]:
     """Ask questions and return answers.
```

### Comparing `monas-0.0.3/src/monas/utils.py` & `monas-0.1.0/src/monas/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,22 +29,25 @@
 def info(msg: str) -> None:
     """Print info message."""
     prefix = f"[info]{PROJECT_NAME}[/] "
     err_console.print(prefix + msg, highlight=False)
 
 
 def run_command(
-    cmd: list[str], cwd: str = None, env: dict[str, str] | None = None, **kwargs: Any
+    cmd: list[str],
+    cwd: str | None = None,
+    env: dict[str, str] | None = None,
+    **kwargs: Any,
 ) -> subprocess.CompletedProcess:
     """Run command in subprocess"""
     try:
         return subprocess.run(cmd, cwd=cwd, env=env, check=True, **kwargs)
     except subprocess.CalledProcessError:
-        err_console.print("[danger]Error running command[/] {}. ")
-        raise click.Abort()
+        err_console.print(f"[danger]Error running command[/] {cmd}. ")
+        raise click.Abort() from None
 
 
 def get_preferred_python_version() -> str:
     """Get preferred python version"""
     major, minor = sys.version_info[:2]
     return f"{major}.{minor}"
 
@@ -54,15 +57,15 @@
     from virtualenv import cli_run
 
     if path.exists():
         return
     info(f"Creating virtualenv: [primary]{path}[/]")
     args = [str(path)]
     if python_version:
-        args = ["-p", python_version] + args
+        args = ["-p", python_version, *args]
     cli_run(args, setup_logging=True)
 
 
 def pip_install(venv_path: Path, requirements: Iterable[str]) -> None:
     """Install the given requirements into the venv"""
     ensure_virtualenv(venv_path)
     if os.name == "nt":
@@ -93,17 +96,7 @@
 def is_relative_to(path: Path, parent: Path) -> bool:
     """Check if path is relative path to the parent"""
     try:
         path.absolute().relative_to(parent)
         return True
     except ValueError:
         return False
-
-
-if sys.version_info >= (3, 8):
-    from shlex import join as sh_join
-else:
-    from shlex import quote as quote
-
-    def sh_join(split_command: Iterable[str]) -> str:
-        """Return a shell-escaped string from *split_command*."""
-        return " ".join(quote(arg) for arg in split_command)
```

### Comparing `monas-0.0.3/src/monas/vcs.py` & `monas-0.1.0/src/monas/vcs.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_add.py` & `monas-0.1.0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_bump.py` & `monas-0.1.0/tests/cli/test_bump.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_changed.py` & `monas-0.1.0/tests/cli/test_changed.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_init.py` & `monas-0.1.0/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_install.py` & `monas-0.1.0/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_list.py` & `monas-0.1.0/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_new.py` & `monas-0.1.0/tests/cli/test_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 [build-system]
 requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 """
 
 pdm_backend = """
 [build-system]
-requires = ["pdm-pep517"]
-build-backend = "pdm.pep517.api"
+requires = ["pdm-backend"]
+build-backend = "pdm.backend"
 """
 
 hatch_backend = """
 [build-system]
 requires = ["hatchling>=0.22.0"]
 build-backend = "hatchling.build"
 """
```

### Comparing `monas-0.0.3/tests/cli/test_publish.py` & `monas-0.1.0/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/cli/test_remove.py` & `monas-0.1.0/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/tests/conftest.py` & `monas-0.1.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,30 +42,33 @@
 def python_version():
     return get_preferred_python_version()
 
 
 @pytest.fixture()
 def test_project(cli_run, project):
     run_command(["git", "init"], cwd=str(project))
-    with mock.patch(
-        "monas.commands.new.ask_for",
-        side_effect=[
-            {
-                "name": "foo",
-                "version": "0.0.0",
-                "author": "John",
-                "author_email": "john@doe.me",
-                "description": "Test Project",
-                "license_expr": "MIT",
-                "homepage": "https://example.org",
-                "requires_python": ">=3.7",
-                "build_backend": backend,
-            }
-            for backend in ["setuptools(setup.cfg)", "pdm", "flit"]
-        ],
-    ):
-        cli_run(["new", "foo"], cwd=project, input="\n")
-        cli_run(["new", "bar"], cwd=project, input="\n")
-        cli_run(["new", "foo-more", "extras"], cwd=project, input="\n")
+    projects = (
+        (("new", "foo"), "setuptools(setup.cfg)"),
+        (("new", "bar"), "pdm"),
+        (("new", "foo-more", "extras"), "flit"),
+    )
+    for cli_args, backend in projects:
+        with mock.patch(
+            "monas.commands.new.ask_for",
+            side_effect=[
+                {
+                    "name": cli_args[1],
+                    "version": "0.0.0",
+                    "author": "John",
+                    "author_email": "john@doe.me",
+                    "description": "Test Project",
+                    "license_expr": "MIT",
+                    "homepage": "https://example.org",
+                    "requires_python": ">=3.7",
+                    "build_backend": backend,
+                }
+            ],
+        ):
+            cli_run(cli_args, cwd=project, input="\n")
     run_command(["git", "add", "."], cwd=str(project))
     run_command(["git", "commit", "-m", "Initial commit"], cwd=str(project))
     return project
```

### Comparing `monas-0.0.3/tests/test_utils.py` & `monas-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `monas-0.0.3/PKG-INFO` & `monas-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 Metadata-Version: 2.1
 Name: monas
-Version: 0.0.3
+Version: 0.1.0
 Summary: Python monorepo made easy
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Homepage, https://github.com/frostming/monas
+Classifier: Programming Language :: Python :: 3.10
 Project-URL: Repository, https://github.com/frostming/monas
+Project-URL: Homepage, https://github.com/frostming/monas
+Requires-Python: >=3.8
+Requires-Dist: gitpython>=3
+Requires-Dist: click>=7
+Requires-Dist: packaging>=20
+Requires-Dist: questionary
+Requires-Dist: rich-click>=1.3.0
+Requires-Dist: twine
+Requires-Dist: tomlkit>=0.8
+Requires-Dist: virtualenv>=20.1.0
+Requires-Dist: parver
 Description-Content-Type: text/markdown
-Description: # Monas
-        
-        <!--index start-->
-        
-        [![Tests](https://github.com/frostming/monas/workflows/Tests/badge.svg)](https://github.com/frostming/monas/actions?query=workflow%3Aci)
-        [![pypi version](https://img.shields.io/pypi/v/monas.svg)](https://pypi.org/project/monas/)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-        
-        Python monorepo made easy.
-        
-        🚧 **[WIP]** This project still in a rapid development and the behaviors may change. 🚧
-        
-        ➡️ [Example Repository](https://github.com/frostming/monas-example-repo)
-        
-        ## About this project
-        
-        **Monas** is a tool to manage multiple Python projects in a single repository, or the so called ["Monorepo"](https://en.wikipedia.org/wiki/Monorepo).
-        It is mainly inspired by [Lerna](https://lerna.js.org/). In a monorepo, some dependencies are shared across packages while others are different. When you change the code of one of these shared dependencies, you may want to run the test suite across all dependant packages. Monas makes the workflow easier.
-        
-        <!--index end-->
-        
-        ## Installation
-        
-        **Monas** requires Python >=3.7.
-        
-        It is recommended to install with `pipx`, if `pipx` haven't been installed yet, refer to the [pipx's docs](https://github.com/pipxproject/pipx)
-        
-        ```bash
-        pipx install monas
-        ```
-        
-        Alternatively, install with `pip` to the user site:
-        
-        ```bash
-        python -m pip install --user monas
-        ```
-        
-        ## To-do
-        
-        - [x] Documentation
-        - [x] Tests
-        - [x] `setup.cfg` support
-        - [ ] (Possible) Poetry backend support
-        - [ ] `src` package layout
-        
-        ## License
-        
-        MIT.
 
+# Monas
+
+<!--index start-->
+
+[![Tests](https://github.com/frostming/monas/workflows/Tests/badge.svg)](https://github.com/frostming/monas/actions?query=workflow%3Aci)
+[![pypi version](https://img.shields.io/pypi/v/monas.svg)](https://pypi.org/project/monas/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+
+Python monorepo made easy.
+
+🚧 **[WIP]** This project still in a rapid development and the behaviors may change. 🚧
+
+➡️ [Example Repository](https://github.com/frostming/monas-example-repo)
+
+## About this project
+
+**Monas** is a tool to manage multiple Python projects in a single repository, or the so called ["Monorepo"](https://en.wikipedia.org/wiki/Monorepo).
+It is mainly inspired by [Lerna](https://lerna.js.org/). In a monorepo, some dependencies are shared across packages while others are different. When you change the code of one of these shared dependencies, you may want to run the test suite across all dependant packages. Monas makes the workflow easier.
+
+<!--index end-->
+
+## Installation
+
+**Monas** requires Python >=3.8.
+
+It is recommended to install with `pipx`, if `pipx` haven't been installed yet, refer to the [pipx's docs](https://github.com/pipxproject/pipx)
+
+```bash
+pipx install monas
+```
+
+Alternatively, install with `pip` to the user site:
+
+```bash
+python -m pip install --user monas
+```
+
+## To-do
+
+- [x] Documentation
+- [x] Tests
+- [x] `setup.cfg` support
+- [ ] (Possible) Poetry backend support
+- [ ] `src` package layout
+
+## License
+
+MIT.
```

