# Comparing `tmp/polyglot-piranha-playground-0.0.2.tar.gz` & `tmp/polyglot-piranha-playground-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyglot-piranha-playground-0.0.2.tar", last modified: Tue Jul 18 23:29:50 2023, max compression
+gzip compressed data, was "polyglot-piranha-playground-0.0.3.tar", last modified: Fri Aug  4 21:53:34 2023, max compression
```

## Comparing `polyglot-piranha-playground-0.0.2.tar` & `polyglot-piranha-playground-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.976536 polyglot-piranha-playground-0.0.2/piranha_playground/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/data_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.976536 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/piranha_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/piranha_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/rule_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/static_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.976536 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_codebase_refactorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_piranha_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/logger_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/pretty_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/rule_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/piranha_playground/static/
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/static/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/piranha_playground/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/piranha_playground/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 23:29:50.000000 polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:29:50.980536 polyglot-piranha-playground-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-18 23:29:14.000000 polyglot-piranha-playground-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.955813 polyglot-piranha-playground-0.0.3/piranha_playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/piranha_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/piranha_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/rule_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/static_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_codebase_refactorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_piranha_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/logger_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/pretty_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/rule_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/piranha_playground/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/piranha_playground/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/piranha_playground/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 21:53:34.000000 polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:53:34.959813 polyglot-piranha-playground-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-04 21:48:42.000000 polyglot-piranha-playground-0.0.3/setup.py
```

### Comparing `polyglot-piranha-playground-0.0.2/PKG-INFO` & `polyglot-piranha-playground-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot-piranha-playground
-Version: 0.0.2
+Version: 0.0.3
 Summary: A playground for Piranha
 Home-page: https://github.com/uber/piranha
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `polyglot-piranha-playground-0.0.2/README.md` & `polyglot-piranha-playground-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/__init__.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/__init__.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/data_validation.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/data_validation.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/main.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/main.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/__init__.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/controller.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/controller.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/graph_parser.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/graph_parser.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/piranha_agent.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/piranha_agent.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/piranha_chat.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/piranha_chat.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/rule_application.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/rule_application.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 # <p>Unless required by applicable law or agreed to in writing, software distributed under the
 # License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import multiprocessing
-from typing import List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import attr
 import toml
-from polyglot_piranha import (PiranhaArguments, PiranhaOutputSummary, Rule,
-                              RuleGraph, execute_piranha)
-
-from piranha_playground.rule_inference.utils.logger_formatter import \
-    CustomFormatter
+from piranha_playground.rule_inference.utils.logger_formatter import CustomFormatter
 from piranha_playground.rule_inference.utils.rule_utils import RawRuleGraph
+from polyglot_piranha import (
+    PiranhaArguments,
+    PiranhaOutputSummary,
+    Rule,
+    RuleGraph,
+    execute_piranha,
+)
 
 logger = logging.getLogger("CodebaseRefactorer")
 logger.setLevel(logging.DEBUG)
 
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
@@ -44,16 +47,33 @@
     Sets up the logging configurations for Piranha.
     """
     FORMAT = "%(levelname)s %(name)s %(asctime)-15s %(filename)s:%(lineno)d %(message)s"
     logging.basicConfig(format=FORMAT)
     logging.getLogger().setLevel(logging.DEBUG)
 
 
+def flatten_dict_list(d: Dict):
+    for k, v in d.items():
+        if isinstance(v, list) and len(v) == 1:
+            d[k] = v[0]
+        elif isinstance(v, dict):
+            flatten_dict_list(v)
+        elif isinstance(v, list):
+            for item in v:
+                if isinstance(item, dict):
+                    flatten_dict_list(item)
+    return d
+
+
 def _run_piranha_with_timeout_aux(
-    source_code: str, language: str, raw_graph: RawRuleGraph, substitutions: dict, timeout: int = 0
+    source_code: str,
+    language: str,
+    raw_graph: RawRuleGraph,
+    timeout: int = 0,
+    **kwargs,
 ):
     """
     Private method to run Piranha with a timeout. Executes Piranha with provided arguments.
 
     :param source_code: str: The source code to be refactored.
     :param language: str: The language of the source code.
     :param raw_graph: RawRuleGraph: The rule graph to be used for refactoring.
@@ -64,15 +84,15 @@
     try:
         # Prepare arguments for Piranha execution
         args = PiranhaArguments(
             code_snippet=source_code,
             language=language,
             rule_graph=raw_graph.to_graph(),
             dry_run=True,
-            substitutions=substitutions,
+            **kwargs,
         )
         piranha_results = execute_piranha(args)
         # Check if the execution returns results, if yes then return the content of the first result
         # Otherwise, return an empty list
         if piranha_results:
             return piranha_results[0].content, True
         return source_code, True
@@ -126,21 +146,22 @@
 
         :return: List[PiranhaOutputSummary]: A list of summaries of the changes made by Piranha.
         :raises CodebaseRefactorerException: If the refactoring fails.
         """
         try:
             toml_dict = toml.loads(self.rules)
             rule_graph = RawRuleGraph.from_toml(toml_dict)
+            arguments = toml_dict.get("arguments", [{}])[0]
+            arguments = flatten_dict_list(arguments)
             args = PiranhaArguments(
                 language=self.language,
                 path_to_codebase=self.path_to_codebase,
                 rule_graph=rule_graph.to_graph(),
                 dry_run=dry_run,
-                substitutions=toml_dict.get("substitutions", [{}])[0],
-                allow_dirty_ast=True,
+                **arguments,
             )
 
             output_summaries = execute_piranha(args)
             logger.info("Changed files:")
             for summary in output_summaries:
                 logger.info(summary.path)
             return output_summaries
@@ -157,21 +178,22 @@
         :param rules: str: The refactoring rules in a .toml format.
 
         :return: str: The refactored code or error message.
         :raises CodebaseRefactorerException: If the refactoring fails.
         """
         try:
             toml_dict = toml.loads(rules)
-            substitutions = toml_dict.get("substitutions", [{}])[0]
+            arguments = toml_dict.get("arguments", [{}])[0]
+            arguments = flatten_dict_list(arguments)
             refactored_code, success = run_piranha_with_timeout(
                 source_code,
                 language,
                 RawRuleGraph.from_toml(toml_dict),
                 timeout=5,
-                substitutions=substitutions,
+                **arguments,
             )
             return refactored_code
         except multiprocessing.context.TimeoutError as e:
             raise CodebaseRefactorerException(
                 "Piranha is likely in an infinite loop. Please check your rules."
             ) from e
         except Exception as e:
```

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/static_inference.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/static_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,17 +169,16 @@
                 if cursor.node.is_named:
                     visited += 1
                     s_exp += self.strategy.process_child(cursor, depth)
                 next_child = cursor.goto_next_sibling()
 
             # if the node is an identifier, add it to eq constraints
             if visited == 0:
