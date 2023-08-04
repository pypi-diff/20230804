# Comparing `tmp/cyclonedx_editor_validator-0.6.1.tar.gz` & `tmp/cyclonedx_editor_validator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_editor_validator-0.6.1.tar", max compression
+gzip compressed data, was "cyclonedx_editor_validator-0.7.0.tar", max compression
```

## Comparing `cyclonedx_editor_validator-0.6.1.tar` & `cyclonedx_editor_validator-0.7.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    35114 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/LICENSE
--rw-r--r--   0        0        0     2429 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/README.md
--rw-r--r--   0        0        0       34 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/__init__.py
--rw-r--r--   0        0        0    20098 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/__main__.py
--rw-r--r--   0        0        0      410 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/command.py
--rw-r--r--   0        0        0    59830 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/license_name_id_map.json
--rw-r--r--   0        0        0     6560 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/operations.py
--rw-r--r--   0        0        0     2062 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/replace_license_name_with_id.py
--rw-r--r--   0        0        0        0 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/__init__.py
--rw-r--r--   0        0        0     5793 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/identity.py
--rw-r--r--   0        0        0     3854 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/output.py
--rw-r--r--   0        0        0    10454 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/sbomFunctions.py
--rw-r--r--   0        0        0        0 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/__init__.py
--rw-r--r--   0        0        0    13619 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.0.xsd
--rw-r--r--   0        0        0    39484 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.1.xsd
--rw-r--r--   0        0        0    37056 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
--rw-r--r--   0        0        0    36058 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.schema.json
--rw-r--r--   0        0        0    76147 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.xsd
--rw-r--r--   0        0        0    43822 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
--rw-r--r--   0        0        0    40239 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
--rw-r--r--   0        0        0    23176 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.proto
--rw-r--r--   0        0        0    39180 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.schema.json
--rw-r--r--   0        0        0    88384 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.xsd
--rw-r--r--   0        0        0    76794 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
--rw-r--r--   0        0        0    34897 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.proto
--rw-r--r--   0        0        0    72249 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.schema.json
--rw-r--r--   0        0        0   133616 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.xsd
--rw-r--r--   0        0        0     9063 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
--rw-r--r--   0        0        0     8233 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
--rw-r--r--   0        0        0     3146 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
--rw-r--r--   0        0        0     6380 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14195 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
--rw-r--r--   0        0        0     8210 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/jsf-0.82.schema.json
--rw-r--r--   0        0        0    10482 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.schema.json
--rw-r--r--   0        0        0   125048 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.xsd
--rw-r--r--   0        0        0     5646 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/build_public_bom.py
--rw-r--r--   0        0        0     2642 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/error.py
--rw-r--r--   0        0        0     2763 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/log.py
--rw-r--r--   0        0        0    18104 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/merge.py
--rw-r--r--   0        0        0     2702 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/mergeVex.py
--rw-r--r--   0        0        0      135 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/pkg.py
--rw-r--r--   0        0        0     7211 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/set.py
--rw-r--r--   0        0        0       65 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/helper.py
--rw-r--r--   0        0        0     7098 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/validate.py
--rw-r--r--   0        0        0     3022 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/warningsngreport.py
--rw-r--r--   0        0        0     1684 2023-06-12 07:31:06.265780 cyclonedx_editor_validator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35114 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1302 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/README.md
+-rw-r--r--   0        0        0       34 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/__init__.py
+-rw-r--r--   0        0        0    20099 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/__main__.py
+-rw-r--r--   0        0        0      410 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/amend/__init__.py
+-rw-r--r--   0        0        0     1218 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/amend/command.py
+-rw-r--r--   0        0        0    59830 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/amend/license_name_id_map.json
+-rw-r--r--   0        0        0     6560 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/amend/operations.py
+-rw-r--r--   0        0        0     2066 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/amend/replace_license_name_with_id.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/__init__.py
+-rw-r--r--   0        0        0     5793 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/identity.py
+-rw-r--r--   0        0        0     3854 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/output.py
+-rw-r--r--   0        0        0    10454 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/sbomFunctions.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/__init__.py
+-rw-r--r--   0        0        0    13619 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.0.xsd
+-rw-r--r--   0        0        0    39484 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.1.xsd
+-rw-r--r--   0        0        0    37056 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
+-rw-r--r--   0        0        0    36058 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2.schema.json
+-rw-r--r--   0        0        0    76147 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2.xsd
+-rw-r--r--   0        0        0    43822 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
+-rw-r--r--   0        0        0    40239 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
+-rw-r--r--   0        0        0    23176 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.proto
+-rw-r--r--   0        0        0    39180 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.schema.json
+-rw-r--r--   0        0        0    88384 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.xsd
+-rw-r--r--   0        0        0    76794 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
+-rw-r--r--   0        0        0    34897 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.proto
+-rw-r--r--   0        0        0    72249 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.schema.json
+-rw-r--r--   0        0        0   133616 2023-08-04 15:09:40.407308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.xsd
+-rw-r--r--   0        0        0     9063 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
+-rw-r--r--   0        0        0     8233 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
+-rw-r--r--   0        0        0     3146 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
+-rw-r--r--   0        0        0     6380 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14195 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
+-rw-r--r--   0        0        0     8210 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/jsf-0.82.schema.json
+-rw-r--r--   0        0        0    10482 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/spdx.schema.json
+-rw-r--r--   0        0        0   125048 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/spdx.xsd
+-rw-r--r--   0        0        0     5646 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/build_public_bom.py
+-rw-r--r--   0        0        0     2642 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/error.py
+-rw-r--r--   0        0        0     2763 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/log.py
+-rw-r--r--   0        0        0    18104 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/merge.py
+-rw-r--r--   0        0        0     2702 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/merge_vex.py
+-rw-r--r--   0        0        0      135 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/pkg.py
+-rw-r--r--   0        0        0     7211 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/set.py
+-rw-r--r--   0        0        0       65 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/validator/__init__.py
+-rw-r--r--   0        0        0     4610 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/validator/helper.py
+-rw-r--r--   0        0        0     7098 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/validator/validate.py
+-rw-r--r--   0        0        0     3022 2023-08-04 15:09:40.411308 cyclonedx_editor_validator-0.7.0/cdxev/validator/warningsngreport.py
+-rw-r--r--   0        0        0     1689 2023-08-04 15:09:55.831425 cyclonedx_editor_validator-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.7.0/PKG-INFO
```

### Comparing `cyclonedx_editor_validator-0.6.1/LICENSE` & `cyclonedx_editor_validator-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/__main__.py` & `cyclonedx_editor_validator-0.7.0/cdxev/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from cdxev.amend.command import run as amend
 from cdxev.auxiliary.identity import Key, KeyType
 from cdxev.auxiliary.output import write_sbom
 from cdxev.build_public_bom import build_public_bom
 from cdxev.error import AppError, InputFileError
 from cdxev.log import configure_logging
 from cdxev.merge import merge
