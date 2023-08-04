# Comparing `tmp/jsonator-0.1.6.tar.gz` & `tmp/jsonator-0.1.7.tar.gz`

## Comparing `jsonator-0.1.6.tar` & `jsonator-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/__main__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/enum.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/jsonator.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/output.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/report.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.6/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.6/LICENSE
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 jsonator-0.1.6/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jsonator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jsonator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/__main__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/enum.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/output.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/report.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 jsonator-0.1.7/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jsonator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 jsonator-0.1.7/PKG-INFO
```

### Comparing `jsonator-0.1.6/jsonator/__init__.py` & `jsonator-0.1.7/jsonator/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,30 +35,69 @@
         help="Show colored diff. Only applies when `--diff` is given.",
     )
     arg_parser.add_argument(
         "--sort-keys",
         action="store_true",
         help="Sort the output of dictionaries alphabetically by key.",
     )
+    group = arg_parser.add_mutually_exclusive_group()
+    group.add_argument(
+        "--indent",
+        type=int,
+        help="Separate items with newlines and use this number of spaces for indentation.",
+    )
+    group.add_argument(
+        "--tab",
+        action="store_true",
+        help="Separate items with newlines and use tabs for indentation.",
+    )
+    group.add_argument(
+        "--no-indent", action="store_true", help="Separate items with spaces rather than newlines."
+    )
+    group.add_argument(
+        "--compact", action="store_true", help="Suppress all whitespace separation (most compact)."
+    )
 
     args = arg_parser.parse_args()
 
     if not args.path.exists():
         return ReturnCode.FILE_NOT_FOUND.value
 
     if args.sort_keys and sys.version_info < (3, 5):
         print("The `--sort-keys` option is only available on Python 3.5 and above", file=sys.stderr)
         return ReturnCode.INTERNAL_ERROR.value
 
+    if (args.indent or args.tab or args.no_indent or args.tab) and sys.version_info < (3, 9):
+        print(
+            "`--indent`, `--tab`, `--no-indent`, `--compact` options "
+            "are only available on Python 3.9 and above",
+            file=sys.stderr,
+        )
+        return ReturnCode.INTERNAL_ERROR.value
+
     report = Report(args.check, args.diff)
 
     if args.path.is_dir():
         pattern = "**/*.json" if args.recursive else "*.json"
-
-        for json_file in args.path.glob(pattern):
-            format_json_file(json_file, report, args.check, args.diff, args.color, args.sort_keys)
+        files_to_scan = list(args.path.glob(pattern))
 
     else:
-        format_json_file(args.path, report, args.check, args.diff, args.color, args.sort_keys)
+        files_to_scan = [
+            args.path,
+        ]
+
+    for file_to_scan in files_to_scan:
+        format_json_file(
+            file_to_scan,
+            report,
+            args.check,
+            args.diff,
+            args.color,
+            args.sort_keys,
+            args.indent,
+            args.tab,
+            args.no_indent,
+            args.compact,
+        )
 
     print(report)
     return report.status
```

### Comparing `jsonator-0.1.6/jsonator/jsonator.py` & `jsonator-0.1.7/jsonator/jsonator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import filecmp
 import os
 import random
 import string
 import sys
 from pathlib import Path
 from tempfile import gettempdir
+from typing import Optional
 
 from jsonator import output
 from jsonator.report import Report
 
 INTERPRETER = Path(sys.executable).stem
 FILES_ENCODING = "utf-8"
 
@@ -29,25 +30,42 @@
     while temp_file.exists():
         temp_file = temp_dir / random_str()
 
     return temp_file
 
 
 def format_json_file(  # pylint: disable=too-many-arguments
-    json_file: Path, report: Report, check: bool, diff: bool, color: bool, sort_keys: bool
+    json_file: Path,
+    report: Report,
+    check: bool,
+    diff: bool,
+    color: bool,
+    sort_keys: bool,
+    indent: Optional[int],
+    tab: bool,
+    no_indent: bool,
+    compact: bool,
 ) -> None:
     """
     This function formats the file in JSON format.
     It uses the json.tool module, built into Python, to create a readable JSON format.
     """
     tmp_file = make_temp_file()
 
     cmd = [INTERPRETER, "-m", "json.tool", f'"{json_file}"', tmp_file]
     if sort_keys:
         cmd.append("--sort-keys")
+    if indent is not None:
+        cmd.append(f"--indent {indent}")
+    if tab:
+        cmd.append("--tab")
+    if no_indent:
+        cmd.append("--no-indent")
+    if compact:
+        cmd.append("--compact")
 
     os.system(" ".join([str(command) for command in cmd]))
 
     try:
         is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
     except FileNotFoundError:
         report.failed(json_file, "Internal error")
```

### Comparing `jsonator-0.1.6/jsonator/output.py` & `jsonator-0.1.7/jsonator/output.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.6/jsonator/report.py` & `jsonator-0.1.7/jsonator/report.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.6/LICENSE` & `jsonator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.6/README.md` & `jsonator-0.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -26,15 +26,25 @@
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
 * --diff: Don't write the files back, just output a diff for each file on stdout.
 
 * --color: Show colored diff. Only applies when `--diff` is given.
 
-* --sort-keys: Sort the output of dictionaries alphabetically by key.
+* --sort-keys: Sort the output of dictionaries alphabetically by key. *Available on Python 3.5+.*
+
+* --indent: Separate items with newlines and use this number of spaces for indentation.
+
+* --tab: Separate items with newlines and use tabs for indentation.
+
+* --no-indent: Separate items with spaces rather than newlines.
+
+* --compact: Suppress all whitespace separation (most compact).
+
+  *--indent, --tab, --no-indent, --compact — mutually exclusive options for whitespace control. Available on Python 3.9+.*
 
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsonator-0.1.6/pyproject.toml` & `jsonator-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=0.25.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonator"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Sergey Fomin", email="sergiusnn@gmail.com" },
 ]
 description = "JSON formatting and validating tool"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
@@ -33,12 +33,12 @@
 
 [project.scripts]
 jsonator = "jsonator:main"
 
 [tool.poetry]
 readme = "README.md"
 name = "jsonator"
-version = "0.1.6"
+version = "0.1.7"
 description = "JSON formatting and validating tool"
 authors = [
   "Sergey Fomin <sergiusnn@gmail.com>",
 ]
```

### Comparing `jsonator-0.1.6/PKG-INFO` & `jsonator-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.6
+Version: 0.1.7
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
@@ -38,15 +38,25 @@
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
 * --diff: Don't write the files back, just output a diff for each file on stdout.
 
 * --color: Show colored diff. Only applies when `--diff` is given.
 
-* --sort-keys: Sort the output of dictionaries alphabetically by key.
+* --sort-keys: Sort the output of dictionaries alphabetically by key. *Available on Python 3.5+.*
+
+* --indent: Separate items with newlines and use this number of spaces for indentation.
+
+* --tab: Separate items with newlines and use tabs for indentation.
+
+* --no-indent: Separate items with spaces rather than newlines.
+
+* --compact: Suppress all whitespace separation (most compact).
+
+  *--indent, --tab, --no-indent, --compact — mutually exclusive options for whitespace control. Available on Python 3.9+.*
 
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

