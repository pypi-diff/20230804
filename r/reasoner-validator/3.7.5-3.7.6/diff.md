# Comparing `tmp/reasoner_validator-3.7.5.tar.gz` & `tmp/reasoner_validator-3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.5.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.6.tar", max compression
```

## Comparing `reasoner_validator-3.7.5.tar` & `reasoner_validator-3.7.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1153 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/LICENSE
--rw-r--r--   0        0        0    12920 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/README.md
--rw-r--r--   0        0        0      131 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/conf.py
--rw-r--r--   0        0        0    19963 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    37242 2023-07-20 22:09:33.051180 reasoner_validator-3.7.5/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2177 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/pyproject.toml
--rw-r--r--   0        0        0    38452 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    78585 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    40494 2023-07-20 22:09:33.055180 reasoner_validator-3.7.5/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/message.py
--rw-r--r--   0        0        0    29675 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11622 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    12532 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/reasoner_validator/versioning.py
--rw-r--r--   0        0        0     1499 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/conftest.py
--rw-r--r--   0        0        0   114915 2023-07-20 22:09:33.059180 reasoner_validator-3.7.5/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    39404 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26808 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_validate.py
--rw-r--r--   0        0        0    21570 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-20 22:09:33.063181 reasoner_validator-3.7.5/tests/test_workflows.py
--rw-r--r--   0        0        0    14907 1970-01-01 00:00:00.000000 reasoner_validator-3.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/LICENSE
+-rw-r--r--   0        0        0    12920 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/README.md
+-rw-r--r--   0        0        0      131 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/conf.py
+-rw-r--r--   0        0        0    20273 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    37242 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2248 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/pyproject.toml
+-rw-r--r--   0        0        0      990 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    83629 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    40494 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/message.py
+-rw-r--r--   0        0        0    26619 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    13885 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1112 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38887 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12532 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0     1477 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/conftest.py
+-rw-r--r--   0        0        0   118956 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40854 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_semver.py
+-rw-r--r--   0        0        0     2278 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27158 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_validate.py
+-rw-r--r--   0        0        0    20409 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-08-04 05:22:07.557872 reasoner_validator-3.7.6/tests/test_workflows.py
+-rw-r--r--   0        0        0    14905 1970-01-01 00:00:00.000000 reasoner_validator-3.7.6/PKG-INFO
```

### Comparing `reasoner_validator-3.7.5/LICENSE` & `reasoner_validator-3.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/README.md` & `reasoner_validator-3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/docs/Makefile` & `reasoner_validator-3.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/docs/conf.py` & `reasoner_validator-3.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/docs/index.rst` & `reasoner_validator-3.7.6/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 Top level programmatic validation of a TRAPI Response uses a TRAPIResponseValidator class wrapper as follows (sample script):
 
 .. code-block:: python
 
     #!/usr/bin/env python
     from typing import Optional, List, Dict