-                self.query_ctrs.append(
-                    f"(#eq? {node_name} \"{node.text.decode('utf8')}\")"
-                )
+                text = node.text.decode("utf8").replace("\n", " ")
+                self.query_ctrs.append(f'(#eq? {node_name} "{text}")')
             s_exp += f")"
 
         self.capture_groups[node_name] = node
         self.outer_most_node = node_name
         return s_exp + f" {node_name}"
 
     def simplify_query(self, capture_group):
```

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/template_parser.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/template_parser.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/__init__.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_codebase_refactorer.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_codebase_refactorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 from unittest.mock import Mock, patch
 
 import pytest
 import toml
 from polyglot_piranha import PiranhaOutputSummary
 
 from piranha_playground.rule_inference.rule_application import (
-    CodebaseRefactorer, CodebaseRefactorerException,
-    _run_piranha_with_timeout_aux)
+    CodebaseRefactorer,
+    CodebaseRefactorerException,
+    _run_piranha_with_timeout_aux,
+)
 
 
 # Test for successful execution of Piranha with a timeout
 def test_run_piranha_with_timeout_success():
     rules = pathlib.Path(
         "test-resources/java/feature_flag_system_2/control/configurations/rules.toml"
     ).read_text()
@@ -30,20 +32,24 @@
     ).read_text()
 
     language = "java"
     # append substitutions to the toml_dict
     toml_dict = {
         **toml.loads(rules),
         **toml.loads(edges),
-        "substitutions": [
+        "arguments": [
             {
-                "stale_flag_name": "STALE_FLAG",
-                "treated": "true",
-                "treated_complement": "false",
-                "namespace": "some_long_name",
+                "substitutions": [
+                    {
+                        "stale_flag_name": "STALE_FLAG",
+                        "treated": "true",
+                        "treated_complement": "false",
+                        "namespace": "some_long_name",
+                    }
+                ]
             }
         ],
     }
 
     refactorer = CodebaseRefactorer(
         language,
         "test-resources/java/feature_flag_system_2/control/input",
@@ -68,10 +74,13 @@
         (#eq? @var_name "A")
     )"""
     replace_node = "var_name"
     replace = "B"
     '''
     source_code = "class A {}"
 
-    with patch('piranha_playground.rule_inference.rule_application.run_piranha_with_timeout', new=_run_piranha_with_timeout_aux):
+    with patch(
+        "piranha_playground.rule_inference.rule_application.run_piranha_with_timeout",
+        new=_run_piranha_with_timeout_aux,
+    ):
         x = CodebaseRefactorer.refactor_snippet(source_code, language, graph)
         assert x == "class B {}"
```

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_controller.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_graph_parser.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_graph_parser.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_inference.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_piranha_agent.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_piranha_agent.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_server.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,24 @@
         "test-resources/java/feature_flag_system_2/control/configurations/edges.toml"
     ).read_text()
 
     # append substitutions to the toml_dict
     toml_dict = {
         **toml.loads(rules),
         **toml.loads(edges),
-        "substitutions": [
+        "arguments": [
             {
-                "stale_flag_name": "STALE_FLAG",
-                "treated": "true",
-                "treated_complement": "false",
-                "namespace": "some_long_name",
+                "substitutions": [
+                    {
+                        "stale_flag_name": "STALE_FLAG",
+                        "treated": "true",
+                        "treated_complement": "false",
+                        "namespace": "some_long_name",
+                    }
+                ]
             }
         ],
     }
 
     # Test data for the /refactor_codebase route
     data = {
         "language": "java",
```

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/tests/test_template_parser.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/tests/test_template_parser.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/__init__.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/logger_formatter.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/logger_formatter.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/node_utils.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/node_utils.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/pretty_toml.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/pretty_toml.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/rule_inference/utils/rule_utils.py` & `polyglot-piranha-playground-0.0.3/piranha_playground/rule_inference/utils/rule_utils.py`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/static/script.js` & `polyglot-piranha-playground-0.0.3/piranha_playground/static/script.js`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/static/styles.css` & `polyglot-piranha-playground-0.0.3/piranha_playground/static/styles.css`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/piranha_playground/templates/index.html` & `polyglot-piranha-playground-0.0.3/piranha_playground/templates/index.html`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/PKG-INFO` & `polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot-piranha-playground
-Version: 0.0.2
+Version: 0.0.3
 Summary: A playground for Piranha
 Home-page: https://github.com/uber/piranha
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `polyglot-piranha-playground-0.0.2/polyglot_piranha_playground.egg-info/SOURCES.txt` & `polyglot-piranha-playground-0.0.3/polyglot_piranha_playground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyglot-piranha-playground-0.0.2/setup.py` & `polyglot-piranha-playground-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import find_packages, setup
 
 setup(
     name="polyglot-piranha-playground",
-    version="0.0.2",
+    version="0.0.3",
     description="A playground for Piranha",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/uber/piranha",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

