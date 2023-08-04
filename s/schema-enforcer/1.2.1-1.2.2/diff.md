# Comparing `tmp/schema_enforcer-1.2.1.tar.gz` & `tmp/schema_enforcer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_enforcer-1.2.1.tar", max compression
+gzip compressed data, was "schema_enforcer-1.2.2.tar", max compression
```

## Comparing `schema_enforcer-1.2.1.tar` & `schema_enforcer-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     2374 2023-06-13 15:24:24.105442 schema_enforcer-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      602 2023-06-13 15:24:24.109443 schema_enforcer-1.2.1/LICENSE
--rwxr-xr-x   0        0        0    10213 2023-06-13 15:24:24.109443 schema_enforcer-1.2.1/README.md
--rwxr-xr-x   0        0        0     2126 2023-06-13 15:24:36.510090 schema_enforcer-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/__init__.py
--rw-r--r--   0        0        0    10605 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/ansible_inventory.py
--rw-r--r--   0        0        0    12628 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/cli.py
--rw-r--r--   0        0        0     4038 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/config.py
--rw-r--r--   0        0        0     1384 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/exceptions.py
--rw-r--r--   0        0        0     6980 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/instances/file.py
--rw-r--r--   0        0        0     6181 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/jsonschema.py
--rw-r--r--   0        0        0    13444 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/manager.py
--rw-r--r--   0        0        0     4022 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/validator.py
--rwxr-xr-x   0        0        0    18373 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/utils.py
--rw-r--r--   0        0        0     2608 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/validation.py
--rw-r--r--   0        0        0    11605 1970-01-01 00:00:00.000000 schema_enforcer-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2465 2023-08-04 16:02:46.540902 schema_enforcer-1.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      602 2023-08-04 16:02:46.540902 schema_enforcer-1.2.2/LICENSE
+-rwxr-xr-x   0        0        0     9445 2023-08-04 16:02:46.540902 schema_enforcer-1.2.2/README.md
+-rwxr-xr-x   0        0        0     2104 2023-08-04 16:02:58.732924 schema_enforcer-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    10605 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/ansible_inventory.py
+-rw-r--r--   0        0        0    12628 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/cli.py
+-rw-r--r--   0        0        0     4038 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/config.py
+-rw-r--r--   0        0        0     1384 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/exceptions.py
+-rw-r--r--   0        0        0     6980 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/instances/file.py
+-rw-r--r--   0        0        0     4979 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/schemas/draft7_schema.json
+-rw-r--r--   0        0        0     6352 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/schemas/jsonschema.py
+-rw-r--r--   0        0        0    13471 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/schemas/manager.py
+-rw-r--r--   0        0        0     4022 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/schemas/validator.py
+-rwxr-xr-x   0        0        0    18355 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/utils.py
+-rw-r--r--   0        0        0     2595 2023-08-04 16:02:46.548902 schema_enforcer-1.2.2/schema_enforcer/validation.py
+-rw-r--r--   0        0        0    10787 1970-01-01 00:00:00.000000 schema_enforcer-1.2.2/PKG-INFO
```

### Comparing `schema_enforcer-1.2.1/CHANGELOG.md` & `schema_enforcer-1.2.2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
+## v1.2.2
+
+- #156 Add support for jsonschema 4.18
+- Remove support for python version 3.7
+
 ## v1.2.1
 
 ### Changes
 
-- #152 Update requirement for rich to ^12.5.1
+- #152 Update requirement for rich to `>=9.5`
 
 ## v1.2.0 - 2023-06-05
 
 ### Adds
 
 - Support for versions of jsonschema >= 4.6
```

### Comparing `schema_enforcer-1.2.1/LICENSE` & `schema_enforcer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/README.md` & `schema_enforcer-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 # Schema Enforcer
 