-    from reasoner_validator import TRAPIResponseValidator
+    from reasoner_validator.validator import TRAPIResponseValidator
     from reasoner_validator import MESSAGE_CATALOG
 
     SAMPLE_RESPONSE = {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
@@ -247,24 +247,25 @@
 
     {
         # If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
-        # Otherwise, the TRAPI Response 'schema_version' (not 'latest') becomes the default validation version.
+        # Otherwise, a TRAPI 1.4.0 Response embedded 'schema_version' (not 'latest') becomes the default validation version.
 
         trapi_version="1.4.2",
 
         # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
-        # Otherwise, the TRAPI Response stated 'biolink_version' (not BMT) becomes the default validation version.
+        # Otherwise, a TRAPI 1.4.0 Response embedded 'biolink_version' (not BMT) becomes the default validation version.
+        # The biolink_version may also be set to the string 'suppress', in which case, most Biolink Model validation is NOT done during the validation of a TRAPI Response.
 
         biolink_version="3.5.0",
 
         "sources": {
             "ara_source": "infores:aragorn",
             "kp_source": "infores:panther",
             "kp_source_type": "primary"
@@ -272,16 +273,16 @@
         "strict_validation": true,
         "response": {"some TRAPI Response JSON - see below"}
     }
 
 
 The request body consists of JSON data structure with two top level tag:
 
-* An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases).
-* An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted).
+* An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (if omitted, defaults to 'latest' otherwise; partial SemVer strings are resolved to their 'latest' minor and patch releases).
+* An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (if omitted defaults to 'latest' Biolink Model Toolkit supported version otherwise). Special string value "suppress" disables Biolink Model validation of the TRAPI Response.
 * An **optional** `sources` with an object dictionary (example shown) specifying the ARA and KP sources involved in the TRAPI call (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "sources" or any of the subsidiary tags may be omitted (default to None)
 * An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors.
 * A **mandatory** `response` tag should have as its value the complete TRAPI **Response** JSON data structure to be validated (see example below).
 
 Running the Web Service Directly
 --------------------------------
```

### Comparing `reasoner_validator-3.7.5/docs/make.bat` & `reasoner_validator-3.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.6/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/pyproject.toml` & `reasoner_validator-3.7.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.5"
+version = "3.7.6"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -37,33 +37,34 @@
 include = [
     { path = "tests" },
     { path = "docs" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-bmt = "^1.1.0"
+bmt = "^1.1.1"
+#bmt = { git = "https://github.com/biolink/biolink-model-toolkit.git" }
 
 # jsonschema needs to be pinned to <= 4.18.0 for now,
 # since 4.18.0 appeared to break something for the
 # access and processing of JSON schemata
 jsonschema = "~4.17.3"
 
 PyYAML = "^6.0"
 requests = "^2.28.1"
 pydantic = "^1.10.11"
 urllib3 = "^1.26.15"
 numpydoc = {version = "^1.5.0", optional = true}
-sphinx = {version = "^5.3.0", optional = true}
-myst-parser = {version = "^0.18.1", optional = true}
+sphinx = {version = "^6.2.1", optional = true}
+myst-parser = {version = "^2.0.0", optional = true}
 fastapi = {version = "^0.68", optional = true}
 uvicorn = {version = "^0.15", optional = true}
 pytest-cov = {version = "^4.0.0"}
 pytest = {version = "^7.2.2"}
-sphinx-rtd-theme = {version = "^1.2.1", optional = true}
+sphinx-rtd-theme = {version = "^1.2.2", optional = true}
 
 
 [tool.poetry.urls]
 "Change Log" = "https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/NCATSTranslator/reasoner-validator/issues"
 
 [tool.poetry.extras]
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/__init__.py` & `reasoner_validator-3.7.6/reasoner_validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 from typing import Optional, List, Dict
 
 from bmt import Toolkit
-from reasoner_validator.report import ValidationReporter
+
 from reasoner_validator.biolink import (
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph,
     BMTWrapper,
     BiolinkValidator,
-    get_biolink_model_toolkit,
-    TRAPIGraphType
+    get_biolink_model_toolkit
 )
 
 # Maximum number of data points to scrutinize
 # in various parts TRAPI Query Response.Message
 from reasoner_validator.trapi import (
+    check_trapi_validity,
+    TRAPISchemaValidator, TRAPIGraphType
+)
+from reasoner_validator import (
     TRAPI_1_3_0_SEMVER,
-    TRAPI_1_4_0_SEMVER,
-    TRAPI_1_4_1_SEMVER,
     TRAPI_1_4_0_BETA3_SEMVER,
     TRAPI_1_4_0_BETA4_SEMVER,
-    LATEST_TRAPI_MAJOR_RELEASE_SEMVER,
-    LATEST_TRAPI_RELEASE_SEMVER,
+    TRAPI_1_4_0_SEMVER,
     LATEST_TRAPI_RELEASE,
-    check_trapi_validity,
-    TRAPISchemaValidator
+    LATEST_TRAPI_MAJOR_RELEASE_SEMVER
 )
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
-from reasoner_validator.versioning import SemVer, SemVerError
+from reasoner_validator.versioning import SemVer, SemVerError, get_latest_version
 from reasoner_validator.sri.util import get_aliases
 
 import logging
 logger = logging.getLogger(__name__)
 
+
 # Unspoken assumption here is that validation of results returned for
 # Biolink Model release compliance only needs to be superficial
 RESULT_TEST_DATA_SAMPLE_SIZE = 10
 
 
-class TRAPIResponseValidator(ValidationReporter):
+class TRAPIResponseValidator(BiolinkValidator):
     """
     TRAPI Validator is an overall wrapper class for validating
     conformance of TRAPI Responses to TRAPI and the Biolink Model.
     """
     def __init__(
             self,
+            prefix: Optional[str] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             strict_validation: bool = False,
             suppress_empty_data_warnings: bool = False
     ):
         """
-        :param trapi_version: version of component against which to validate the message (mandatory, no default)
-        :type trapi_version: str
-        :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
-                                validated (Default: if None, use the Biolink Model Toolkit default version).
-        :type biolink_version: Optional[str] = None
-        :param strict_validation: if True, some tests validate as 'error'; None or False, simply issue a 'warning'
-        :type strict_validation: Optional[bool] = None
-        :param suppress_empty_data_warnings: validation normally reports empty Message query graph, knowledge graph
-                       and results as warnings. This flag suppresses the reporting of such warnings (default: False).
-        :type suppress_empty_data_warnings: bool
+        :param prefix: named context of the BiolinkValidator, used as a prefix in validation messages.
+        :param trapi_version: str, version of component against which to validate the message (mandatory, no default)
+        :param biolink_version: Optional[str] = None, Biolink Model (SemVer) release against which the knowledge graph
+                                is to be validated (Default: if None, use the Biolink Model Toolkit default version).
+        :param strict_validation: bool = False, if True, some tests validate as 'error'; False, simply issue a 'warning'
+        :param suppress_empty_data_warnings: bool = False, validation normally reports empty Message query graph,
+                                knowledge graph and results as warnings. This flag suppresses the reporting
+                                of such warnings (default: False).
         """
-        ValidationReporter.__init__(
+        BiolinkValidator.__init__(
             self,
-            prefix="Validate TRAPI Response",
+            # graph_type=None  # not yet resolved
+            prefix=prefix if prefix else "Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             strict_validation=strict_validation
         )
         self._is_trapi_1_4: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
 
@@ -152,19 +152,17 @@
         :type response: Optional[Dict]
         :param max_kg_edges: integer maximum number of edges to be validated from the
                                      knowledge graph of the response. A value of zero triggers validation
                                       of all edges in the knowledge graph (Default: 0 - use all edges)
         :type max_kg_edges: int
         :param max_results: target sample number of results to validate (default: 0 for 'use all results').
         :type max_results: int
-        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :param target_provenance: Dictionary of context identifying the ARA and KP for provenance attribute validation
         :type target_provenance: Dict
 
-        :returns: Validator cataloging "information", "warning" and "error" messages (could be empty)
-        :rtype: ValidationReporter
         """
         if not (response and "message" in response):
             if not self.suppress_empty_data_warnings:
                 self.report("error.trapi.response.empty")
 
             # nothing more to validate?
             return
@@ -173,14 +171,24 @@
         if not message:
             if not self.suppress_empty_data_warnings:
                 self.report("error.trapi.response.message.empty")
 
             # ... also, nothing more here to validate?
             return
 
+        # TRAPI JSON specified versions override default versions
+        if "schema_version" in response and response["schema_version"]:
+            if self.default_trapi:
+                self.trapi_version = get_latest_version(response["schema_version"])
+
+        if "biolink_version" in response and response["biolink_version"]:
+            if self.default_biolink:
+                self.bmt = get_biolink_model_toolkit(biolink_version=response["biolink_version"])
+                self.biolink_version = self.bmt.get_model_version()
+
         response = self.sanitize_trapi_response(response)
 
         trapi_validator: TRAPISchemaValidator = check_trapi_validity(
             instance=response,
             component="Response",
             trapi_version=self.trapi_version
         )
@@ -295,15 +303,15 @@
 
                 if self.validate_biolink():
                     # Conduct validation of Biolink Model compliance
                     # of the Query Graph, if not suppressed...
                     biolink_validator = check_biolink_model_compliance_of_query_graph(
                         graph=query_graph,
                         biolink_version=self.biolink_version,
-                        # the ValidationReporter calling this function *might*
+                        # the TRAPIResponseValidator calling this function *might*
                         # have an explicit strict_validation override (if not None)
                         strict_validation=self.strict_validation
                     )
                     if biolink_validator.has_messages():
                         self.merge(biolink_validator)
                         # 'info' and 'warning' messages do
                         # not fully invalidate the query_graph
@@ -321,15 +329,15 @@
         Validate a TRAPI Knowledge Graph.
 
         :param message: input message expected to contain the 'knowledge_graph'
         :type message: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
                             triggers validation of all edges in the knowledge graph (Default: 0 - use all edges)
         :type edges_limit: int
-        :param target_provenance: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
+        :param target_provenance: Dictionary of context identifying the ARA and KP for provenance attribute validation
         :type target_provenance: Dict
 
         :return: bool, False, if validation errors
         """
         # This integrity constraint may not really be necessary
         # since negative numbers are functionally equivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
@@ -373,15 +381,15 @@
                     # Knowledge Graph, if Biolink validation not suppressed...
                     biolink_validator: BiolinkValidator = \
                         check_biolink_model_compliance_of_knowledge_graph(
                             graph=kg_sample,
                             trapi_version=self.trapi_version,
                             biolink_version=self.biolink_version,
                             target_provenance=target_provenance,
-                            # the ValidationReporter calling this function *might*
+                            # the TRAPIResponseValidator calling this function *might*
                             # have an explicit strict_validation override (if not None)
                             strict_validation=self.strict_validation
                         )
                     if biolink_validator.has_messages():
                         self.merge(biolink_validator)
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.6/reasoner_validator/biolink/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Version-specific Biolink Model semantic validation of knowledge graph components.
 """
-from typing import Optional, Any, Dict, List, Tuple, Set
+from typing import Optional, Any, Dict, List, Tuple
 from sys import stderr
-from enum import Enum
 from functools import lru_cache
 from urllib.error import HTTPError
 from pprint import PrettyPrinter
 
 
 from bmt import Toolkit, utils
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
-from reasoner_validator.message import MESSAGE_CATALOG
 from reasoner_validator.sri.util import is_curie
-from reasoner_validator.report import ValidationReporter
 from reasoner_validator.versioning import SemVer, SemVerError
+from reasoner_validator.message import MESSAGE_CATALOG
+from reasoner_validator.trapi import TRAPISchemaValidator, TRAPIGraphType
 
 import logging
 logger = logging.getLogger(__name__)
 
 pp = PrettyPrinter(indent=4)
 
 
@@ -74,34 +73,42 @@
             logger.error(str(ex))
 
     # 'latest' default Biolink Model
     # version of given Toolkit returned
     return Toolkit()
 
 
-class TRAPIGraphType(Enum):
-    """ Enum type of Biolink Model compliant graph data being validated."""
-    Input_Edge = "Input Edge"
-    Query_Graph = "Query Graph"
-    Knowledge_Graph = "Knowledge Graph"
-
-
 class BMTWrapper:
     def __init__(self, biolink_version: Optional[str] = None):
         self.bmt: Optional[Toolkit] = None
+        self.default_biolink: bool = False
         if biolink_version != "suppress":
             # Here, the Biolink Model version is validated, and the relevant Toolkit pulled.
+            if biolink_version is None:
+                self.default_biolink = True
             self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
-            self.resolved_biolink_version = self.bmt.get_model_version()
+            self.biolink_version = self.bmt.get_model_version()
         else:
-            self.resolved_biolink_version = "suppress"
-        print(f"\nBiolink Model Toolkit Wrapper set to TRAPI Version: '{self.resolved_biolink_version}'", file=stderr)
+            self.biolink_version = "suppress"
+        print(f"\nResolved Biolink Model Version: '{self.biolink_version}'", file=stderr)
+
+    def get_biolink_version(self) -> str:
+        """
+        :return: Biolink Model version currently targeted by the ValidationReporter.
+        :rtype biolink_version: str
+        """
+        return self.biolink_version
 
-    def get_resolved_biolink_version(self) -> Optional[str]:
-        return self.resolved_biolink_version
+    def reset_biolink_version(self, version: str):
+        """
+        Reset Biolink Model version tracked by the ValidationReporter.
+        :param version: new version
+        :return: None
+        """
+        self.biolink_version = version
 
     def get_bmt(self) -> Optional[Toolkit]:
         return self.bmt
 
     def is_symmetric(self, name: str) -> bool:
         """
         Checks if a given element identified by name, is a symmetric (predicate) slot.
@@ -135,49 +142,71 @@
 
             if inverse_predicate_name:
                 ip = self.bmt.get_element(inverse_predicate_name)
                 return utils.format_element(ip)
         return None
 
 
-class BiolinkValidator(ValidationReporter, BMTWrapper):
+class BiolinkValidator(TRAPISchemaValidator, BMTWrapper):
     """
-    Wrapper class for Biolink Model validation.
+    Wrapper class for Biolink Model validation of a TRAPI message.
     """
     def __init__(
         self,
-        graph_type: TRAPIGraphType,
+        graph_type: Optional[TRAPIGraphType] = None,
+        prefix: Optional[str] = None,
         trapi_version: Optional[str] = None,
         biolink_version: Optional[str] = None,
         target_provenance: Optional[Dict[str, str]] = None,
         strict_validation: bool = False
     ):
         """
         Biolink Validator constructor.
 
-        :param graph_type: type of graph data being validated
-        :type graph_type: TRAPIGraphType
-        :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
-        :type trapi_version: Optional[str] or None
-        :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
-        :type biolink_version: Optional[str] or None
-        :param target_provenance: Dictionary of context identifying the ARA and KP for provenance attribute validation
-        :type target_provenance: Optional[Dict[str,str]]
+        :param graph_type: Optional[TRAPIGraphType] == None, type of graph data being validated (if already known)
+        :param prefix: named context of the BiolinkValidator, used as a prefix in validation messages.
+        :param trapi_version:  Optional[str], caller specified Biolink Model version (default: None, use TRAPI 'latest')
+        :param biolink_version: Optional[str], caller specified Biolink Model version (default: None, use BMT 'latest')
+        :param target_provenance: Optional[Dict[str,str]], Dictionary of context ARA and KP for provenance validation
+        :param strict_validation: bool, applies stricter constraints on Biolink class term semantics
         """
         BMTWrapper.__init__(self, biolink_version=biolink_version)
-        ValidationReporter.__init__(
+        TRAPISchemaValidator.__init__(
             self,
-            prefix=f"Biolink Validation of {graph_type.value}",
+            prefix=prefix if prefix else f"Biolink Validation of {graph_type.value}",
             trapi_version=trapi_version,
-            biolink_version=self.get_resolved_biolink_version(),
             strict_validation=strict_validation
         )
         self.target_provenance: Optional[Dict] = target_provenance
         self.graph_type: TRAPIGraphType = graph_type
-        self.nodes: Set[str] = set()
+        self.nodes: Dict[str, List[str]] = dict()
+
+    def get_biolink_version(self) -> str:
+        """
+        :return: Biolink Model version currently tracked by the TRAPISchemaValidator.
+        :rtype biolink_version: str
+        """
+        return BMTWrapper.get_biolink_version(self)
+
+    def reset_biolink_version(self, version: str):
+        """
+        Reset Biolink Model version tracked by the ValidationReporter.
+        :param version: new version
+        :return: None
+        """
+        BMTWrapper.reset_biolink_version(self, version)
+
+    def validate_biolink(self) -> bool:
+        """
+        Predicate to check if the Biolink (version) is
+        tagged to 'suppress' compliance validation.
+
+        :return: bool, returns 'True' if Biolink Validation is expected.
+        """
+        return self.biolink_version is not None and self.biolink_version.lower() != "suppress"
 
     def minimum_required_biolink_version(self, version: str) -> bool:
         """
         :param version: simple 'major.minor.patch' Biolink Model SemVer
         :return: True if current version is equal to, or newer than, a targeted 'minimum_version'
         """
         try:
@@ -341,16 +370,43 @@
                 if is_set and not isinstance(is_set, bool):
                     self.report(code="error.query_graph.node.is_set.not_boolean", identifier=node_id)
             # else:  # a missing key or null "is_set" value is permitted in QNodes but defaults to 'False'
 
             # constraints  # TODO: how do we validate node constraints?
             pass
 
-    def set_nodes(self, nodes: Set):
-        self.nodes.update(nodes)
+    def set_nodes(self, nodes: Dict):
+        """
+        Records additional nodes, uniquely by node_id, with specified categories.
+        :param nodes: Dict, node_id indexed node categories
+        :return: None
+        """
+        # TODO: node_id keys of nodes assumed to be unique, thus
+        #       nodes should never overwrite previously seen nodes?
+        self.nodes.update(
+            {
+                node_id: details['categories']
+                if 'categories' in details and details['categories'] else ['biolink:NamedThing']
+                for node_id, details in nodes.items()
+            }
+        )
+
+    def get_node_identifiers(self) -> List[str]:
+        """
+        :return: List of currently registered node_ids
+        """
+        return list(self.nodes.keys())
+
+    def get_node_categories(self, node_id: str) -> Optional[List[str]]:
+        """
+        Categories by 'node_id'.
+        :param node_id:
+        :return: For a given node_id, returns the associated categories; None if node_id is currently unknown
+        """
+        return self.nodes[node_id] if node_id in self.nodes else None
 
     def validate_element_status(
             self,
             context: str,
             identifier: str,
             edge_id: str,
             source_trail: Optional[str] = None
@@ -524,15 +580,15 @@
         :return: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         """
         # in TRAPI 1.4.0, the source_trail is parsed in from the Edge.sources annotation, hence
         # the source_trail is already known and given to this method for reporting purposes here
 
         # Otherwise, in TRAPI 1.3.0, the 'sources' may be compiled here, in this method, from the attributes
         # themselves, then a newly generated 'source_trail', returned for use by the rest of the application
-        sources: Dict[str, List[str]] = dict()
+        # sources: Dict[str, List[str]] = dict()
 
         # we only report errors about missing or empty edge attributes if TRAPI 1.3.0 or earlier,
         # and Biolink Validation is not suppressed, since we can't fully validate provenance and
         # since earlier TRAPI releases are minimally expected to record provenance attributes
         # we only report this for TRAPI < 1.4 when Biolink Validation is done given that
         # without Biolink validation, provenance cannot be reliably assessed
 
@@ -737,25 +793,34 @@
             return  # nullable: true... missing key or None value is ok?
         elif not isinstance(edge['attribute_constraints'], List):
             self.report(code="error.query_graph.edge.attribute_constraints.not_array", identifier=edge_id)
         elif not edge['attribute_constraints']:
             return  # nullable: true... an empty 'attribute_constraints' array is ok?
         else:
             # TODO: not yet sure what else to do here (if anything...yet)
-            attribute_constraints: List = edge['attribute_constraints']
+            # attribute_constraints: List = edge['attribute_constraints']
+            pass
 
-    def validate_qualifier_entry(self, context: str, edge_id: str, qualifiers: List[Dict[str, str]]):
+    def validate_qualifier_entry(
+            self,
+            context: str,
+            edge_id: str,
+            qualifiers: List[Dict[str, str]],
+            associations: Optional[List[str]] = None
+    ):
         """
         Validate Qualifier Entry (JSON Object).
 
         :param context: str, Validation (subcode) context:
                         - query graph qualifier constraints ("query_graph.edge.qualifier_constraints.qualifier_set") or
                         - knowledge graph edge qualifiers (knowledge_graph.edge.qualifiers)
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param qualifiers: List[Dict[str, str]], of qualifier entries to be validated.
+        :param associations: Optional[List[str]] = None,
+                             Biolink association subclasses possibly related to the current edge.
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
         """
         for qualifier in qualifiers:
             qualifier_type_id: str = qualifier['qualifier_type_id']
             qualifier_value: str = qualifier['qualifier_value']
             try:
                 if not self.bmt.is_qualifier(name=qualifier_type_id):
@@ -771,19 +836,20 @@
                             code=f"error.{context}.qualifier.value.not_a_predicate",
                             identifier=qualifier_value,
                             edge_id=edge_id
                         )
 
                 # A Query Graph miss on qualifier_value is less an issue since there may not be enough
                 # context to resolve the 'qualifier_value'; whereas a Knowledge Graph miss is more severe
-                # TODO: however, we somehow need to leverage TRAPI MetaEdge.association metadata here?
-                elif context.startswith("knowledge_graph") and not self.bmt.validate_qualifier(
-                        qualifier_type_id=qualifier_type_id,
-                        qualifier_value=qualifier_value
-                ):
+                elif context.startswith("knowledge_graph") and \
+                        not self.bmt.validate_qualifier(
+                            qualifier_type_id=qualifier_type_id,
+                            qualifier_value=qualifier_value,
+                            associations=associations
+                        ):
                     self.report(
                         code=f"error.{context}.qualifier.value.unresolved",
                         identifier=qualifier_value,
                         edge_id=edge_id,
                         qualifier_type_id=qualifier_type_id
                     )
             except Exception as e:
@@ -793,20 +859,26 @@
                     code=f"error.{context}.qualifier.invalid",
                     identifier=edge_id,
                     qualifier_type_id=qualifier_type_id,
                     qualifier_value=qualifier_value,
                     reason=str(e)
                 )
 
-    def validate_qualifiers(self, edge_id: str, edge: Dict):
+    def validate_qualifiers(
+            self,
+            edge_id: str,
+            edge: Dict,
+            associations: Optional[List[str]] = None
+    ):
         """
         Validate Knowledge Edge Qualifiers.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
+        :param associations: Optional[List[str]], Biolink association subclasses possibly related to the current edge.
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
         """
         # Edge qualifiers will only be seen in Biolink 3 data,
         # but with missing 'qualifiers', no validation is attempted
         if 'qualifiers' not in edge or edge['qualifiers'] is None:
             return  # nullable: true... missing key or None value is ok?
         elif not isinstance(edge['qualifiers'], List):
@@ -814,18 +886,23 @@
         elif not edge['qualifiers']:
             return  # nullable: true... an empty 'qualifiers' array is ok?
         elif self.validate_biolink():
             qualifiers: List = edge['qualifiers']
             self.validate_qualifier_entry(
                 context="knowledge_graph.edge.qualifiers",
                 edge_id=edge_id,
-                qualifiers=qualifiers
+                qualifiers=qualifiers,
+                associations=associations
             )
 
-    def validate_qualifier_constraints(self, edge_id: str, edge: Dict):
+    def validate_qualifier_constraints(
+            self,
+            edge_id: str,
+            edge: Dict
+    ):
         """
         Validate Query Edge Qualifier Constraints.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
         """
@@ -1178,18 +1255,20 @@
         :param edge: dictionary of slot properties of the edge.
         :type edge: dict[str, str]
         """
         # logger.debug(edge)
         # edge data fields to be validated...
         subject_id = edge['subject'] if 'subject' in edge else None
 
-        predicates = predicate = None
+        predicates: Optional[List[str]]
+        predicate: Optional[str] = None
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
             predicate = edge['predicate'] if 'predicate' in edge else None
             edge_label = predicate
+            predicates = [predicate]
         else:
             # Query Graph...
             predicates = edge['predicates'] if 'predicates' in edge else None
             edge_label = str(predicates)
 
         object_id = edge['object'] if 'object' in edge else None
 
@@ -1204,18 +1283,31 @@
         # for reasoner-validator issue#86 - edge sources reporting.
         #
         # Validate edge attributes (or attribute_constraints)
         # and (Biolink) edge qualifiers (or qualifier_constraints)
         source_trail: Optional[str] = None
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
 
+            associations: Optional[List[str]] = None
+            if self.validate_biolink():
+                # We need to look up the biolink:Association subclass
+                # matching the subject and object categories of the edge
+                subject_categories: Optional[List[str]] = self.get_node_categories(node_id=subject_id)
+                object_categories: Optional[List[str]] = self.get_node_categories(node_id=object_id)
+                associations = self.bmt.get_associations(
+                    subject_categories=subject_categories,
+                    predicates=predicates,
+                    object_categories=object_categories,
+                    formatted=True
+                )
+
             # Edge "qualifiers" field is only recorded as an
             # Edge property, from TRAPI 1.3.0-beta onwards
             if self.minimum_required_trapi_version("1.3.0-beta"):
-                self.validate_qualifiers(edge_id=edge_id, edge=edge)
+                self.validate_qualifiers(edge_id=edge_id, edge=edge, associations=associations)
 
             # Edge provenance "sources" field is only recorded
             # as an Edge property, from TRAPI 1.4.0-beta onwards
             if self.minimum_required_trapi_version("1.4.0-beta"):
                 # For TRAPI 1.4.0, the 'source_trail' is parsed in by 'validate_sources'...
                 source_trail = self.validate_sources(edge_id=edge_id, edge=edge)
 
@@ -1223,14 +1315,15 @@
                 #    to 'validate_attributes' for use in attribute validation reporting
                 self.validate_attributes(edge_id=edge_id, edge=edge, source_trail=source_trail)
             else:
                 # For TRAPI 1.3.0, the 'sources' are discovered internally by 'validate_attributes'
                 # and the resulting source_trail returned, for further external reporting purposes
                 source_trail = self.validate_attributes(edge_id=edge_id, edge=edge)
         else:
+            # NOT a Knowledge Graph edge validation
             self.validate_attribute_constraints(edge_id=edge_id, edge=edge)
 
             # Edge "qualifiers" field is only recorded as an
             # Edge property, from TRAPI 1.3.0-beta onwards
             # We don't care about 'source_trail' here, for the Query Graph edges
             if self.minimum_required_trapi_version("1.3.0-beta"):
                 self.validate_qualifier_constraints(edge_id=edge_id, edge=edge)
@@ -1239,15 +1332,15 @@
         if not subject_id:
             self.report(
                 code=f"error.{context}.edge.subject.missing",
                 source_trail=source_trail,
                 identifier=edge_id
             )
 
-        elif subject_id not in self.nodes:
+        elif subject_id not in self.get_node_identifiers():
             self.report(
                 code=f"error.{context}.edge.subject.missing_from_nodes",
                 source_trail=source_trail,
                 identifier=subject_id,
                 edge_id=edge_id
             )
 
@@ -1298,15 +1391,15 @@
         # Validate Object Node
         if not object_id:
             self.report(
                 code=f"error.{context}.edge.object.missing",
                 source_trail=source_trail,
                 identifier=edge_id
             )
-        elif object_id not in self.nodes:
+        elif object_id not in self.get_node_identifiers():
             self.report(
                 code=f"error.{context}.edge.object.missing_from_nodes",
                 source_trail=source_trail,
                 identifier=object_id,
                 edge_id=edge_id
             )
 
@@ -1479,25 +1572,57 @@
         else:
             if self.graph_type is not TRAPIGraphType.Query_Graph:
                 self.report(code="error.knowledge_graph.edges.empty")
             # else:  Query Graphs can omit the 'edges' tag
             edges = None
 
         if nodes:
+
             for node_id, details in nodes.items():
                 self.validate_graph_node(node_id, details)
 
-            # Needed for the subsequent edge validation
-            self.set_nodes(set(nodes.keys()))
+            # The instances of 'node_id' and associated 'categories'
+            # are needed for the subsequent edge validation processes
+            self.set_nodes(nodes)
 
             if edges:
                 for edge in edges.values():
                     # print(f"{str(edge)}", flush=True)
                     self.validate_graph_edge(edge)
 
+    def merge(self, reporter):
+        """
+        Merge all messages and metadata from a second BiolinkValidator,
+        into the calling TRAPISchemaValidator instance.
+
+        :param reporter: second BiolinkValidator
+        """
+        TRAPISchemaValidator.merge(self, reporter)
+
+        # First come, first serve... We only overwrite
+        # empty versions in the parent reporter
+        if isinstance(reporter, BiolinkValidator) and not self.get_biolink_version():
+            self.reset_biolink_version(reporter.get_biolink_version())
+
+    def to_dict(self) -> Dict:
+        """
+        Export BiolinkValidator contents as a Python dictionary
+        (including Biolink version and parent class dictionary content).
+        :return: Dict
+        """
+        dictionary = TRAPISchemaValidator.to_dict(self)
+        dictionary["biolink_version"] = self.get_biolink_version()
+        return dictionary
+
+    def report_header(self, title: Optional[str], compact_format: bool) -> str:
+        header: str = TRAPISchemaValidator.report_header(self, title, compact_format)
+        header += "and Biolink Model version " \
+                  f"'{str(self.get_biolink_version() if self.get_biolink_version() is not None else 'Default')}'"
+        return header
+
 
 def check_biolink_model_compliance_of_input_edge(
         edge: Dict[str, str],
         biolink_version: Optional[str] = None,
         strict_validation: Optional[bool] = None
 ) -> BiolinkValidator:
     """
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.6/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/reasoner_validator/message.py` & `reasoner_validator-3.7.6/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/reasoner_validator/report.py` & `reasoner_validator-3.7.6/reasoner_validator/report.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Error and Warning Reporting Module"""
 from typing import Optional, Dict, List
-from sys import stdout, stderr
+from sys import stdout
 from importlib import metadata
 from io import StringIO
 import copy
 
 from json import dumps, JSONEncoder
 
 from reasoner_validator.message import (
     MESSAGE_CATALOG,
     MESSAGE_PARTITION,
     SCOPED_MESSAGES,
     IDENTIFIED_MESSAGES,
     MESSAGE_PARAMETERS
 )
 from reasoner_validator.validation_codes import CodeDictionary
-from reasoner_validator.versioning import SemVer, SemVerError, get_latest_version
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class ReportJsonEncoder(JSONEncoder):
     def default(self, o):
@@ -51,84 +50,31 @@
     _message_type_name: Dict[str, str] = {
         "info": "information",
         "warning": "warnings",
         "error": "errors",
         "critical": "critical"
     }
 
-    def __init__(
-            self,
-            prefix: Optional[str] = None,
-            trapi_version: Optional[str] = None,
-            biolink_version: Optional[str] = None,
-            strict_validation: bool = False
-    ):
+    def __init__(self, prefix: Optional[str] = None, strict_validation: bool = False):
         """
         :param prefix: named context of the Validator, used as a prefix in validation messages.
         :type prefix: str
-        :param trapi_version: version of component against which to validate the message.
-                              Could be a TRAPI release SemVer or a Git branch identifier.
-        :type trapi_version: Optional[str], target version of TRAPI upon which the validation is attempted
-        :param biolink_version: Biolink Model (SemVer) release against which the knowledge graph is to be
-                                validated (Default: if None, use the Biolink Model Toolkit default version).
-        :type biolink_version: Optional[str] = None
         :param strict_validation: if True, abstract and mixin elements validate as 'error';
                                   if None or False, just issue a 'warning'
         :type strict_validation: Optional[bool] = None
         """
         self.prefix: str = prefix if prefix else ""
-
-        self.trapi_version = get_latest_version(trapi_version) \
-            if trapi_version else get_latest_version(self.DEFAULT_TRAPI_VERSION)
-        print(f"\nValidationReporter set to TRAPI Version: '{self.trapi_version}'", file=stderr)
-
-        self.biolink_version = biolink_version
         self.strict_validation: Optional[bool] = strict_validation
         self.messages: MESSAGE_CATALOG = {
             "critical": dict(),
             "errors": dict(),
             "warnings": dict(),
             "information": dict()
         }
 
-    def get_trapi_version(self) -> str:
-        """
-        :return: str, TRAPI (SemVer) version currently targeted by the ValidationReporter.
-        """
-        return self.trapi_version
-
-    def minimum_required_trapi_version(self, version: str) -> bool:
-        """
-        :param version: simple 'major.minor.patch' TRAPI schema release SemVer
-        :return: True if current version is equal to, or newer than, a targeted 'minimum_version'
-        """
-        try:
-            current: SemVer = SemVer.from_string(self.trapi_version)
-            target: SemVer = SemVer.from_string(version)
-            return current >= target
-        except SemVerError as sve:
-            logger.error(f"minimum_required_trapi_version() error: {str(sve)}")
-            return False
-
-    def get_biolink_version(self) -> str:
-        """
-        :return: Biolink Model version currently targeted by the ValidationReporter.
-        :rtype biolink_version: str
-        """
-        return self.biolink_version
-
-    def validate_biolink(self) -> bool:
-        """
-        Predicate to check if the Biolink (version) is
-        tagged to 'suppress' compliance validation.
-
-        :return: bool, returns 'True' if Biolink Validation is expected.
-        """
-        return self.biolink_version is None or self.biolink_version.lower() != "suppress"
-
     def is_strict_validation(self) -> bool:
         """
         :return: bool, value of validation strictness set in the ValidationReporter.
         """
         return self.strict_validation
 
     def has_messages(self) -> bool:
@@ -334,32 +280,20 @@
         :param reporter: second ValidationReporter
         """
         assert isinstance(reporter, ValidationReporter)
 
         # new coded messages also need to be merged!
         self.add_messages(reporter.get_messages())
 
-        # First come, first serve... We only overwrite
-        # empty versions in the parent reporter
-        if not self.trapi_version:
-            self.trapi_version = reporter.trapi_version
-        if not self.biolink_version:
-            self.biolink_version = reporter.biolink_version
-
     def to_dict(self) -> Dict:
         """
-        Export ValidationReporter contents as a Python dictionary
-        (including TRAPI version, Biolink Model version and messages)
+        Export ValidationReporter message contents as a Python dictionary.
         :return: Dict
         """
-        return {
-            "trapi_version": self.trapi_version,
-            "biolink_version": self.biolink_version,
-            "messages": self.get_messages()
-        }
+        return {"messages": self.get_messages()}
 
     def apply_validation(self, validation_method, *args, **kwargs) -> bool:
         """
         Wrapper to allow validation_methods direct access to the ValidationReporter.
 
         :param validation_method: function which accepts this instance of the
                ValidationReporter as its first argument, for use in reporting validation errors.
@@ -384,16 +318,15 @@
         :return: True if the case contains validation messages
         """
         # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
         #
         # The 'case' dictionary object could have a format something like this:
         #
         #     tag: {
-        #         "trapi_version": "1.3",
-        #         "biolink_version": "3.0.2",
+        #         ...
         #         "messages": {
         #             "information": [],
         #             "warnings": [
         #                 {
         #                     "warning.predicate.non_canonical": {
         #                         "infores:molepro -> infores:arax": {  # local source scope of error
         #                             "biolink:participates_in": {
@@ -428,14 +361,37 @@
                     'errors' in case[tag]['messages'] and case[tag]['messages']['errors'] or
                     'critical' in case[tag]['messages'] and case[tag]['messages']['critical']
                 ):
             return True
         else:
             return False
 
+    def report_header(self, title: Optional[str], compact_format: bool) -> str:
+        header: str = ""
+        if title is not None:
+
+            if not compact_format:
+                header += "\n"
+
+            if not title:
+                title = f"Validation Report"
+                title += f" for '{self.prefix}'" if self.prefix else ""
+
+            if not compact_format:
+                header += f"\n\033[4m{title}\033[0m\n"
+            else:
+                # compact also ignores underlining
+                header += f"{title}\n"
+
+        if not compact_format:
+            header += "\n"
+
+        header += f"Reasoner Validator version '{metadata.version('reasoner-validator')}'"
+        return header
+
     def dump(
             self,
             title: Optional[str] = "",
             id_rows: int = 0,
             msg_rows: int = 0,
             compact_format: bool = False,
             file=stdout
@@ -454,37 +410,15 @@
                                also, suppress character escapes (i.e. underlining of titles) (default: False)
         :param file: target file device for output
         :return: n/a
         """
         assert id_rows >= 0, "dump(): 'id_rows' argument must be positive or equal to zero"
         assert msg_rows >= 0, "dump(): 'pm_rows' argument must be positive or equal to zero"
 
-        if title is not None:
-
-            if not compact_format:
-                print(file=file)
-
-            if not title:
-                title = f"Validation Report"
-                title += f" for '{self.prefix}'" if self.prefix else ""
-
-            if not compact_format:
-                print(f"\n\033[4m{title}\033[0m", file=file)
-                print(file=file)
-            else:
-                # compact also ignores underlining
-                print(title, file=file)
-
-        print(
-            f"Reasoner Validator version '{metadata.version('reasoner-validator')}' validating against "
-            f"TRAPI schema version '{str(self.trapi_version if self.trapi_version is not None else 'Default')}' " +
-            "and Biolink Model version " +
-            f"'{str(self.biolink_version if self.biolink_version is not None else 'Default')}'.\n",
-            file=file
-        )
+        print(f"{self.report_header(title, compact_format)}.\n", file=file)
 
         if self.has_messages():
 
             # self.messages is a MESSAGE_CATALOG where MESSAGE_CATALOG is Dict[<message type>, MESSAGE_PARTITION]
             # <message type> is the top level partition of messages into 'critical', 'error', 'warning' or 'info'
             message_type: str
             coded_messages: MESSAGE_PARTITION
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.6/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.6/reasoner_validator/trapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,40 @@
 """TRAPI Validation Functions."""
+from enum import Enum
 from json import dumps
 from typing import Optional, Dict, List
+from sys import stderr
 from os.path import isfile
 import copy
 from functools import lru_cache
 
 import jsonschema
 import requests
 
 from yaml import load, CLoader as Loader
 
+from reasoner_validator import (
+    TRAPI_1_4_0_BETA_SEMVER,
+    TRAPI_1_4_0_BETA3_SEMVER,
+    TRAPI_1_4_0_BETA4_SEMVER,
+    TRAPI_1_4_0_SEMVER
+)
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.trapi.mapping import check_node_edge_mappings
 from reasoner_validator.versioning import (
     SemVer,
     SemVerError,
     get_latest_version,
     GIT_ORG,
     GIT_REPO
 )
 
 import logging
 logger = logging.getLogger(__name__)
 
-TRAPI_1_3_0_SEMVER = SemVer.from_string("v1.3.0")
-TRAPI_1_3_0: str = str(TRAPI_1_3_0_SEMVER)
-
-TRAPI_1_4_0_BETA_SEMVER = SemVer.from_string("v1.4.0-beta")
-TRAPI_1_4_0_BETA = str(TRAPI_1_4_0_BETA_SEMVER)
-
-TRAPI_1_4_0_BETA2_SEMVER = SemVer.from_string("v1.4.0-beta2")
-TRAPI_1_4_0_BETA3_SEMVER = SemVer.from_string("v1.4.0-beta3")
-TRAPI_1_4_0_BETA4_SEMVER = SemVer.from_string("v1.4.0-beta4")
-
-TRAPI_1_4_0_SEMVER = SemVer.from_string("v1.4.0")
-TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
-
-# patch version to fix 'auxiliary_graphs' model in 1.4.0
-TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
-TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
-
-# patch version to fix '#components/schemas/AuxiliaryGraph' bug
-TRAPI_1_4_2_SEMVER = SemVer.from_string("v1.4.2")
-TRAPI_1_4_2: str = str(TRAPI_1_4_2_SEMVER)
-
-LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_2_SEMVER
-LATEST_TRAPI_RELEASE: str = TRAPI_1_4_2
-
-LATEST_TRAPI_MAJOR_RELEASE_SEMVER: SemVer = SemVer.from_string("v1.4", core_fields=['major', 'minor'])
-LATEST_TRAPI_MAJOR_RELEASE: str = str(LATEST_TRAPI_MAJOR_RELEASE_SEMVER)
-
 # For testing, set TRAPI API query POST timeouts to 10 minutes == 600 seconds
 DEFAULT_TRAPI_POST_TIMEOUT = 600.0
 
 
 class TRAPIAccessError(RuntimeError):
     pass
 
@@ -213,15 +194,15 @@
 
     # we'll only tweak mapped schemata and
     # such releases that are prior to TRAPI 1.4.0-beta
     if (
             mapped_semver and
             not (TRAPI_1_4_0_BETA4_SEMVER >= mapped_semver >= TRAPI_1_4_0_BETA_SEMVER)
     ) and "allOf" in schema:
-        # September 1, 2022 hacky patch to rewrite 'allOf'
+        # 2022 September 1 hacky patch to rewrite 'allOf'
         # tagged schemata, in TRAPI 1.3.0 or earlier, to 'oneOf'
         schema["oneOf"] = schema.pop("allOf")
 
     if schema.get("type", None) == "object":
         for tag, prop in schema.get("properties", dict()).items():
             patch_schema(tag, prop, version)
             openapi_to_jsonschema(prop, version=version)
@@ -229,37 +210,78 @@
     elif schema.get("type", None) == "array":
         openapi_to_jsonschema(schema.get("items", dict()), version=version)
 
     if schema.pop("nullable", False):
         fix_nullable(schema)
 
 
+class TRAPIGraphType(Enum):
+    """ Enum type of Biolink Model compliant graph data being validated."""
+    Input_Edge = "Input Edge"
+    Query_Graph = "Query Graph"
+    Knowledge_Graph = "Knowledge Graph"
+
+
 class TRAPISchemaValidator(ValidationReporter):
     """
     TRAPI Validator is a wrapper class for validating
     conformance of JSON messages to the Translator Reasoner API.
     """
     def __init__(
             self,
-            trapi_version: Optional[str] = None
+            prefix: Optional[str] = None,
+            trapi_version: Optional[str] = None,
+            strict_validation: bool = False
     ):
         """
         TRAPI Validator constructor.
 
-        Parameters
-        ----------
-        trapi_version : str
-            version of component to validate against
+        :param prefix: str named context of the TRAPISchemaValidator, used as a prefix in validation messages.
+        :param trapi_version: str, version of component to validate against
+        :param strict_validation: bool, applies stricter constraints on Biolink class term semantics
         """
+        self.default_trapi: bool = False
+        if trapi_version is None:
+            self.default_trapi = True
+        self.trapi_version = get_latest_version(trapi_version) \
+            if trapi_version else get_latest_version(self.DEFAULT_TRAPI_VERSION)
+        print(f"\nTRAPISchemaValidator set to TRAPI Version: '{self.trapi_version}'", file=stderr)
         ValidationReporter.__init__(
             self,
-            prefix="TRAPI Validation",
-            trapi_version=trapi_version
+            prefix=prefix if prefix is not None else "TRAPI Validation",
+            strict_validation=strict_validation
         )
 
+    def get_trapi_version(self) -> str:
+        """
+        :return: str, TRAPI (SemVer) version currently targeted by the TRAPISchemaValidator.
+        """
+        return self.trapi_version
+
+    def reset_trapi_version(self, version: str):
+        """
+        Reset TRAPI version tracked by the TRAPISchemaValidator.
+        :param version: new version
+        :return: None
+        """
+        self.trapi_version = version
+
+    def minimum_required_trapi_version(self, version: str) -> bool:
+        """
+        :param version: simple 'major.minor.patch' TRAPI schema release SemVer
+        :return: True if current version is equal to, or newer than, a targeted 'minimum_version'
+        """
+        try:
+            current: SemVer = SemVer.from_string(self.trapi_version)
+            target: SemVer = SemVer.from_string(version)
+            return current >= target
+        except SemVerError as sve:
+            logger.error(f"minimum_required_trapi_version() error: {str(sve)}")
+            return False
+
     def validate(self, instance, component):
         """Validate instance against schema.
 
         Parameters
         ----------
         instance
             dict, instance to validate
@@ -312,14 +334,44 @@
             self.report(
                 code="critical.trapi.validation",
                 identifier=self.trapi_version,
                 component=component,
                 reason=reason
             )
 
+    def merge(self, reporter):
+        """
+        Merge all messages and metadata from a second TRAPISchemaValidator,
+        into the calling TRAPISchemaValidator instance.
+
+        :param reporter: second TRAPISchemaValidator
+        """
+        ValidationReporter.merge(self, reporter)
+
+        # First come, first serve... We only overwrite
+        # empty versions in the parent reporter
+        if isinstance(reporter, TRAPISchemaValidator) and not self.get_trapi_version():
+            self.reset_trapi_version(reporter.get_trapi_version())
+
+    def to_dict(self) -> Dict:
+        """
+        Export TRAPISchemaValidator contents as a Python dictionary
+        (including TRAPI version and parent class dictionary content)
+        :return: Dict
+        """
+        dictionary = ValidationReporter.to_dict(self)
+        dictionary["trapi_version"] = self.get_trapi_version()
+        return dictionary
+
+    def report_header(self, title: Optional[str], compact_format: bool) -> str:
+        header: str = ValidationReporter.report_header(self, title, compact_format)
+        header += f" validating against TRAPI version " \
+                  f"'{str(self.get_trapi_version() if self.get_trapi_version() is not None else 'Default')}'"
+        return header
+
 
 def check_trapi_validity(instance, trapi_version: str, component: str = "Query") -> TRAPISchemaValidator:
     """
     Checks schema compliance of a Query component against a given TRAPI version.
 
     Parameters
     ----------
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.6/reasoner_validator/trapi/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from reasoner_validator import ValidationReporter
+from reasoner_validator.report import ValidationReporter
 
 
 class MappingValidator(ValidationReporter):
     """
     The Mapping Validator is a wrapper class for detecting
     dangling references between nodes and edges of a graph.
     This is more of a TRAPI expectation (that all nodes and edges identifiers refer to one another)
```

### Comparing `reasoner_validator-3.7.5/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.6/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/reasoner_validator/versioning.py` & `reasoner_validator-3.7.6/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/tests/__init__.py` & `reasoner_validator-3.7.6/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from typing import Tuple, List
 from sys import stderr
 from os.path import abspath, dirname, sep
 from copy import deepcopy
 
-from reasoner_validator.trapi import (
-    TRAPI_1_3_0,
-    LATEST_TRAPI_MAJOR_RELEASE,
-    LATEST_TRAPI_RELEASE
-)
+from reasoner_validator import TRAPI_1_3_0, LATEST_TRAPI_RELEASE, LATEST_TRAPI_MAJOR_RELEASE
 
 TESTS_DIRECTORY = abspath(dirname(__file__))
 print(f"Test Directory: {TESTS_DIRECTORY}", file=stderr)
 
 PATCHED_SCHEMA_VERSION = "v1.4.0-beta5"
 PATCHED_140_SCHEMA_FILEPATH = f"{TESTS_DIRECTORY}{sep}test_data{sep}patched_trapi_schema_{PATCHED_SCHEMA_VERSION}.yaml"
 BROKEN_SCHEMA_FILEPATH = f"broken-{PATCHED_SCHEMA_VERSION}.yaml"
```

### Comparing `reasoner_validator-3.7.5/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.6/tests/test_biolink_compliance_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 from copy import deepcopy
 from pprint import PrettyPrinter
 import logging
 import pytest
 from bmt import Toolkit
 from linkml_runtime.linkml_model import SlotDefinition
 
-from reasoner_validator import TRAPISchemaValidator
-from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_0_BETA, LATEST_TRAPI_RELEASE
+from reasoner_validator import TRAPI_1_3_0, TRAPI_1_4_0_BETA
 from reasoner_validator.biolink import (
-    TRAPIGraphType,
     BiolinkValidator,
     get_biolink_model_toolkit,
     check_biolink_model_compliance_of_input_edge,
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph
 )
+from reasoner_validator.trapi import TRAPIGraphType
 from tests import SIMPLE_SAMPLE_NODES, SAMPLE_NODES_WITH_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 pp = PrettyPrinter(indent=4)
@@ -38,26 +37,31 @@
 SUPPRESS_BIOLINK_MODEL_VALIDATION = "suppress"
 
 
 def test_set_default_biolink_versioned_global_environment():
     validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
     model_version = validator.get_biolink_version()
     print(
-        f"\ntest_set_default_global_environment(): Biolink Model version is: '{str(model_version)}'",
+        f"\nBiolinkValidator set to (default) Biolink Model version: '{str(model_version)}'",
         file=stderr, flush=True
     )
     assert model_version == Toolkit().get_model_version()
 
 
 def test_set_specific_biolink_versioned_global_environment():
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         biolink_version="1.8.2"
     )
-    assert validator.get_biolink_version() == "1.8.2"
+    model_version = validator.get_biolink_version()
+    print(
+        f"\nBiolinkValidator set to (explicit) Biolink Model version: '{str(model_version)}'",
+        file=stderr, flush=True
+    )
+    assert model_version == "1.8.2"
 
 
 def test_minimum_required_biolink_version():
     # Setting Validator to BLM release 2.2.0
     validator = BiolinkValidator(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         biolink_version="2.2.0"
@@ -66,14 +70,33 @@
     assert validator.minimum_required_biolink_version("1.8.2")
     # 2.2.0 >= 2.2.0 - True!
     assert validator.minimum_required_biolink_version("2.2.0")
     # 2.2.0 >= 2.4.8 - False!
     assert not validator.minimum_required_biolink_version("2.4.8")
 
 
+def test_message():
+    reporter = BiolinkValidator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
+        prefix="Test Message",
+        trapi_version="v1.3",
+        biolink_version="v3.5.2"
+    )
+    assert reporter.get_trapi_version() == "v1.3.0"
+
+    # Note: BMT is a bit tricky in resolving Biolink Model versions:
+    # the version is reported without the 'v' prefix of the Github release!
+    assert reporter.get_biolink_version() == "3.5.2"
+
+    assert not reporter.has_messages()
+    reporter.report("info.compliant")
+    assert reporter.has_messages()
+    reporter.dump()
+
+
 def test_inverse_predicate():
     tk: Toolkit = get_biolink_model_toolkit("2.2.0")
     predicate = tk.get_element("biolink:related_to")
     assert predicate['symmetric']
     predicate = tk.get_element("biolink:active_in")
     assert not predicate['symmetric']
     assert isinstance(predicate, SlotDefinition)
@@ -355,15 +378,15 @@
 )
 def test_check_biolink_model_compliance_of_input_edge(query: Tuple):
     validator: BiolinkValidator = check_biolink_model_compliance_of_input_edge(edge=query[1], biolink_version=query[0])
     check_messages(validator, query[2])
 
 
 @pytest.mark.parametrize(
-    "query",
+    "biolink_version,graph",
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 0: Sample small valid TRAPI Query Graph
             {
                 "edges": {
                     "t_edge": {
@@ -420,21 +443,21 @@
                         "object": "type-2 diabetes"
                     }
                 }
             }
         )
     ]
 )
-def test_conservation_of_query_graph(query: Tuple):
+def test_conservation_of_query_graph(biolink_version: str, graph: Dict):
     """
     This test checks for internal glitch where the query graph is somehow deleted
     """
-    original_graph: Dict = deepcopy(query[1])
-    check_biolink_model_compliance_of_query_graph(graph=query[1], biolink_version=query[0])
-    assert query[1] == original_graph
+    original_graph: Dict = deepcopy(graph)
+    check_biolink_model_compliance_of_query_graph(graph=graph, biolink_version=biolink_version)
+    assert graph == original_graph
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,
@@ -1247,62 +1270,64 @@
         target_provenance=query[1]
     )
     validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
     check_messages(validator, query[2])
 
 
 def qualifier_validator(
+        graph_type: TRAPIGraphType,
         tested_method,
         edge_model: str,
-        query: Tuple[Dict, str],
+        edge: Dict,
+        message: str,
         trapi_version: Optional[str] = None,
-        biolink_version: Optional[str] = LATEST_BIOLINK_MODEL_VERSION
+        biolink_version: Optional[str] = LATEST_BIOLINK_MODEL_VERSION,
+        **kwargs
 ):
-    # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
-    # Sanity check: does TRAPI validation catch this first?
-    trapi_validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    # TODO: to review: which of the validation tests that
+    #       may be overridden by earlier TRAPI validation
+    validator = BiolinkValidator(
+        graph_type=graph_type,
+        trapi_version=trapi_version,
+        biolink_version=biolink_version
+    )
     # Wrap Qualifiers inside a small mock QEdge
-    mock_edge: Dict = deepcopy(query[0])
+    mock_edge: Dict = deepcopy(edge)
     mock_edge["subject"] = "mock_subject"
 
-    if trapi_validator.minimum_required_trapi_version(TRAPI_1_4_0_BETA):
+    if validator.minimum_required_trapi_version(TRAPI_1_4_0_BETA):
         # not testing Edge semantics here but rather, the qualifiers,
         # but from 1.4.0-beta(2) onwards, we also need
         # a non-null predicate and the new 'sources' field here!
         mock_edge["predicate"] = "biolink:related_to"
         mock_edge["sources"] = [
             {
                 "resource_id": "infores:molepro",
                 "resource_role": "primary_knowledge_source"
             }
         ]
 
     mock_edge["object"] = "mock_object"
-    trapi_validator.is_valid_trapi_query(mock_edge, edge_model)
+    validator.is_valid_trapi_query(mock_edge, edge_model)
     # TODO: not sure if simple errors should be fully displaced
     #       by 'critical' errors or rather, just complement them
-    if trapi_validator.has_critical():
-        validator = trapi_validator
+    if validator.has_critical():
+        validator = validator
     else:
-        # if you get this far,then attempt additional Biolink Validation
-        validator = BiolinkValidator(
-            graph_type=TRAPIGraphType.Query_Graph,
-            trapi_version=trapi_version,
-            biolink_version=biolink_version
-        )
         tested_method(
             validator,
             edge_id=f"{tested_method.__name__} unit test",
-            edge=query[0]
+            edge=edge,
+            **kwargs
         )
-    check_messages(validator, query[1])
+    check_messages(validator, message)
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edge,message",
     [
         (  # Query 0 - no 'qualifier_constraints' key - since nullable: true, this should pass
             {},
             ""
         ),
         (  # Query 1 - 'qualifier_constraints' value is None - invalidated by TRAPI schema
             {
@@ -1414,15 +1439,15 @@
                             }
                         ]
                     }
                 ]
             },
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
-        (  # Query 13 - 'qualifier_type_id' property value is valid but abstract
+        (  # Query 13 - 'qualifier_type_id' property is valid but abstract
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:aspect_qualifier",
                                 'qualifier_value': "stability"
@@ -1525,20 +1550,22 @@
                     }
                 ]
             },
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.not_a_predicate"
         )
     ]
 )
-def test_validate_qualifier_constraints(query: Tuple[Dict, str]):
+def test_validate_qualifier_constraints(edge: Dict, message: str):
     # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
     qualifier_validator(
+        graph_type=TRAPIGraphType.Query_Graph,
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
-        query=query
+        edge=edge,
+        message=message
     )
 
 
 # This tests identifiers within a RetrievalSource and is only done for the context of
 # 'resource_id' identifiers but the equivalent functionality assumed for 'upstream_resource_ids'
 @pytest.mark.parametrize(
     "identifier,validation_code",
@@ -1580,15 +1607,15 @@
 def test_validate_infores(identifier: str, validation_code: str):
     validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
     validator.validate_infores("resource_id", "test_validate_infores", identifier)
     check_messages(validator, validation_code)
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edge,message",
     [
         (   # Query 0 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
             #            an incorrect value, which is not a Biolink predicate,  but...
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
@@ -1619,19 +1646,21 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             #    then we don't expect any validation output here?
             ""
         )
     ]
 )
-def test_biolink_validation_suppressed_validate_qualifier_constraints(query: Tuple[Dict, str]):
+def test_biolink_validation_suppressed_validate_qualifier_constraints(edge: Dict, message: str):
     qualifier_validator(
+        graph_type=TRAPIGraphType.Query_Graph,
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
-        query=query,
+        edge=edge,
+        message=message,
         biolink_version="suppress"
     )
 
 
 QC_QS_NOT_A_CURIE = {
     'qualifier_constraints': [
         {
@@ -1643,39 +1672,41 @@
             ]
         }
     ]
 }
 
 
 @pytest.mark.parametrize(
-    "query",
+    "trapi_version,edge,message",
     [
         (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
             TRAPI_1_3_0,
             QC_QS_NOT_A_CURIE,
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
             TRAPI_1_4_0_BETA,
             QC_QS_NOT_A_CURIE,
             "critical.trapi.validation"
         )
     ]
 )
-def test_validate_biolink_curie_in_qualifier_constraints(query: Tuple[str, Dict, str]):
+def test_validate_biolink_curie_in_qualifier_constraints(trapi_version: str, edge: Dict, message: str):
     qualifier_validator(
+        graph_type=TRAPIGraphType.Query_Graph,
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
-        query=query[1:],
-        trapi_version=query[0]
+        edge=edge,
+        message=message,
+        trapi_version=trapi_version
     )
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edge,message",
     [
         (  # Query 0 - no 'qualifiers' key - since nullable: true, this should pass
             {},
             ""
         ),
         (  # Query 1 - 'qualifiers' value is nullable: true, this should pass
             {
@@ -1770,16 +1801,16 @@
                         'qualifier_type_id': "biolink:object_direction_qualifier",
                         'qualifier_value': "upregulated"
                     }
                 ]
             },
             ""    # this particular use case should pass
         ),
-        # (   # This use case was discussed with Sierra on 11 April 2023 and
-        #     # decided to be out-of-scope of enum values for is_permissible_value_of_enum()
+        # (   # This use case was discussed with Sierra on 11 April 2023 and )
+        #     # decided to be out-of-scope of enum values for is_permissible_value_of_enum
         #
         #     # Query ## - 'qualifier_type_id' is a valid Biolink qualifier type and 'RO:0002213'
         #     #            is an 'exact match' to a 'upregulated', the above 'qualifier_value'.
         #     #            This unit test won't pass without a modification of the Biolink Model Toolkit
         #     #            method for validating qualifier values to accept mapped values.
         #     {
         #         'qualifiers': [
@@ -1789,53 +1820,129 @@
         #             }
         #         ]
         #     },
         #     ""
         # )
     ]
 )
-def test_validate_qualifiers(query: Tuple):
+def test_validate_qualifiers(edge: Dict, message: str):
     qualifier_validator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
         tested_method=BiolinkValidator.validate_qualifiers,
         edge_model="Edge",
-        query=query
+        edge=edge,
+        message=message
+    )
+
+
+@pytest.mark.parametrize(
+    "edge,associations,message",
+    [
+        (   # Query 0 - qualifier_type_id 'dubject_aspect_qualifier' is a valid Biolink qualifier type and
+            #            'synthesis' is a valid corresponding 'permissible value' enum 'qualifier_value', but
+            #            only within the context of a specific subclass of biolink:Association, i.e.
+            #
+            #                 gene to disease or phenotypic feature association
+            #                     slot_usage:
+            #                        subject aspect qualifier:
+            #                            range: GeneOrGeneProductOrChemicalEntityAspectEnum
+            #
+            #            which has 'synthesis' as an allowable qualifier value
+            {
+                'qualifiers': [
+                    {
+                        'qualifier_type_id': "biolink:subject_aspect_qualifier",
+                        'qualifier_value': "synthesis"
+                    }
+                ]
+            },
+            ["biolink:GeneToDiseaseOrPhenotypicFeatureAssociation"],  # associations: Optional[List[str]]
+            ""   # this particular use case should pass
+        ),
+        (   # Query 1 - This example is identical to the above, but we know that it must fail if the
+            #      biolink:Association context of the edge is not given to the qualifier validator as a parameter
+            {
+                'qualifiers': [
+                    {
+                        'qualifier_type_id': "biolink:subject_aspect_qualifier",
+                        'qualifier_value': "synthesis"
+                    }
+                ]
+            },
+
+            None,  # associations: Optional[List[str]]
+
+            "error.knowledge_graph.edge.qualifiers.qualifier.value.unresolved"
+        ),
+        (   # Query 2 -  another example of a 'qualifier_type_id' resolvable only within
+            #            the context of a specific subclass of biolink:Association, i.e.
+            #
+            #                 biolink:ChemicalAffectsGeneAssociation
+            #                     slot_usage:
+            #                        object aspect qualifier:
+            #                            range: GeneOrGeneProductOrChemicalPartQualifierEnum
+            #
+            #            which has 'promoter' as an allowable qualifier value
+            {
+                'qualifiers': [
+                    {
+                        'qualifier_type_id': "biolink:object_aspect_qualifier",
+                        'qualifier_value': "promoter"
+                    }
+                ]
+            },
+            ["biolink:ChemicalAffectsGeneAssociation"],  # associations: Optional[List[str]]
+            ""   # this particular use case should pass
+        )
+    ]
+)
+def test_validate_qualifiers_with_association(edge: Dict, associations: Optional[List[str]], message: str):
+    qualifier_validator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
+        tested_method=BiolinkValidator.validate_qualifiers,
+        edge_model="Edge",
+        edge=edge,
+        message=message,
+        associations=associations
     )
 
 
 Q_NOT_A_CURIE = {
     'qualifiers': [
         {
             'qualifier_type_id': "not-a-curie",
             'qualifier_value': "fake-qualifier-value"
         }
     ]
 }
 
 
 @pytest.mark.parametrize(
-    "query",
+    "trapi_version,edge,message",
     [
         (  # Query 0 - 'qualifier_type_id' value not a Biolink CURIE - seen as 'unknown' in TRAPI < 1.4.0-beta
                 TRAPI_1_3_0,
                 Q_NOT_A_CURIE,
                 "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
                 TRAPI_1_4_0_BETA,
                 Q_NOT_A_CURIE,
                 "critical.trapi.validation"
         )
     ]
 )
-def test_validate_biolink_curie_in_qualifiers(query: Tuple[str, Dict, str]):
+def test_validate_biolink_curie_in_qualifiers(trapi_version: str, edge: Dict, message: str):
     qualifier_validator(
+        graph_type=TRAPIGraphType.Knowledge_Graph,
         tested_method=BiolinkValidator.validate_qualifiers,
         edge_model="Edge",
-        query=query[1:],
-        trapi_version=query[0]
+        edge=edge,
+        message=message,
+        trapi_version=trapi_version
     )
 
 
 ##################################
 # Validate TRAPI Knowledge Graph #
 ##################################
 @pytest.mark.parametrize(
@@ -2277,16 +2384,14 @@
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
                 }
             },
             # ditto for predicate and object... but identical code pattern thus we only test missing subject id here
-            # f"{KNOWLEDGE_GRAPH_PREFIX}: ERROR - Edge 'None--biolink:interacts_with->NCBIGene:29974' " +
-            # "has a missing or empty 'subject' slot value!"
             "error.knowledge_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 15: 'subject' id is missing from the nodes catalog
             {
                 "nodes": SIMPLE_SAMPLE_NODES,
@@ -2739,15 +2844,17 @@
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         )
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(
-        biolink_version: str, graph_data: Dict, validation_code: str
+        biolink_version: str,
+        graph_data: Dict,
+        validation_code: str
 ):
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=graph_data, biolink_version=biolink_version
     )
     check_messages(validator, validation_code)
```

### Comparing `reasoner_validator-3.7.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/tests/test_response_validator.py` & `reasoner_validator-3.7.6/tests/test_response_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 from json import dump
 
 from copy import deepcopy
 
 import pytest
 
-from reasoner_validator import TRAPIResponseValidator
-from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
+from reasoner_validator import TRAPI_1_3_0, TRAPI_1_4_2
+from reasoner_validator.validator import TRAPIResponseValidator
+from reasoner_validator.trapi import TRAPIGraphType
 
 from tests import PATCHED_140_SCHEMA_FILEPATH, SAMPLE_NODES_WITH_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
@@ -200,15 +201,15 @@
 
 
 _TEST_KG_4 = {
     "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_4
 }
 
-# From Implementation Guidlines circa June 2023
+# From Implementation Guidelines circa June 2023
 _TEST_TRAPI_1_4_2_FULL_SAMPLE = {
     "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
@@ -294,124 +295,120 @@
         ]
     }
 }
 
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
 
+# original TRAPI schema.. changing the 'schema_version' may generate errors
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION["schema_version"] = "1.3.0"
+
+# original TRAPI schema.. changing the 'biolink_version' may generate errors
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION["biolink_version"] = "2.4.8"
 
 @pytest.mark.parametrize(
-    "query",
+    "response",
     [
-        (   # Query 0 - No "workflow" key in TRAPI Response
-            {
-                "message": {}
-            },
-        ),
-        (   # Query 1 - Null "workflow" key value
-            {
-                "message": {},
-                "workflow": None
-            },
-        ),
-        (  # Query 2 - Null "workflow" key list
-            {
-                "message": {},
-                "workflow": []
-            },
-        ),
-        (  # Query 3 - "runner_parameters" is Null
-            {
-                "message": {},
-                "workflow": [
-                    {
-                        "runner_parameters": None,
-                        "id": "sort_results_score",
-                        "parameters": {"ascending_or_descending": "ascending"}
-                    }
-                ]
-            },
-        ),
-        (  # Query 4 - "parameters" is Null
-            {
-                "message": {},
-                "workflow": [
-                    {"runner_parameters": {"allowlist": ["infores:aragorn"]}, "id": "lookup", "parameters": None}
-                ]
-            },
-        ),
-        (  # Query 5 - both "parameters" and "runner_parameters" are Null
-            {
-                "message": {},
-                "workflow": [
-                    {"runner_parameters": None, "id": "lookup", "parameters": None}
-                ]
-            },
-        ),
-        (   # Query 6 - Now, we patch the Message itself when it is not empty - knowledge graph is nullable
-            {
-                "message": {
-                    "knowledge_graph": None
+        # Query 0 - No "workflow" key in TRAPI Response
+        {
+            "message": {}
+        },
+        # Query 1 - Null "workflow" key value
+        {
+            "message": {},
+            "workflow": None
+        },
+        # Query 2 - Null "workflow" key list
+        {
+            "message": {},
+            "workflow": []
+        },
+        # Query 3 - "runner_parameters" is Null
+        {
+            "message": {},
+            "workflow": [
+                {
+                    "runner_parameters": None,
+                    "id": "sort_results_score",
+                    "parameters": {"ascending_or_descending": "ascending"}
                 }
-            },
-        ),
-        (   # Query 7 - Now, we patch the Message itself when it is not empty
-            {
-                "message": {
-                    "knowledge_graph": {
-                        "nodes": {},
-                        "edges": {}
-                    }
+            ]
+        },
+        # Query 4 - "parameters" is Null
+        {
+            "message": {},
+            "workflow": [
+                {"runner_parameters": {"allowlist": ["infores:aragorn"]}, "id": "lookup", "parameters": None}
+            ]
+        },
+        # Query 5 - both "parameters" and "runner_parameters" are Null
+        {
+            "message": {},
+            "workflow": [
+                {"runner_parameters": None, "id": "lookup", "parameters": None}
+            ]
+        },
+        # Query 6 - Now, we patch the Message itself when it is not empty - knowledge graph is nullable
+        {
+            "message": {
+                "knowledge_graph": None
+            }
+        },
+        # Query 7 - Now, we patch the Message itself when it is not empty
+        {
+            "message": {
+                "knowledge_graph": {
+                    "nodes": {},
+                    "edges": {}
                 }
-            },
-        ),
-        (   # Query 8 - Now, we patch the Message itself when it is not empty
-            {
-                "message": {
-                    "knowledge_graph": {
-                        "nodes": {},
-                        "edges": {}
-                    }
+            }
+        },
+        # Query 8 - Now, we patch the Message itself when it is not empty
+        {
+            "message": {
+                "knowledge_graph": {
+                    "nodes": {},
+                    "edges": {}
                 }
-            },
-        ),
-        (   # Query 9 - Now, we patch the "Message.knowledge_edge.sources" itself when it is not empty
-            {
-                "message": {
-                    "knowledge_graph": {
-                        "nodes": {},
-                        "edges": {
-                            "alice-in-wonderland": {
-                                 "subject": "tweedle-dee",
-                                 "predicate": "and",
-                                 "object": "tweedle-dum",
-                                 "sources": [
-                                     {
-                                         "resource_id": "infores:rabbit-hole",
-                                         "resource_role": "primary_knowledge_source"
-                                     }
-                                 ]
-                            }
+            }
+        },
+        # Query 9 - Now, we patch the "Message.knowledge_edge.sources" itself when it is not empty
+        {
+            "message": {
+                "knowledge_graph": {
+                    "nodes": {},
+                    "edges": {
+                        "alice-in-wonderland": {
+                             "subject": "tweedle-dee",
+                             "predicate": "and",
+                             "object": "tweedle-dum",
+                             "sources": [
+                                 {
+                                     "resource_id": "infores:rabbit-hole",
+                                     "resource_role": "primary_knowledge_source"
+                                 }
+                             ]
                         }
                     }
                 }
-            },
-        ),
-        (   # Query 10 - Now, we patch the Message itself when it is not empty
-            {
-                "message": {
-                    "auxiliary_graphs": None
-                }
-            },
-        )
+            }
+        },
+        # Query 10 - Now, we patch the Message itself when it is not empty
+        {
+            "message": {
+                "auxiliary_graphs": None
+            }
+        }
     ]
 )
-def test_sanitize_trapi_query(query: Tuple):
+def test_sanitize_trapi_query(response: Dict):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
-    response: Dict = validator.sanitize_trapi_response(response=query[0])
+    response: Dict = validator.sanitize_trapi_response(response=response)
     dump(response, stderr, indent=4)
 
 
 NUM_SAMPLE_NODES = 5
 
 SAMPLE_NODES: Dict = dict()
 for node_id in range(1, NUM_SAMPLE_NODES):
@@ -430,15 +427,15 @@
 TEST_GRAPH: Dict = {
     "nodes": SAMPLE_NODES,
     "edges": SAMPLE_EDGES
 }
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edges_limit,number_of_nodes_returned,number_of_edges_returned",
     [
         (   # Query 0 - unlimited sample whole graph
             0,  # edges_limit
             len(SAMPLE_NODES),  # number of nodes returned
             len(SAMPLE_EDGES)   # number of edges returned
         ),
         (   # Query 1 - sample just 2 edges
@@ -449,24 +446,24 @@
         (   # Query 2 - sample just edge_value is negative number (functionally equivalent to zero)
             -1,  # edges_limit
             len(SAMPLE_NODES),  # number of nodes returned
             len(SAMPLE_EDGES)   # number of edges returned
         )
     ]
 )
-def test_sample_graph(query: Tuple[int, int, int]):
+def test_sample_graph(edges_limit: int, number_of_nodes_returned: int, number_of_edges_returned: int):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
-    kg_sample: Dict = validator.sample_graph(graph=TEST_GRAPH, edges_limit=query[0])
+    kg_sample: Dict = validator.sample_graph(graph=TEST_GRAPH, edges_limit=edges_limit)
     assert kg_sample
-    assert len(kg_sample["nodes"]) == query[1]
-    assert len(kg_sample["edges"]) == query[2]
+    assert len(kg_sample["nodes"]) == number_of_nodes_returned
+    assert len(kg_sample["edges"]) == number_of_edges_returned
 
 
 @pytest.mark.parametrize(
-    "query",
+    "response,trapi_version,biolink_version,target_provenance,strict_validation,message",
     [
         (   # Query 0 - Completely empty Response.Message
             {
                 "message": {
 
                 }
             },
@@ -979,25 +976,51 @@
             #            TRAPI implementation guidelines...) just for fun and profit
             _TEST_TRAPI_1_4_2_FULL_SAMPLE,
             TRAPI_1_4_2,
             None,
             None,
             True,
             ""   # this filtered workflow spec should pass
+        ),
+        (   # Query 27 - We throw a full TRAPI JSON example here (taken directly from the TRAPI implementation
+            #            guidelines...) but add the 'schema_version' just for fun and profit
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION,
+            None,
+            "3.0.0",
+            None,
+            True,
+            "critical.trapi.validation"   # trying to validate a 1.4.2 schema against 1.3.0 will fail!
+        ),
+        (   # Query 28 - We throw a full TRAPI JSON example here (taken directly from the TRAPI implementation
+            #            guidelines...) but explicitly specify the 'biolink_version == 2.5.8' just for fun and profit
+            _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION,
+            TRAPI_1_4_2,
+            None,
+            None,
+            True,
+            # Validation with 2.4.8 generates a warning
+            "warning.knowledge_graph.edge.predicate.non_canonical"
         )
     ]
 )
-def test_check_biolink_model_compliance_of_trapi_response(query: Tuple):
+def test_check_biolink_model_compliance_of_trapi_response(
+        response: Dict,
+        trapi_version: str,
+        biolink_version: str,
+        target_provenance: Dict,
+        strict_validation: bool,
+        message: str
+):
     validator: TRAPIResponseValidator = TRAPIResponseValidator(
-        trapi_version=query[1],
-        biolink_version=query[2],
-        strict_validation=query[4]
+        trapi_version=trapi_version,
+        biolink_version=biolink_version,
+        strict_validation=strict_validation
     )
-    validator.check_compliance_of_trapi_response(response=query[0], target_provenance=query[3])
-    check_messages(validator, query[5], no_errors=True)
+    validator.check_compliance_of_trapi_response(response=response, target_provenance=target_provenance)
+    check_messages(validator, message, no_errors=True)
 
 
 @pytest.mark.parametrize(
     "response,trapi_version,biolink_version,sources,strict_validation,code",
     [
         (   # Query 0 - Completely empty Response.Message
             {
```

### Comparing `reasoner_validator-3.7.5/tests/test_semver.py` & `reasoner_validator-3.7.6/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.6/tests/test_trapi_versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test TRAPI version handling."""
 from typing import Dict, Optional
 
 import pytest
 
 from reasoner_validator.versioning import get_latest_version
-from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, load_schema, TRAPIAccessError
+from reasoner_validator.trapi import load_schema, TRAPIAccessError
+from reasoner_validator import LATEST_TRAPI_RELEASE
 from tests import PATCHED_140_SCHEMA_FILEPATH, BROKEN_SCHEMA_FILEPATH
 
 
 def test_release_tag_is_none():
     trapi_version:  Optional[str] = get_latest_version(release_tag=None)
     assert trapi_version is None
```

### Comparing `reasoner_validator-3.7.5/tests/test_validate.py` & `reasoner_validator-3.7.6/tests/test_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from copy import deepcopy
 
 import pytest
 
 from jsonschema.exceptions import ValidationError
 
 from reasoner_validator.trapi import TRAPISchemaValidator, openapi_to_jsonschema, load_schema
-
+from reasoner_validator import LATEST_TRAPI_RELEASE
 from tests import LATEST_TEST_RELEASES, PRE_1_4_0_TEST_VERSIONS, ALL_TEST_VERSIONS
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # query 0
@@ -87,14 +87,23 @@
 
 def test_load_master_schema():
     """Test load_schema('master')."""
     schema = load_schema("master")
     assert schema, "TRAPI Schema for ('master') branch is not available?"
 
 
+def test_message():
+    reporter = TRAPISchemaValidator(prefix="Test Message", trapi_version="v1.4")
+    assert reporter.get_trapi_version() == LATEST_TRAPI_RELEASE
+    assert not reporter.has_messages()
+    reporter.report("info.compliant")
+    assert reporter.has_messages()
+    reporter.dump()
+
+
 @pytest.mark.parametrize(
     "trapi_version",
     ALL_TEST_VERSIONS
 )
 def test_query_and_version_completion(trapi_version: str):
     """Test TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
```

### Comparing `reasoner_validator-3.7.5/tests/test_validation_report.py` & `reasoner_validator-3.7.6/tests/test_validation_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
 def test_unknown_message_code():
     with pytest.raises(AssertionError):
         CodeDictionary.display(code="foo.bar")
 
 
 def test_message_report():
-    reporter = ValidationReporter(prefix="First Validation Report", trapi_version=TEST_TRAPI_VERSION)
+    reporter = ValidationReporter(prefix="First Validation Report")
     reporter.report(code="info.compliant")
     reporter.report(
         code="info.input_edge.predicate.abstract",
         identifier="biolink:contributor",
         edge_id="a->biolink:contributor->b"
     )
     report: MESSAGE_CATALOG = reporter.get_messages()
@@ -222,54 +222,43 @@
         displayed.extend(scoped_messages["global"])
     assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in displayed
     assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" in displayed
 
 
 def test_messages():
     # Loading and checking a first reporter
-    reporter1 = ValidationReporter(prefix="1st Test Message Set", trapi_version=TEST_TRAPI_VERSION)
-    assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
-    assert reporter1.get_biolink_version() is None
+    reporter1 = ValidationReporter(prefix="1st Test Message Set")
     assert not reporter1.has_messages()
     reporter1.report("info.compliant")
     assert reporter1.has_messages()
     assert reporter1.has_information()
     assert not reporter1.has_warnings()
     assert not reporter1.has_errors()
     assert not reporter1.has_critical()
 
     reporter1.report("warning.graph.empty", identifier="Reporter1 Unit Test")
     assert reporter1.has_warnings()
     reporter1.report("error.knowledge_graph.nodes.empty")
     assert reporter1.has_errors()
 
     # Testing merging of messages from a second reporter
-    reporter2 = ValidationReporter(
-        prefix="2nd Test Message Set",
-        biolink_version=TEST_BIOLINK_VERSION
-    )
-    assert reporter2.get_trapi_version() == TEST_TRAPI_VERSION
-    assert reporter2.get_biolink_version() == TEST_BIOLINK_VERSION
+    reporter2 = ValidationReporter(prefix="2nd Test Message Set")
     reporter2.report(
         code="info.query_graph.edge.predicate.mixin",
         identifier="biolink:this_is_a_mixin",
         edge_id="a-biolink:this_is_a_mixin->b"
     )
     reporter2.report("warning.trapi.response.results.empty")
     reporter2.report("error.knowledge_graph.edges.empty")
     reporter1.merge(reporter2)
-    assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
-    assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
-    
+
     # No prefix...
     reporter3 = ValidationReporter()
     reporter3.report("error.trapi.response.query_graph.missing")
     reporter1.merge(reporter3)
-    assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
-    assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
 
     # testing addition a few raw batch messages
     new_messages: MESSAGE_CATALOG = {
         "information": {
             "info.excluded": {
                 "global": {
                     "Horace van der Gelder": None
@@ -351,16 +340,14 @@
     for code, messages in message_catalog['critical'].items():
         scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
         scope, value = scoped_messages.popitem()
         critical.append(value[0])
     assert "CRITICAL - Trapi: Schema validation error" in critical
 
     obj = reporter1.to_dict()
-    assert obj["trapi_version"] == TEST_TRAPI_VERSION
-    assert obj["biolink_version"] == TEST_BIOLINK_VERSION
     assert "messages" in obj
     assert "critical" in obj["messages"]
     assert "critical.trapi.validation" in obj["messages"]["critical"]
 
     message_catalog: SCOPED_MESSAGES = obj["messages"]["critical"]["critical.trapi.validation"]
     assert message_catalog, "Empty 'critical.trapi.validation' messages set?"
     assert "9.1.1" in message_catalog["global"]
@@ -406,19 +393,15 @@
 
     validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
     assert validation_report.startswith("Reasoner Validator")
 
 
 def test_validator_method():
 
-    reporter = ValidationReporter(
-        prefix="Test Validator Method",
-        trapi_version=TEST_TRAPI_VERSION,
-        biolink_version=TEST_BIOLINK_VERSION
-    )
+    reporter = ValidationReporter(prefix="Test Validator Method")
 
     test_data: Dict = {
         "some key": "some value"
     }
     test_parameters: Dict = {
         "some parameter": "some parameter value",
         "another parameter": "some other parameter value"
@@ -458,54 +441,48 @@
         scope, value = scoped_messages.popitem()
         errors.append(value[0])
     assert "ERROR - Knowledge Graph Edge Provenance Infores: " + \
            "Edge has provenance value which is not a well-formed InfoRes CURIE" in errors
 
 
 @pytest.mark.parametrize(
-    "query",
+    "tag,case,result",
     [
         (
             'validation',
             {
                 "validation": {
-                    "trapi_version": "1.3",
-                    "biolink_version": "2.4.7",
                     "messages": {
                         "information": {},
                         "warnings": {},
                         "errors": {},
                         "critical": {""}
                     }
                 }
             },
             True
         ),
         (
-                'validation',
-                {
-                    "validation": {
-                        "trapi_version": "1.3",
-                        "biolink_version": "2.4.7",
-                        "messages": {
-                            "information": {},
-                            "warnings": {},
-                            "errors": {""},
-                            "critical": {}
-                        }
+            'validation',
+            {
+                "validation": {
+                    "messages": {
+                        "information": {},
+                        "warnings": {},
+                        "errors": {""},
+                        "critical": {}
                     }
-                },
-                True
+                }
+            },
+            True
         ),
         (
             "validation",
             {
                 "validation": {
-                    "trapi_version": "1.3",
-                    "biolink_version": "2.4.7",
                     "messages": {
                         "information": {},
                         "warnings": {
                             "warning.input_edge.node.category.deprecated": [
                                 {
                                     "identifier": "biolink:ChemicalSubstance"
                                 }
@@ -522,10 +499,10 @@
                     }
                 }
             },
             False
         ),
     ]
 )
-def test_has_validation_errors(query: Tuple):
+def test_has_validation_errors(tag: str, case: Dict, result: bool):
     reporter = ValidationReporter()
-    assert reporter.test_case_has_validation_errors(tag=query[0], case=query[1]) == query[2]
+    assert reporter.test_case_has_validation_errors(tag=tag, case=case) == result
```

### Comparing `reasoner_validator-3.7.5/tests/test_workflows.py` & `reasoner_validator-3.7.6/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.5/PKG-INFO` & `reasoner_validator-3.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.5
+Version: 3.7.6
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -17,25 +17,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: docs
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: bmt (>=1.1.0,<2.0.0)
+Requires-Dist: bmt (>=1.1.1,<2.0.0)
 Requires-Dist: fastapi (>=0.68,<0.69) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
-Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
+Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.2.1,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx (>=6.2.1,<7.0.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.2.2,<2.0.0) ; extra == "docs"
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.15,<0.16) ; extra == "web"
 Project-URL: Bug Tracker, https://github.com/NCATSTranslator/reasoner-validator/issues
 Project-URL: Change Log, https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://translator-reasoner-validator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/NCATSTranslator/reasoner-validator
 Description-Content-Type: text/markdown
```

