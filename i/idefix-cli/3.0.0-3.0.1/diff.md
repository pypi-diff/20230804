# Comparing `tmp/idefix_cli-3.0.0.tar.gz` & `tmp/idefix_cli-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-3.0.0.tar", last modified: Wed Aug  2 16:05:56 2023, max compression
+gzip compressed data, was "idefix_cli-3.0.1.tar", last modified: Thu Aug  3 10:44:35 2023, max compression
```

## Comparing `idefix_cli-3.0.0.tar` & `idefix_cli-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/src/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.496300 idefix_cli-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-03 10:44:35.496300 idefix_cli-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:44:35.496300 idefix_cli-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.488300 idefix_cli-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.492300 idefix_cli-3.0.1/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.492300 idefix_cli-3.0.1/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.492300 idefix_cli-3.0.1/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 10:44:35.000000 idefix_cli-3.0.1/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:35.496300 idefix_cli-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-03 10:44:21.000000 idefix_cli-3.0.1/tests/test_write.py
```

### Comparing `idefix_cli-3.0.0/LICENSE` & `idefix_cli-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/PKG-INFO` & `idefix_cli-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-3.0.0/README.md` & `idefix_cli-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/pyproject.toml` & `idefix_cli-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/__main__.py` & `idefix_cli-3.0.1/src/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_backports.py` & `idefix_cli-3.0.1/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/clean.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/clone.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/conf.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/digest.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/digest.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,52 +8,31 @@
 from typing import Any
 
 from idefix_cli.lib import print_err
 
 _LOG_LINE_REGEXP = re.compile(r"^(?P<trailer>TimeIntegrator:)(?P<data>.*\|.*)")
 
 
-def _parse_token(raw_data: str):
-    sdata = raw_data.strip()
-    if sdata == "N/A":
-        return float("nan")
-    try:
-        return int(sdata)
-    except ValueError:
-        pass
-    try:
-        return float(sdata)
-    except ValueError:
-        pass
-    return sdata
-
-
 def _log_to_data(log: list[str]):
     columns: dict[str, list[Any]] = {name.strip(): [] for name in log[0].split("|")}
-    types = [type(_parse_token(t)) for t in log[1].split("|")]
     tokenized_log = [line.replace("N/A", "NaN").split("|") for line in log[1:]]
     for i, name in enumerate(columns.keys()):
         columns[name] = [L[i] for L in tokenized_log]
-    return columns, types
+    return columns
 
 
-def _data_to_json(header: str, data: dict[str, list[str]], types: list[type]) -> str:
+def _data_to_json(header: str, data: dict[str, list[str]]) -> str:
     res: list[str] = ['"%s": {' % header]
-    ncolumns = len(types)
-    for icol, ((name, record), t) in enumerate(zip(data.items(), types)):
+    ncolumns = len(data)
+    for icol, (name, record) in enumerate(data.items()):
         if icol < ncolumns - 1:
             trail = ","
         else:
             trail = ""
-        line = '"%s":' % name
-        if t is str:
-            line += '  ["' + ', "'.join(record) + '"]' + trail
-        else:
-            line += "  [" + ", ".join(record) + "]" + trail
-        res.append(line)
+        res.append(f'"{name}":[{",".join([_.strip() for _ in record])}]{trail}')
 
     res.append("}")
     return "\n".join(res)
 
 
 def add_arguments(parser: ArgumentParser) -> None:
     parser.add_argument(
@@ -127,16 +106,16 @@
     if len(data) > 1:
         for p, c in zip(log_files[1:], data[1:]):
             if c[0] != header:  # pragma: no cover
                 print_err(f"header mismatch from {p} and {log_files[0]}")
 
     final_result: list[str] = []
     for p, d in zip(log_files, data):
-        columns, types = _log_to_data(d)
-        final_result.append(_data_to_json(p.name, columns, types))
+        columns = _log_to_data(d)
+        final_result.append(_data_to_json(p.name, columns))
 
     _json = "{\n" + ",\n".join(final_result) + "\n}"
     if isinstance(output, str):
         with open(output, "w") as fh:
             print(_json, file=fh)
     else:
         print(_json, file=output)
```

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/read.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/run.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/stamp.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/switch.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/_commands/write.py` & `idefix_cli-3.0.1/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli/lib.py` & `idefix_cli-3.0.1/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/src/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-3.0.1/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-3.0.0/src/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-3.0.1/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_app_structure.py` & `idefix_cli-3.0.1/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_clean.py` & `idefix_cli-3.0.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_clone.py` & `idefix_cli-3.0.1/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_commons.py` & `idefix_cli-3.0.1/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_conf.py` & `idefix_cli-3.0.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_digest.py` & `idefix_cli-3.0.1/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_read.py` & `idefix_cli-3.0.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_run.py` & `idefix_cli-3.0.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_stamp.py` & `idefix_cli-3.0.1/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_ux.py` & `idefix_cli-3.0.1/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-3.0.0/tests/test_write.py` & `idefix_cli-3.0.1/tests/test_write.py`

 * *Files identical despite different names*

