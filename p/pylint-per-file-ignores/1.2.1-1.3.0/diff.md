# Comparing `tmp/pylint_per_file_ignores-1.2.1.tar.gz` & `tmp/pylint_per_file_ignores-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_per_file_ignores-1.2.1.tar", max compression
+gzip compressed data, was "pylint_per_file_ignores-1.3.0.tar", max compression
```

## Comparing `pylint_per_file_ignores-1.2.1.tar` & `pylint_per_file_ignores-1.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     8823 2023-05-15 17:46:33.388506 pylint_per_file_ignores-1.2.1/pylint_per_file_ignores/__init__.py
--rw-r--r--   0        0        0      811 2023-05-15 17:47:11.778774 pylint_per_file_ignores-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      788 2023-05-15 17:46:33.388506 pylint_per_file_ignores-1.2.1/readme.md
--rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 pylint_per_file_ignores-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1217 2023-08-04 12:05:37.639405 pylint_per_file_ignores-1.3.0/README.md
+-rw-r--r--   0        0        0     9775 2023-08-04 12:05:37.643405 pylint_per_file_ignores-1.3.0/pylint_per_file_ignores/__init__.py
+-rw-r--r--   0        0        0      788 2023-08-04 12:06:08.355764 pylint_per_file_ignores-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 pylint_per_file_ignores-1.3.0/PKG-INFO
```

### Comparing `pylint_per_file_ignores-1.2.1/pylint_per_file_ignores/__init__.py` & `pylint_per_file_ignores-1.3.0/pylint_per_file_ignores/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
 from pathlib import Path
 from typing import List, Optional
 
+from pylint import utils
+from pylint.checkers import BaseChecker
 from pylint.exceptions import UnknownMessageError
 from pylint.lint import PyLinter
 
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib  # type: ignore
@@ -15,16 +17,14 @@
     """Search upstream for a pyproject.toml file."""
     for directory in Path(src).parents:
         pyproject = directory / "pyproject.toml"
 
         if pyproject.is_file():
             return pyproject
 
-    raise ValueError("Could not find pyproject.toml file in the project.")
-
 
 def get_checker_by_msg(linter, msg):
     for checker in linter.get_checkers():
         for key, value in checker.msgs.items():
             if msg in [key, value[1]]:
                 return checker
 
@@ -223,18 +223,49 @@
         return bool(
             re.search(
                 self.file_string, Path(self.linter.current_file).as_posix(), re.VERBOSE
             )
         )
 
 
-def register(linter: "PyLinter") -> None:
-    """This required method auto registers the checker during initialization.
-
-    :param linter: The linter to register the checker to.
-    """
-    content = tomllib.load(find_pyproject(linter.current_file).open("rb"))
-    ignores = {**content["tool"]["pylint-per-file-ignores"]}
+class PerFileIgnoresChecker(BaseChecker):
+    # Just to register custom config option
+    options = (
+        (
+            "per-file-ignores",
+            {
+                "default": "",
+                "type": "string",
+                "metavar": "<str>",
+                "help": "Newline-separated list of ignores",
+            },
+        ),
+    )
+
+
+def register(linter: PyLinter) -> None:
+    linter.register_checker(PerFileIgnoresChecker(linter))
+
+
+def load_configuration(linter: PyLinter) -> None:
+    # Loading configuration from native pylint configuration mechanism
+    if not isinstance(linter.config.per_file_ignores, dict):
+        linter.config.per_file_ignores = dict(
+            config_item.split(":")
+            for config_item in utils._splitstrip(
+                linter.config.per_file_ignores, sep="\n"
+            )
+        )
 
-    for file_path, rules in ignores.items():
+    for file_path, rules in linter.config.per_file_ignores.items():
         for rule in rules.split(","):
             disable_message(linter, rule.strip(), IsFile(file_path, linter))
+
+    # Loading custom pyproject.toml
+    pyproject_file = find_pyproject(linter.current_file)
+    if pyproject_file:
+        content = tomllib.load(pyproject_file).open("rb")
+        ignores = {**content["tool"]["pylint-per-file-ignores"]}
+
+        for file_path, rules in ignores.items():
+            for rule in rules.split(","):
+                disable_message(linter, rule.strip(), IsFile(file_path, linter))
```

### Comparing `pylint_per_file_ignores-1.2.1/pyproject.toml` & `pylint_per_file_ignores-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 quiet = true
 
 [tool.poetry]
 authors = ["Christopher Pickering <christopher@going.bg>"]
 description = "A pylint plugin to ignore error codes per file."
 license = "MIT"
 name = "pylint-per-file-ignores"
-readme = "readme.md"
+readme = "README.md"
 repository = "https://github.com/christopherpickering/pylint-per-file-ignores.git"
-version = "1.2.1"
+version = "1.3.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 tomli = {version = "^2.0.1", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
-flake8 = "6.0.0"
 isort = "^5.10.1"
-pylint = "^2.15.8"
+ruff = "^0.0.282"
 tox = "^4.0.8"
 
-[tool.pylint.messages_control]
-disable = "C0116,C0301,C0114,R0901,C0115,R0903,W0201,C0103"
+[tool.ruff]
+ignore = ["B009", "B010"]
+select = ["E", "F", "I", "S", "T20", "PL", "B"]
```

### Comparing `pylint_per_file_ignores-1.2.1/PKG-INFO` & `pylint_per_file_ignores-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-per-file-ignores
-Version: 1.2.1
+Version: 1.3.0
 Summary: A pylint plugin to ignore error codes per file.
 Home-page: https://github.com/christopherpickering/pylint-per-file-ignores.git
 License: MIT
 Author: Christopher Pickering
 Author-email: christopher@going.bg
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,30 +28,55 @@
 
 # w/ pip
 pip install pylint-per-file-ignores
 ```
 
 ## Add to Pylint Settings
 
-Edit your `pyproject.toml`:
-
-```
+```toml
 [tool.pylint.MASTER]
 load-plugins=[
     "pylint_per_file_ignores",
     ...
 ]
 ```
 
 
 ## Usage
 
-Add a section to your `pyproject.toml` with the patterns and codes you would like to ignore.
+Add list of patterns and codes you would like to ignore.
+
+### Using native pylint settings
+
+Section "MESSAGES CONTROL". Examples:
+
+```ini
+# setup.cfg
+
+[pylint.MESSAGES CONTROL]
+per-file-ignores =
+  /folder_1/:missing-function-docstring,W0621,W0240,C0115
+  file.py:C0116,E0001
+```
+
+```toml
+# pyproject.toml
 
+[tool.pylint.'MESSAGES CONTROL']
+per-file-ignores = [
+    "/folder_1/:missing-function-docstring,W0621,W0240,C0115",
+    "file.py:C0116,E0001"
+]
 ```
+
+### Using custom `pyproject.toml` section
+
+For backwards compatibility only. Example:
+
+```toml
 [tool.pylint-per-file-ignores]
 "/folder_1/"="missing-function-docstring,W0621,W0240,C0115"
 "file.py"="C0116,E0001"
 ```
 
 ## Thanks
```

