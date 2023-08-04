# Comparing `tmp/csbschema-1.1.0.tar.gz` & `tmp/csbschema-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csbschema-1.1.0.tar", last modified: Tue Aug  1 19:37:24 2023, max compression
+gzip compressed data, was "csbschema-1.1.1.tar", last modified: Fri Aug  4 20:16:47 2023, max compression
```

## Comparing `csbschema-1.1.0.tar` & `csbschema-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.978525 csbschema-1.1.0/
--rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.1.0/LICENSE.txt
--rw-r--r--   0 miles      (505) staff       (20)      376 2023-08-01 19:35:57.000000 csbschema-1.1.0/MANIFEST.in
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-01 19:37:24.978412 csbschema-1.1.0/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.1.0/README.md
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.975237 csbschema-1.1.0/csbschema/
--rw-r--r--   0 miles      (505) staff       (20)     1911 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/__init__.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.976660 csbschema-1.1.0/csbschema/command/
--rw-r--r--   0 miles      (505) staff       (20)      285 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)     1368 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/__main__.py
--rw-r--r--   0 miles      (505) staff       (20)     1234 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/command/validate.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.978284 csbschema-1.1.0/csbschema/data/
--rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    27028 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    24735 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)    24283 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/CSB-schema-3_2_0-BETA.json
--rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    24608 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
--rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.1.0/csbschema/data/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)    29329 2023-08-01 19:35:57.000000 csbschema-1.1.0/csbschema/validators.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-01 19:37:24.976241 csbschema-1.1.0/csbschema.egg-info/
--rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)      731 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/SOURCES.txt
--rw-r--r--   0 miles      (505) staff       (20)        1 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/dependency_links.txt
--rw-r--r--   0 miles      (505) staff       (20)       62 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/entry_points.txt
--rw-r--r--   0 miles      (505) staff       (20)      135 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/requires.txt
--rw-r--r--   0 miles      (505) staff       (20)       10 2023-08-01 19:37:24.000000 csbschema-1.1.0/csbschema.egg-info/top_level.txt
--rw-r--r--   0 miles      (505) staff       (20)     1059 2023-08-01 19:35:57.000000 csbschema-1.1.0/pyproject.toml
--rw-r--r--   0 miles      (505) staff       (20)       38 2023-08-01 19:37:24.978554 csbschema-1.1.0/setup.cfg
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.234769 csbschema-1.1.1/
+-rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.1.1/LICENSE.txt
+-rw-r--r--   0 miles      (505) staff       (20)      433 2023-08-04 20:13:07.000000 csbschema-1.1.1/MANIFEST.in
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-04 20:16:47.234655 csbschema-1.1.1/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.1.1/README.md
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.231333 csbschema-1.1.1/csbschema/
+-rw-r--r--   0 miles      (505) staff       (20)     2041 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/__init__.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.232574 csbschema-1.1.1/csbschema/command/
+-rw-r--r--   0 miles      (505) staff       (20)      285 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1368 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/__main__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1234 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/command/validate.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.234534 csbschema-1.1.1/csbschema/data/
+-rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    27028 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24735 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    24283 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/CSB-schema-3_2_0-BETA.json
+-rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    24608 2023-08-01 19:35:57.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)    21489 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json
+-rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.1.1/csbschema/data/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)    32476 2023-08-04 20:13:07.000000 csbschema-1.1.1/csbschema/validators.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-08-04 20:16:47.232003 csbschema-1.1.1/csbschema.egg-info/
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)      780 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/SOURCES.txt
+-rw-r--r--   0 miles      (505) staff       (20)        1 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/dependency_links.txt
+-rw-r--r--   0 miles      (505) staff       (20)       62 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/entry_points.txt
+-rw-r--r--   0 miles      (505) staff       (20)      135 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/requires.txt
+-rw-r--r--   0 miles      (505) staff       (20)       10 2023-08-04 20:16:47.000000 csbschema-1.1.1/csbschema.egg-info/top_level.txt
+-rw-r--r--   0 miles      (505) staff       (20)     1059 2023-08-01 19:35:57.000000 csbschema-1.1.1/pyproject.toml
+-rw-r--r--   0 miles      (505) staff       (20)       38 2023-08-04 20:16:47.234806 csbschema-1.1.1/setup.cfg
```

### Comparing `csbschema-1.1.0/LICENSE.txt` & `csbschema-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/PKG-INFO` & `csbschema-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.1.0
+Version: 1.1.1
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `csbschema-1.1.0/README.md` & `csbschema-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/__init__.py` & `csbschema-1.1.1/csbschema/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from pathlib import Path
 from typing import Tuple, Union
 
 from csbschema import validators
 
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 # Current versions
 B12_VERSION_3_1_0_2023_08 = '3.1.0-2023-08'
 B12_VERSION_3_0_0_2023_08 = '3.0.0-2023-08'
+XYZ_B12_VERSION_3_1_0_2023_08 = 'XYZ-3.1.0-2023-08'
 XYZ_B12_VERSION_3_0_0_2023_08 = 'XYZ-3.0.0-2023-08'
 # Previous versions
 B12_VERSION_3_0_0_2023_03 = '3.0.0-2023-03'
 XYZ_B12_VERSION_3_0_0_2023_03 = 'XYZ-3.0.0-2023-03'
 B12_VERSION_3_1_0_2023_03 = '3.1.0-2023-03'
 # Development versions
 B12_VERSION_3_2_0_BETA = '3.2.0-BETA'
 
 DEFAULT_VALIDATOR_VERSION = B12_VERSION_3_1_0_2023_08
 VALIDATORS = {
     # Current versions
     B12_VERSION_3_1_0_2023_08: validators.validate_b12_3_1_0_2023_08,
+    XYZ_B12_VERSION_3_1_0_2023_08: validators.validate_b12_xyz_3_1_0_2023_08,
     B12_VERSION_3_0_0_2023_08: validators.validate_b12_3_0_0_2023_08,
     XYZ_B12_VERSION_3_0_0_2023_08: validators.validate_b12_xyz_3_0_0_2023_08,
     # Previous versions
     B12_VERSION_3_0_0_2023_03: validators.validate_b12_3_0_0_2023_03,
     XYZ_B12_VERSION_3_0_0_2023_03: validators.validate_b12_xyz_3_0_0_2023_03,
     B12_VERSION_3_1_0_2023_03: validators.validate_b12_3_1_0_2023_03,
     # Development versions
```