-from cdxev.mergeVex import merge_vex
+from cdxev.merge_vex import merge_vex
 from cdxev.validator import validate_sbom
 
 logger: logging.Logger
 _STATUS_OK = 0
 _STATUS_APP_ERROR = 2
 _STATUS_USAGE_ERROR = 3
 _STATUS_VALIDATION_ERROR = 4
```

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/amend/command.py` & `cyclonedx_editor_validator-0.7.0/cdxev/amend/command.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/amend/license_name_id_map.json` & `cyclonedx_editor_validator-0.7.0/cdxev/amend/license_name_id_map.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/amend/operations.py` & `cyclonedx_editor_validator-0.7.0/cdxev/amend/operations.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/amend/replace_license_name_with_id.py` & `cyclonedx_editor_validator-0.7.0/cdxev/amend/replace_license_name_with_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Returns
     -------
     str:
         Id of the given string
     """
     license_id = ""
-    if type(license_name) == str:
+    if isinstance(license_name, str):
         for dicts in license_namelist:
             if license_name.lower() == dicts.get("exp", "").lower():
                 license_id = dicts.get("exp", "")
             else:
                 for name in dicts.get("names", []):
                     if license_name.lower() == name.lower():
                         license_id = dicts.get("exp", "")
```

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/identity.py` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/identity.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/output.py` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/sbomFunctions.py` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/sbomFunctions.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.0.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.1.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.1.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2-strict.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.2.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-custom.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-strict.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.proto` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.3.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4-custom.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.proto` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/bom-1.4.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/jsf-0.82.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/jsf-0.82.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.schema.json` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/spdx.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.xsd` & `cyclonedx_editor_validator-0.7.0/cdxev/auxiliary/schema/spdx.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/build_public_bom.py` & `cyclonedx_editor_validator-0.7.0/cdxev/build_public_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/error.py` & `cyclonedx_editor_validator-0.7.0/cdxev/error.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/log.py` & `cyclonedx_editor_validator-0.7.0/cdxev/log.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/merge.py` & `cyclonedx_editor_validator-0.7.0/cdxev/merge.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/mergeVex.py` & `cyclonedx_editor_validator-0.7.0/cdxev/merge_vex.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/set.py` & `cyclonedx_editor_validator-0.7.0/cdxev/set.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/validator/helper.py` & `cyclonedx_editor_validator-0.7.0/cdxev/validator/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,28 +57,54 @@
             return False
         name_of_component = (
             sbom.get("metadata", {}).get("component", {}).get("name", "")
         )
         version_of_component = (
             sbom.get("metadata", {}).get("component", {}).get("version", "")
         )
