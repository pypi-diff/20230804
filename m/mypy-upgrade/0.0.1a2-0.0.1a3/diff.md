# Comparing `tmp/mypy_upgrade-0.0.1a2.tar.gz` & `tmp/mypy_upgrade-0.0.1a3.tar.gz`

## Comparing `mypy_upgrade-0.0.1a2.tar` & `mypy_upgrade-0.0.1a3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__main__.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/py.typed
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/.gitignore
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/AUTHORS.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/LICENSE.txt
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/README.md
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__main__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/cli.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/editing.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/filter.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/py.typed
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/silence.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/utils.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/AUTHORS.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/LICENSE.txt
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/README.md
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/PKG-INFO
```

### Comparing `mypy_upgrade-0.0.1a2/.gitignore` & `mypy_upgrade-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a2/LICENSE.txt` & `mypy_upgrade-0.0.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a2/PKG-INFO` & `mypy_upgrade-0.0.1a3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-upgrade
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: automatic error suppression for mypy
 Project-URL: Documentation, https://github.com/ugognw/mypy-upgrade#readme
 Project-URL: Issues, https://github.com/ugognw/mypy-upgrade/issues
 Project-URL: Source, https://github.com/ugognw/mypy-upgrade
 Author-email: Ugochukwu Nwosu <ugognw@gmail.com>
 License-Expression: MIT
 License-File: AUTHORS.md
@@ -14,88 +14,110 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
+Requires-Dist: typing-extensions; python_version < '3.8'
 Description-Content-Type: text/markdown
 
