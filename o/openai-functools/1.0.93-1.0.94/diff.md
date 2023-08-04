# Comparing `tmp/openai_functools-1.0.93.tar.gz` & `tmp/openai_functools-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-1.0.93.tar", max compression
+gzip compressed data, was "openai_functools-1.0.94.tar", max compression
```

## Comparing `openai_functools-1.0.93.tar` & `openai_functools-1.0.94.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-08-04 13:50:31.851459 openai_functools-1.0.93/LICENSE
--rw-r--r--   0        0        0     7059 2023-08-04 13:50:31.851459 openai_functools-1.0.93/README.md
--rw-r--r--   0        0        0      342 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/__init__.py
--rw-r--r--   0        0        0      240 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/function_spec.py
--rw-r--r--   0        0        0     6838 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/functions_orchestrator.py
--rw-r--r--   0        0        0     1755 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/types.py
--rw-r--r--   0        0        0       69 2023-08-04 13:50:31.871456 openai_functools-1.0.93/openai_functools/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-08-04 13:50:52.415399 openai_functools-1.0.93/pyproject.toml
--rw-r--r--   0        0        0     7759 1970-01-01 00:00:00.000000 openai_functools-1.0.93/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 14:16:33.513892 openai_functools-1.0.94/LICENSE
+-rw-r--r--   0        0        0     7059 2023-08-04 14:16:33.513892 openai_functools-1.0.94/README.md
+-rw-r--r--   0        0        0      342 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/__init__.py
+-rw-r--r--   0        0        0      240 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/function_spec.py
+-rw-r--r--   0        0        0     6838 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/functions_orchestrator.py
+-rw-r--r--   0        0        0     1755 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/types.py
+-rw-r--r--   0        0        0       69 2023-08-04 14:16:33.533893 openai_functools-1.0.94/openai_functools/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-08-04 14:16:59.894067 openai_functools-1.0.94/pyproject.toml
+-rw-r--r--   0        0        0     7759 1970-01-01 00:00:00.000000 openai_functools-1.0.94/PKG-INFO
```

### Comparing `openai_functools-1.0.93/LICENSE` & `openai_functools-1.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.93/README.md` & `openai_functools-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.93/openai_functools/functions_orchestrator.py` & `openai_functools-1.0.94/openai_functools/functions_orchestrator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.93/openai_functools/metadata_generator.py` & `openai_functools-1.0.94/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.93/pyproject.toml` & `openai_functools-1.0.94/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "1.0.93"
+version = "1.0.94"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `openai_functools-1.0.93/PKG-INFO` & `openai_functools-1.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 1.0.93
+Version: 1.0.94
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