+        hashes_of_component = (
+            sbom.get("metadata", {}).get("component", {}).get("hashes", [])
+        )
         if not name_of_component or not version_of_component:
             return False
+
+        component_hash = (
+            "([a-fA-F0-9]{32}|"
+            + "[a-fA-F0-9]{40}|"
+            + "[a-fA-F0-9]{64}|"
+            + "[a-fA-F0-9]{96}|"
+            + "[a-fA-F0-9]{128}"
+        )
+        if len(hashes_of_component) > 0:
+            filename_splitted = file.name.replace(".cdx.json", "").split("_")
+            for hash in hashes_of_component:
+                component_first_hash = [
+                    filename_part
+                    for filename_part in filename_splitted
+                    if hash["content"].startswith(filename_part)
+                ]
+            if component_first_hash:
+                component_hash = "(" + component_first_hash[0]
+            # if hash in file name is not one of the hashes in metadata, file name can not be valid
+            else:
+                return False
         valid_filename = re.search(
             "^"
             + re.escape(name_of_component)
             + "_"
             + re.escape(version_of_component)
-            + "_((([a-fA-F0-9]{32}|[a-fA-F0-9]{40}|[a-fA-F0-9]{64}|"
-            "[a-fA-F0-9]{96}|[a-fA-F0-9]{128})_"
+            + "_("
+            + component_hash
+            + ")_"
             + iso_timestamp
-            + ")|(([a-fA-F0-9]{32}|[a-fA-F0-9]{40}|[a-fA-F0-9]{64}|"
-            "[a-fA-F0-9]{96}|[a-fA-F0-9]{128})|"
+            + ")|"
+            + component_hash
+            + "|"
             + iso_timestamp
-            + "))(.cdx.json)$|^bom.json$",
+            + ")(.cdx.json)$|^bom.json$",
             file.name,
         )
     if valid_filename is not None:
         return True
     else:
         return False
```

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/validator/validate.py` & `cyclonedx_editor_validator-0.7.0/cdxev/validator/validate.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/cdxev/validator/warningsngreport.py` & `cyclonedx_editor_validator-0.7.0/cdxev/validator/warningsngreport.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.1/pyproject.toml` & `cyclonedx_editor_validator-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclonedx-editor-validator"
-version = "v0.6.1"
+version = "v0.7.0"
 description = "Tool for creating, modifying and validating CycloneDX SBOMs."
 authors = [
     "Aleg Vilinski <aleg.vilinski@festo.com>",
     "Christian Beck <christian.beck@festo.com>",
     "Moritz Marseu <moritz.marseu@festo.com>"
 ]
 license = "GPL-3.0-only"
@@ -22,25 +22,25 @@
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dateutil = "2.8.2"
 jsonschema = {version = "4.17.3", extras = ["format"]}
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "6"
-black = "23.3.0"
+flake8 = "6.1.0"
+black = "23.7.0"
 pep8-naming = "0.13.3"
-mypy = "1.3.0"
+mypy = "1.4.1"
 mypy-gitlab-code-quality = "0.0.15"
-types-python-dateutil = "2.8.19.13"
-types-jsonschema = "4.17.0.8"
-pytest = "7.3.2"
+types-python-dateutil = "2.8.19.14"
+types-jsonschema = "4.17.0.10"
+pytest = "7.4.0"
 coverage = "7.2.7"
 toml = "0.10.2"
-typing-extensions = "4.6.3"
+typing-extensions = "4.7.1"
 bandit = "1.7.5"
 isort = "5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