-# mypy-upgrade
+# `mypy-upgrade`
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mypy-upgrade.svg)](https://pypi.org/project/mypy-upgrade)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-upgrade.svg)](https://pypi.org/project/mypy-upgrade)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
 -----
 
 **Table of Contents**
 
+- [What is `mypy-upgrade`?](#what-is-mypy-upgrade)
+- [Features](#features)
 - [Basic Usage](#basic-usage)
 - [Command-Line Options](#command-line-options)
 - [Quick Start](#quick-start)
+- [Known Bugs](#known-bugs)
+- [Similar Projects](#similar-projects)
+
+## What is `mypy-upgrade`?
 
 `mypy-upgrade` is a command-line utility that provides automatic error
-suppression for `mypy` (analogous to `pyre-upgrade`).
+suppression for [`mypy`](http://mypy.readthedocs.io/) (analogous to [`pyre-upgrade`](https://pyre-check.org/docs/types-in-python/#upgrade) and [`pylint-silent`](https://github.com/udifuchs/pylint-silent/)).
 
-Given a type checking report from [mypy](http://mypy.readthedocs.io/),
+Given a type checking report from `mypy`,
 `mypy-upgrade` will silence the listed errors using error suppression
 comments. For example, with the following output from mypy:
 
-    ase/utils/plotting.py:13: error: Incompatible default for argument "filename" (default has type "None", argument has type "str") [assignment]
+    package/subpackage/module.py:13: error: Incompatible default for argument "filename" (default has type "None", argument has type "str") [assignment]
 
 `mypy-upgrade` will place a `# type: ignore[assignment]` comment at the
-end of line 13 in `ase/utils/plotting.py`. If error codes are not present in
-the `mypy` report (e.g., the `hide-error-codes` flag is set when `mypy` was
-invoked), then a non-specific `# type: ignore` comment will be added instead.
+end of line 13 in `package/subpackage/module.py`. If error codes are not
+present in the `mypy` report (e.g., the `hide-error-codes` flag is set when
+`mypy` was invoked), then a non-specific `# type: ignore` comment will be
+added instead.
 
 > :warning: **Warning:** `mypy-check` **must** be run in the same directory
-> that `mypy` was run.*
+> that `mypy` was run.
+
+## Features
+
+* Removal of unused `type: ignore` comments
+
+* Optional inclusion of `mypy` error description messages
+
+* Support for suppressing multiple mypy errors per-line
+
+* Preservation of existing in-line comments
+
+* Replacement of blanket `type: ignore` comments with error code-specific
+comments
 
 ## Basic Usage
 
 There are two idioms for invocation. To silence all errors in a package, one
 can:
 
-1. invoke `mypy-upgrade` in a "Pyre-like" fashion
+1. pipe `mypy`'s output directly to `mypy-upgrade`
 
-        mypy -p my_package | mypy-upgrade -p my_package
+        mypy --strict -p my_package | mypy-upgrade
 
 2. create a `mypy` type checking report text file
 
-        mypy -p my_package > mypy_report.txt
+        mypy --strict -p my_package > mypy_report.txt
 
     and then pass the file to `mypy-upgrade`
 
-        mypy-upgrade --report mypy_report.txt -p my_package
+        mypy-upgrade --report mypy_report.txt
 
 > :memo: **Note:** To ensure desired behaviour, packages and modules must be
 passed using their fully qualified names (e.g., `my_package.my_module`).
 
 ## Command-Line Options
 
 You may want to include the error descriptions provided by `mypy` in the
-suppression comments so that you can fix them later.
+suppression comments so that you can fix them later. You can do so using
+the `-d` (or `--with-descriptions`) option
 
     mypy-upgrade --report mypy_report.txt -d -p MY_PACKAGE
 
-Files and directories can also be passed as positional arguments:
+To selectively silence errors in packages and modules, use the `-p`
+(`--package`) and `-m` (`--module`) options, respectively:
 
-    mypy-upgrade --report mypy_report.txt path/to/my_package/ path/to/another_package/
+Similarly, to selectively silence errors in files and directories,
+pass them in as positional arguments:
 
-    mypy-upgrade --report mypy_report.txt path/to/a/module.py
+    mypy-upgrade --report mypy_report.txt path/to/my_package/ path/to/a/module.py
 
 For a full list of all options and their descriptions, run
 
     mypy-upgrade --help
 
 ## Quick Start
 
@@ -105,7 +127,35 @@
 
 If you want to run the latest version of the code, you can install from the
 repo directly:
 
     python3 -m pip install -U git+https://github.com/ugognw/mypy-upgrade.git
     # or if you don't have 'git' installed
     python3 -m pip install -U https://github.com/ugognw/mypy-upgrade/tree/development
+
+## Known Bugs
+
+This utility is unable to silence mypy errors which occur on lines ending in
+line continuation characters since any non-whitespace following such a
+character is a syntax error. Pre-formatting your code with a PEP8 adherent
+formatter (e.g., [`black`](http://black.readthedocs.io)) to replace such lines with parentheses
+is recommended.
+
+## Similar Projects
+
+If this doesn't fit your use-case, maybe one of these other projects will!
+
+* [`geo7/mypy_clean_slate`](https://github.com/geo7/mypy_clean_slate/tree/main): `mypy` reports are generated internally in `--strict` mode; includes
+support for suppressing multiple errors on a single line; an inspiration for
+much of `mypy-upgrade`'s implementation
+
+* [`whtsky/mypy-silent`](https://github.com/whtsky/mypy-silent/tree/master):
+relies solely on [`typer`](https://typer.tiangolo.com) + the standard
+library; includes support for removing unused `type: ignore` comments but no
+support for suppressing multiple errors on a single line; another inspiration
+for much of `mypy-upgrade`'s implementation
+
+* [`patrick91/mypy-silent`](https://github.com/patrick91/mypy-silent/tree/feature/multiple-errors): a fork of `whtsky/mypy-silent` with support for
+suppressing multiple errors on a single line (on the `feature/multiple-errors` branch)
+
+* [`uptickmetachu/mypy-silent`](https://github.com/uptickmetachu/mypy-silent/tree/main): a fork of `whtsky/mypy-silent` with support for suppressing
+multiple errors on a single line
```