### Comparing `csbschema-1.1.0/csbschema/command/__main__.py` & `csbschema-1.1.1/csbschema/command/__main__.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/command/validate.py` & `csbschema-1.1.1/csbschema/command/validate.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/CSB-schema-3_0_0-2023-08.json` & `csbschema-1.1.1/csbschema/data/CSB-schema-3_0_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-03.json` & `csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/CSB-schema-3_1_0-2023-08.json` & `csbschema-1.1.1/csbschema/data/CSB-schema-3_1_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/CSB-schema-3_2_0-BETA.json` & `csbschema-1.1.1/csbschema/data/CSB-schema-3_2_0-BETA.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json` & `csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json` & `csbschema-1.1.1/csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.1.0/csbschema/validators.py` & `csbschema-1.1.1/csbschema/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -341,66 +341,84 @@
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     return validate_b12_xyz_3_0_0('XYZ-CSB-schema-3_0_0-2023-08.json', document_path)
 
 
-def validate_b12_3_1_0_properties(document: dict, errors: List) -> None:
+def validate_b12_3_1_0_platform(properties: dict, errors: List, *,
+                                context_path: str = '/properties') -> None:
     """
     Do custom semantic validation on metadata properties
     """
-    properties: dict = _get_properties(document, errors)
-    if properties is None:
-        return
-
-    if 'platform' not in properties:
-        return
-
     # There is 'platform' metadata, in which case we'll want to do some custom validation
     platform = properties['platform']
     # Custom validator for Platform.IDNumber, which depends on Platform.IDType
     if 'IDType' not in platform:
