# Comparing `tmp/check_shapes-1.1.0.tar.gz` & `tmp/check_shapes-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_shapes-1.1.0.tar", max compression
+gzip compressed data, was "check_shapes-1.1.1.tar", max compression
```

## Comparing `check_shapes-1.1.0.tar` & `check_shapes-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-08-03 14:20:56.824118 check_shapes-1.1.0/LICENSE
--rw-r--r--   0        0        0     1147 2023-08-03 14:20:56.824118 check_shapes-1.1.0/README.md
--rw-r--r--   0        0        0     2436 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/__init__.py
--rw-r--r--   0        0        0     1756 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/accessors.py
--rw-r--r--   0        0        0     6712 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/argument_ref.py
--rw-r--r--   0        0        0     1106 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/base_types.py
--rw-r--r--   0        0        0     4213 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/bool_specs.py
--rw-r--r--   0        0        0     2908 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/check_shapes.lark
--rw-r--r--   0        0        0    22338 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/checker.py
--rw-r--r--   0        0        0     2775 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/checker_context.py
--rw-r--r--   0        0        0     5981 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/config.py
--rw-r--r--   0        0        0     8043 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/decorator.py
--rw-r--r--   0        0        0     1617 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/docstring.lark
--rw-r--r--   0        0        0    19158 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/error_contexts.py
--rw-r--r--   0        0        0     2624 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/exceptions.py
--rw-r--r--   0        0        0     2561 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/inheritance.py
--rw-r--r--   0        0        0        0 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/__init__.py
--rw-r--r--   0        0        0     3046 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/tf.py
--rw-r--r--   0        0        0     2297 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/tfp.py
--rw-r--r--   0        0        0     1317 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/integration/torch.py
--rw-r--r--   0        0        0    25108 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/parser.py
--rw-r--r--   0        0        0        0 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/py.typed
--rw-r--r--   0        0        0     3374 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/shapes.py
--rw-r--r--   0        0        0     3226 2023-08-03 14:20:56.824118 check_shapes-1.1.0/check_shapes/specs.py
--rw-r--r--   0        0        0     4390 2023-08-03 14:20:56.828118 check_shapes-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 check_shapes-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-04 08:23:26.500158 check_shapes-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1147 2023-08-04 08:23:26.500158 check_shapes-1.1.1/README.md
+-rw-r--r--   0        0        0     2436 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/__init__.py
+-rw-r--r--   0        0        0     1756 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/accessors.py
+-rw-r--r--   0        0        0     6712 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/argument_ref.py
+-rw-r--r--   0        0        0     1106 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/base_types.py
+-rw-r--r--   0        0        0     4213 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/bool_specs.py
+-rw-r--r--   0        0        0     2908 2023-08-04 08:23:26.500158 check_shapes-1.1.1/check_shapes/check_shapes.lark
+-rw-r--r--   0        0        0    22338 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/checker.py
+-rw-r--r--   0        0        0     2775 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/checker_context.py
+-rw-r--r--   0        0        0     5981 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/config.py
+-rw-r--r--   0        0        0     8043 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/decorator.py
+-rw-r--r--   0        0        0     1617 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/docstring.lark
+-rw-r--r--   0        0        0    19158 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/error_contexts.py
+-rw-r--r--   0        0        0     2624 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/exceptions.py
+-rw-r--r--   0        0        0     2561 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/inheritance.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/integration/__init__.py
+-rw-r--r--   0        0        0     3046 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/integration/tf.py
+-rw-r--r--   0        0        0     2297 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/integration/tfp.py
+-rw-r--r--   0        0        0     1317 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/integration/torch.py
+-rw-r--r--   0        0        0    25108 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/parser.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/py.typed
+-rw-r--r--   0        0        0     3374 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/shapes.py
+-rw-r--r--   0        0        0     3226 2023-08-04 08:23:26.504155 check_shapes-1.1.1/check_shapes/specs.py
+-rw-r--r--   0        0        0     4390 2023-08-04 08:23:26.508152 check_shapes-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 check_shapes-1.1.1/PKG-INFO
```

### Comparing `check_shapes-1.1.0/LICENSE` & `check_shapes-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/README.md` & `check_shapes-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/__init__.py` & `check_shapes-1.1.1/check_shapes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from .integration.torch import install_torch_integration
 from .shapes import get_shape, register_get_shape
 
 install_tf_integration()
 install_tfp_integration()
 install_torch_integration()
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 __all__ = [
     "Dimension",
     "DocstringFormat",
     "ErrorContext",
     "Shape",
     "ShapeChecker",
```

### Comparing `check_shapes-1.1.0/check_shapes/accessors.py` & `check_shapes-1.1.1/check_shapes/accessors.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/argument_ref.py` & `check_shapes-1.1.1/check_shapes/argument_ref.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/base_types.py` & `check_shapes-1.1.1/check_shapes/base_types.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/bool_specs.py` & `check_shapes-1.1.1/check_shapes/bool_specs.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/check_shapes.lark` & `check_shapes-1.1.1/check_shapes/check_shapes.lark`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/checker.py` & `check_shapes-1.1.1/check_shapes/checker.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/checker_context.py` & `check_shapes-1.1.1/check_shapes/checker_context.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/config.py` & `check_shapes-1.1.1/check_shapes/config.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/decorator.py` & `check_shapes-1.1.1/check_shapes/decorator.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/docstring.lark` & `check_shapes-1.1.1/check_shapes/docstring.lark`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/error_contexts.py` & `check_shapes-1.1.1/check_shapes/error_contexts.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/exceptions.py` & `check_shapes-1.1.1/check_shapes/exceptions.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/inheritance.py` & `check_shapes-1.1.1/check_shapes/inheritance.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/integration/tf.py` & `check_shapes-1.1.1/check_shapes/integration/tf.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/integration/tfp.py` & `check_shapes-1.1.1/check_shapes/integration/tfp.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/integration/torch.py` & `check_shapes-1.1.1/check_shapes/integration/torch.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/parser.py` & `check_shapes-1.1.1/check_shapes/parser.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/shapes.py` & `check_shapes-1.1.1/check_shapes/shapes.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/check_shapes/specs.py` & `check_shapes-1.1.1/check_shapes/specs.py`

 * *Files identical despite different names*

### Comparing `check_shapes-1.1.0/pyproject.toml` & `check_shapes-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "check_shapes"
-version = "1.1.0"
+version = "1.1.1"
 description = "A library for annotating and checking the shapes of tensors."
 authors = [
     "Jesper Nielsen <jespernielsen1982+check_shapes@gmail.com>",
     "The GPflow Contributors",
 ]
 license = "Apache-2.0"
 
@@ -28,22 +28,22 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Debuggers",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
+dropstackframe = ">=0.1.0"
 lark = "^1.1.0"
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^5.2.2"
 black = "20.8b1"  # Pinned for backwards compatibility with the old stuff.
 click = "<8.1.0"  # Required by `black = "20.8b1"`.
-dropstackframe = ">=0.1.0"
 isort = "^5.10.0"
 matplotlib = "^3.0.0"
 mypy = ">0.920,!=0.982"
 numpy = "<1.22.0"  # MyPy is unhappy about Python 3.7 and newer versions of NumPy.
 # Pandas constrained to reduce Poetry search-time. Feel free to loosen this when we no longer need
 # to support Python 3.7:
 pandas = ">=1.1.0,<1.4.0"
```

### Comparing `check_shapes-1.1.0/PKG-INFO` & `check_shapes-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-shapes
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for annotating and checking the shapes of tensors.
 Home-page: https://gpflow.github.io/check_shapes
 License: Apache-2.0
 Author: Jesper Nielsen
 Author-email: jespernielsen1982+check_shapes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Typing :: Typed
+Requires-Dist: dropstackframe (>=0.1.0)
 Requires-Dist: lark (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://gpflow.github.io/check_shapes
 Project-URL: Repository, https://github.com/GPflow/check_shapes
 Description-Content-Type: text/markdown
 
 # check_shapes
```