-Schema Enforcer provides a framework for testing structured data against schema definitions. Right now, [JSONSchema](https://json-schema.org/understanding-json-schema/index.html) is the only schema definition language supported, but we are thinking about adding other schema definition languages at some point in the future.
+Schema Enforcer provides a framework for testing structured data against schema definitions using [JSONSchema](https://json-schema.org/understanding-json-schema/index.html).
 
 ## Getting Started
 
 ### Install
 
-Schema Enforcer is a python library which is available on PyPi. It requires a python version of 3.7 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.
+Schema Enforcer is a python library which is available on PyPi. It requires a python version of 3.8 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.
 
 ```cli
-bash$ python --version
-Python 3.7.9
-
-bash$ pip --version
-pip 20.1.1 from /usr/local/lib/python3.7/site-packages/pip (python 3.7)
-
 python -m pip install schema-enforcer
 ```
 
-> Note: To determine the version of python your system is using, the command `python --version` can be run from a terminal emulator
-
-> Note: Pip is a package manager for python. While most recent versions of python come with pip installed, some do not. You can determine if pip is installed on your system using the command `pip --version`. If it is not, the instructions for installing it, once python has been installed, can be found [here](https://pip.pypa.io/en/stable/installing/)
-
 ### Overview
 
 Schema Enforcer requires that two different elements be defined by the user:
 
 - Schema Definition Files: These are files which define the schema to which a given set of data should adhere.
 - Structured Data Files: These are files which contain data that should adhere to the schema defined in one (or multiple) of the schema definition files.
```

### Comparing `schema_enforcer-1.2.1/pyproject.toml` & `schema_enforcer-1.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "schema-enforcer"
-version = "v1.2.1"
+version = "v1.2.2"
 description = "Tool/Framework for testing structured data against schema definitions"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode/schema-enforcer"
 repository = "https://github.com/networktocode/schema-enforcer"
 include = [
     "CHANGELOG.md",
     "LICENSE",
     "README.md",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 click = "^7.1 || ^8.0"
 termcolor = "^1.1"
 toml = "^0.10"
 "ruamel.yaml" = "^0.16 || ^0.17"
 jinja2 = ">=2.11"
 jsonref = "^0.2"
 pydantic = "^1.6"
@@ -68,15 +68,14 @@
 no-docstring-rgx="^(_|test_)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
 disable = """,
     line-too-long,
-    bad-continuation,
     """
 
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
```

### Comparing `schema_enforcer-1.2.1/schema_enforcer/ansible_inventory.py` & `schema_enforcer-1.2.2/schema_enforcer/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/cli.py` & `schema_enforcer-1.2.2/schema_enforcer/cli.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/config.py` & `schema_enforcer-1.2.2/schema_enforcer/config.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/exceptions.py` & `schema_enforcer-1.2.2/schema_enforcer/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/instances/file.py` & `schema_enforcer-1.2.2/schema_enforcer/instances/file.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/schemas/jsonschema.py` & `schema_enforcer-1.2.2/schema_enforcer/schemas/jsonschema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """class to manage jsonschema type schema."""
 import copy
-import pkgutil
 import json
+import os
+from functools import cached_property
 
-from jsonschema import Draft7Validator, draft7_format_checker  # pylint: disable=import-self
+from jsonschema import Draft7Validator  # pylint: disable=import-self
 from schema_enforcer.schemas.validator import BaseValidation
 from schema_enforcer.validation import ValidationResult, RESULT_FAIL, RESULT_PASS
 
-# TODO do we need to catch a possible exception here ?
-v7data = pkgutil.get_data("jsonschema", "schemas/draft7.json")
-v7schema = json.loads(v7data.decode("utf-8"))
-
 
 class JsonSchema(BaseValidation):  # pylint: disable=too-many-instance-attributes
     """class to manage jsonschema type schemas."""
 
     schematype = "jsonchema"
 
     def __init__(self, schema, filename, root):
@@ -29,15 +26,24 @@
         self.filename = filename
         self.root = root
         self.data = schema
         self.id = self.data.get("$id")  # pylint: disable=invalid-name
         self.top_level_properties = set(self.data.get("properties"))
         self.validator = None
         self.strict_validator = None
-        self.format_checker = draft7_format_checker
+        self.format_checker = Draft7Validator.FORMAT_CHECKER
+
+    @cached_property
+    def v7_schema(self):
+        """Draft7 Schema."""
+        local_dirname = os.path.dirname(os.path.abspath(__file__))
+        with open(os.path.join(local_dirname, "draft7_schema.json"), encoding="utf-8") as fhd:
+            v7_schema = json.loads(fhd.read())
+
+        return v7_schema
 
     def get_id(self):
         """Return the unique ID of the schema."""
         return self.id
 
     def validate(self, data, strict=False):
         """Validate a given data with this schema.
@@ -127,15 +133,15 @@
 
     def check_if_valid(self):
         """Check if the schema definition is valid against JsonSchema draft7.
 
         Returns:
             List[ValidationResult]: A list of validation result objects.
         """
-        validator = Draft7Validator(v7schema, format_checker=self.format_checker)
+        validator = Draft7Validator(self.v7_schema, format_checker=self.format_checker)
 
         results = []
         has_error = False
         for err in validator.iter_errors(self.data):
             has_error = True
 
             results.append(
```

### Comparing `schema_enforcer-1.2.1/schema_enforcer/schemas/manager.py` & `schema_enforcer-1.2.2/schema_enforcer/schemas/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             schema = self.create_schema_from_file(root, filename)
             self.schemas[schema.get_id()] = schema
 
         # Load validators
         validators = load_validators(config.validator_directory)
         self.schemas.update(validators)
 
-    def create_schema_from_file(self, root, filename):  # pylint: disable=no-self-use
+    def create_schema_from_file(self, root, filename):
         """Create a new JsonSchema object for a given file.
 
         Load the content from disk and resolve all JSONRef within the schema file.
 
         Args:
             root (string): Absolute location of the file in the filesystem.
             filename (string): Name of the file.
@@ -222,17 +222,21 @@
             # Currently the expected results are using OrderedDict instead of Dict
             # the easiest way to remove that is to dump into JSON and convert back into a "normal" dict
             expected_results = json.loads(json.dumps(expected_results["results"]))
 
             results_sorted = sorted(tmp_results, key=lambda i: i.get("message", ""))
             expected_results_sorted = sorted(expected_results, key=lambda i: i.get("message", ""))
 
-            params = dict(
-                schema_id=schema_id, instance_type="TEST", instance_name=test_dir, instance_location=invalid_test_dir
-            )
+            params = {
+                "schema_id": schema_id,
+                "instance_type": "TEST",
+                "instance_name": test_dir,
+                "instance_location": invalid_test_dir,
+            }
+
             if results_sorted != expected_results_sorted:
                 params["result"] = RESULT_FAIL
                 params[
                     "message"
                 ] = f"Invalid test results do not match expected test results from {expected_results_file}"
             else:
                 params["result"] = RESULT_PASS
```

### Comparing `schema_enforcer-1.2.1/schema_enforcer/schemas/validator.py` & `schema_enforcer-1.2.2/schema_enforcer/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.1/schema_enforcer/utils.py` & `schema_enforcer-1.2.2/schema_enforcer/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import importlib
 
 from ruamel.yaml import YAML
 from ruamel.yaml.scalarstring import DoubleQuotedScalarString as DQ
 from jsonschema import (  # pylint: disable=no-name-in-module
     RefResolver,
     Draft7Validator,
-    draft7_format_checker,
 )
 
 from termcolor import colored
 
 
 from click import Option, UsageError
 
@@ -163,15 +162,15 @@
     with open(os.path.join(schema_root_dir, schema_filepath), encoding="utf-8") as fileh:
         schema_definition = json.load(fileh)
 
     # Notes: The Draft7Validator will use the base_uri to resolve any relative references within the loaded schema_defnition
     # these references must match the full filenames currently, unless we modify the RefResolver to handle other cases.
     validator = Draft7Validator(
         schema_definition,
-        format_checker=draft7_format_checker,
+        format_checker=Draft7Validator.FORMAT_CHECKER,
         resolver=RefResolver(base_uri=base_uri, referrer=schema_definition),
     )
     return validator
 
 
 def dump_data_to_yaml(data, yaml_path):
     """Dumps data to a YAML file with special formatting.
```

### Comparing `schema_enforcer-1.2.1/schema_enforcer/validation.py` & `schema_enforcer-1.2.2/schema_enforcer/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     strict: bool = False
 
     # if failed
     absolute_path: Optional[List[str]] = []
     message: Optional[str]
 
     @validator("result")
-    def result_must_be_pass_or_fail(cls, var):  # pylint: disable=no-self-argument, no-self-use
+    def result_must_be_pass_or_fail(cls, var):  # pylint: disable=no-self-argument
         """Validate that result either PASS or FAIL."""
         if var.upper() not in [RESULT_PASS, RESULT_FAIL]:
             raise ValueError("must be either PASS or FAIL")
         return var.upper()
 
     def passed(self):
         """Return True or False to indicate if the test has passed.
```

### Comparing `schema_enforcer-1.2.1/PKG-INFO` & `schema_enforcer-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: schema-enforcer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tool/Framework for testing structured data against schema definitions
 Home-page: https://github.com/networktocode/schema-enforcer
 License: Apache-2.0
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ansible
 Provides-Extra: ansible-base
 Requires-Dist: ansible (>=2.10.0,<3.0.0) ; extra == "ansible"
@@ -30,36 +29,26 @@
 Requires-Dist: termcolor (>=1.1,<2.0)
 Requires-Dist: toml (>=0.10,<0.11)
 Project-URL: Repository, https://github.com/networktocode/schema-enforcer
 Description-Content-Type: text/markdown
 
 # Schema Enforcer
 
-Schema Enforcer provides a framework for testing structured data against schema definitions. Right now, [JSONSchema](https://json-schema.org/understanding-json-schema/index.html) is the only schema definition language supported, but we are thinking about adding other schema definition languages at some point in the future.
+Schema Enforcer provides a framework for testing structured data against schema definitions using [JSONSchema](https://json-schema.org/understanding-json-schema/index.html).
 
 ## Getting Started
 
 ### Install
 
-Schema Enforcer is a python library which is available on PyPi. It requires a python version of 3.7 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.
+Schema Enforcer is a python library which is available on PyPi. It requires a python version of 3.8 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.
 
 ```cli
-bash$ python --version
-Python 3.7.9
-
-bash$ pip --version
-pip 20.1.1 from /usr/local/lib/python3.7/site-packages/pip (python 3.7)
-
 python -m pip install schema-enforcer
 ```
 
-> Note: To determine the version of python your system is using, the command `python --version` can be run from a terminal emulator
-
-> Note: Pip is a package manager for python. While most recent versions of python come with pip installed, some do not. You can determine if pip is installed on your system using the command `pip --version`. If it is not, the instructions for installing it, once python has been installed, can be found [here](https://pip.pypa.io/en/stable/installing/)
-
 ### Overview
 
 Schema Enforcer requires that two different elements be defined by the user:
 
 - Schema Definition Files: These are files which define the schema to which a given set of data should adhere.
 - Structured Data Files: These are files which contain data that should adhere to the schema defined in one (or multiple) of the schema definition files.
```