-        errors.append(_error_factory('/properties/platform',
+        errors.append(_error_factory(f"{context_path}/platform",
                                      "'IDType' attribute not present, but must be."))
     id_type = platform['IDType']
     if 'IDNumber' not in platform:
-        errors.append(_error_factory('/properties/platform',
+        errors.append(_error_factory(f"{context_path}/platform",
                                      "'IDNumber' attribute not present, but must be."))
     id_number = platform['IDNumber']
     try:
         if not ID_NUMBER_RE[id_type].match(id_number):
-            errors.append(_error_factory('/properties/platform/IDNumber',
+            errors.append(_error_factory(f"{context_path}/platform/IDNumber",
                                          f"IDNumber {id_number} is not valid for IDType {id_type}."))
     except KeyError:
-        errors.append(_error_factory('/properties/platform/IDType',
+        errors.append(_error_factory(f"{context_path}/platform/IDType",
                                      f"Unknown IDType {id_type}."))
 
     # Add custom validator for Platform.dataProcessed, which if False, Processing entries should not be present.
     data_processed = platform.get('dataProcessed', False)
     if data_processed:
         # dataProcessed is True, so "processing" entry ought to be present
         if 'processing' not in properties:
-            errors.append(_error_factory('/properties/platform/dataProcessed',
+            errors.append(_error_factory(f"{context_path}/platform/dataProcessed",
                                          f"dataProcessed flag is 'true', but 'processing' properties were not found."))
     else:
         # dataProcessed is False, so "processing" entry should not be present
         if 'processing' in properties:
-            errors.append(_error_factory('/properties/platform/dataProcessed',
+            errors.append(_error_factory(f"{context_path}/platform/dataProcessed",
                                          f"dataProcessed flag is 'false', but 'processing' properties were found."))
     if 'uniqueID' in platform:
         # 'uniqueID' can be present in platform as a duplicate of the required element 'uniqueVesselID` in
         # trustedNode. This is necessary to provide backward compatibility with DCDB ingest processing.
         if platform['uniqueID'] != properties['trustedNode']['uniqueVesselID']:
-            errors.append(_error_factory('/properties/platform/uniqueID',
+            errors.append(_error_factory(f"{context_path}/platform/uniqueID",
                                          f"uniqueID: {platform['uniqueID']} "
-                                         'does not match /properties/trustedNode/uniqueVesselID: '
+                                         f"does not match {context_path}/trustedNode/uniqueVesselID: "
                                          f"{properties['trustedNode']['uniqueVesselID']}"))
 
 
+def validate_b12_3_1_0_properties(document: dict, errors: List) -> None:
+    """
+    Do custom semantic validation on metadata properties
+    """
+    properties: dict = _get_properties(document, errors)
+    if properties is None:
+        return
+
+    if 'platform' not in properties:
+        return
+
+    validate_b12_3_1_0_platform(properties, errors)
+
+
+def validate_b12_xyz_3_1_0_properties(document: dict, errors: List) -> None:
+    """
+    Do custom semantic validation on metadata properties
+    """
+    if 'platform' not in document:
+        return
+
+    validate_b12_3_1_0_platform(document, errors, context_path='')
+
+
 def validate_b12_3_1_0_plus_features(document: dict, errors: List,
                                      get_processing_meta: Callable[[dict, list], Optional[dict]] = \
                                              _get_properties_processing) -> None:
     """
     Do custom semantic validation on features for B12 v. 3.1.0, 3.2.0-BETA, and later
     """
 
@@ -463,25 +481,55 @@
     validate_b12_3_1_0_properties(document, errors)
     if validate_uncertainty:
         validate_b12_3_1_0_plus_features(document, errors)
 
     return _validate_return(document, errors)
 
 
+def validate_b12_xyz_3_1_0(schema_rsrc_name: str,
+                           document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.1.0 CSB data and metadata against JSON schema
+    :param schema_rsrc_name: Internal resource name of schema document to use for validation
+    :param document_path: The document to validate
+    :param validate_uncertainty: Boolean flag controlling whether uncertainty metadata should be validated.
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    validator = _get_validator(schema_rsrc_name)
+    document = _open_document(document_path)
+
+    # Do "structural" validation using jsonschema and capture all errors encountered
+    errors = []
+    for e in validator.iter_errors(document):
+        # Basic validation against schema failed, note the failures, but allow validation to continue
+        errors.append(_error_factory('/' + '/'.join([str(elem) for elem in e.absolute_path]),
+                                     e.message))
+
+    # Do custom "semantic" validation that is difficult/not possible to express in JSON schema
+    validate_b12_xyz_3_1_0_properties(document, errors)
+
+    return _validate_return(document, errors)
+
+
 def validate_b12_3_1_0_2023_03(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.1.0 CSB data and metadata against 2023-03 JSON schema
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
         a single key 'document' whose value is a dict representing the document that was validated. If bool is False
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
-    return validate_b12_3_1_0('CSB-schema-3_1_0-2023-03.json', document_path, validate_uncertainty=False)
+    return validate_b12_3_1_0('CSB-schema-3_1_0-2023-03.json', document_path,
+                              validate_uncertainty=False)
 
 
 def validate_b12_3_1_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
     """
     Validate B12 version 3.1.0 CSB data and metadata against 2023-08 JSON schema
     :param document_path: The document to validate
     :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
@@ -489,14 +537,27 @@
         (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
         is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
         of dicts mapping JSON path elements to errors encountered at that element.
     """
     return validate_b12_3_1_0('CSB-schema-3_1_0-2023-08.json', document_path)
 
 
+def validate_b12_xyz_3_1_0_2023_08(document_path: Union[Path, str]) -> Tuple[bool, dict]:
+    """
+    Validate B12 version 3.1.0 CSB data and metadata against 2023-08 JSON schema
+    :param document_path: The document to validate
+    :return: Tuple[bool, dict]. If bool is True (which signals that validation succeeded), then dict will contain
+        a single key 'document' whose value is a dict representing the document that was validated. If bool is False
+        (which signals that validation failed), then dict will contain two keys: (1) 'document' whose value
+        is a dict representing the document that failed validation; and (2) 'errors' whose value is a list
+        of dicts mapping JSON path elements to errors encountered at that element.
+    """
+    return validate_b12_xyz_3_1_0('XYZ-CSB-schema-3_1_0-2023-08.json', document_path)
+
+
 def validate_b12_3_2_0_properties(document: dict, errors: List) -> None:
     properties: dict = _get_properties(document, errors)
     if properties is None:
         return None
 
     # See if there is 'trustedNodePlatform' metadata, in which case we'll want to do some custom validation
     if 'trustedNodePlatform' in properties:
```

### Comparing `csbschema-1.1.0/csbschema.egg-info/PKG-INFO` & `csbschema-1.1.1/csbschema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.1.0
+Version: 1.1.1
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `csbschema-1.1.0/csbschema.egg-info/SOURCES.txt` & `csbschema-1.1.1/csbschema.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 csbschema/data/CSB-schema-3_0_0-2023-03.json
 csbschema/data/CSB-schema-3_0_0-2023-08.json
 csbschema/data/CSB-schema-3_1_0-2023-03.json
 csbschema/data/CSB-schema-3_1_0-2023-08.json
 csbschema/data/CSB-schema-3_2_0-BETA.json
 csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
 csbschema/data/XYZ-CSB-schema-3_0_0-2023-08.json
+csbschema/data/XYZ-CSB-schema-3_1_0-2023-08.json
 csbschema/data/__init__.py
```

### Comparing `csbschema-1.1.0/pyproject.toml` & `csbschema-1.1.1/pyproject.toml`

 * *Files identical despite different names*

