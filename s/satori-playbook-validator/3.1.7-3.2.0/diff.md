# Comparing `tmp/satori_playbook_validator-3.1.7.tar.gz` & `tmp/satori_playbook_validator-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-3.1.7.tar", last modified: Mon Jul 17 13:10:19 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.2.0.tar", last modified: Fri Aug  4 04:28:54 2023, max compression
```

## Comparing `satori_playbook_validator-3.1.7.tar` & `satori_playbook_validator-3.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/README.md
--rw-r--r--   0        0        0      518 2023-07-17 13:10:19.259078 satori_playbook_validator-3.1.7/pyproject.toml
--rw-r--r--   0        0        0      301 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     6212 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      298 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1906 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2361 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      100 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/src/satorici/validator/warnings.py
--rw-r--r--   0        0        0     2659 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-07-17 13:10:03.006657 satori_playbook_validator-3.1.7/tests/test_reference_finder.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/README.md
+-rw-r--r--   0        0        0      518 2023-08-04 04:28:54.245092 satori_playbook_validator-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     6470 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      361 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1906 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     2906 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-08-04 04:28:37.112410 satori_playbook_validator-3.2.0/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.2.0/PKG-INFO
```

### Comparing `satori_playbook_validator-3.1.7/pyproject.toml` & `satori_playbook_validator-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-playbook-validator"
-version = "3.1.7"
+version = "3.2.0"
 description = ""
 authors = [
     { name = "Satori CI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "fastjsonschema>=2.17.1",
     "aws-cron-expression-validator>=1.1.6",
```

### Comparing `satori_playbook_validator-3.1.7/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.2.0/src/satorici/validator/_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import re
+import shlex
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from urllib.parse import urlsplit
 
 from aws_cron_expression_validator.validator import AWSCronExpressionValidator
 from fastjsonschema import JsonSchemaValueException, compile
 
 from .exceptions import (
+    InvalidCommandError,
     NoExecutionsError,
     PlaybookValidationError,
     PlaybookVariableError,
 )
 from .warnings import NoLogMonitorWarning
 
 INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
@@ -182,14 +184,21 @@
         path, current = stack.pop()
 
         for k, v in (i for i in current.items() if "^" not in i[0]):
             if isinstance(v, dict):
                 stack.append((path + (k,), v))
             elif is_command_group(v):
                 execution_found = True
+
+                for cmd in v:
+                    try:
+                        _ = shlex.split(cmd[0])
+                    except ValueError as e:
+                        raise InvalidCommandError(f"{e} on {cmd[0]}.")
+
                 if get_reference_names(v):
                     validate_references(current, k)
 
     if not execution_found:
         raise NoExecutionsError("No executions found.")
```

### Comparing `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.2.0/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-3.2.0/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.7/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.2.0/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.7/tests/test_playbook_validator.py` & `satori_playbook_validator-3.2.0/tests/test_playbook_validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     validate_playbook(playbook)
 
 
 def test_monitor_without_notification():
     playbook = {
         "settings": {
             "name": "aaaa",
-            "cron": "0 0 0 0 0",
+            "cron": "1 * * * ? *",
         },
         "cmd": [
             ["echo"],
         ],
     }
 
     with pytest.warns(NoLogMonitorWarning):
@@ -137,7 +137,21 @@
         },
         "cmd": [
             ["echo"],
         ],
     }
 
     validate_playbook(playbook)
+
+
+def test_invalid_command():
+    playbook = {
+        "settings": {
+            "timeout": 1,
+        },
+        "cmd": [
+            ['"'],
+        ],
+    }
+
+    with pytest.raises(PlaybookValidationError):
+        validate_playbook(playbook)
```

### Comparing `satori_playbook_validator-3.1.7/tests/test_reference_finder.py` & `satori_playbook_validator-3.2.0/tests/test_reference_finder.py`

 * *Files identical despite different names*

