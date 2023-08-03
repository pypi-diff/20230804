# Comparing `tmp/equation-sampler-0.0.2.tar.gz` & `tmp/equation-sampler-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equation-sampler-0.0.2.tar", last modified: Tue Aug  1 22:22:02 2023, max compression
+gzip compressed data, was "equation-sampler-0.0.3.tar", last modified: Thu Aug  3 22:03:19 2023, max compression
```

## Comparing `equation-sampler-0.0.2.tar` & `equation-sampler-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/src/equation_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/src/equation_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19615 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/src/equation_sampler/equation_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/src/equation_sampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/test_equation_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/test_equation_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.297590 equation-sampler-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.297590 equation-sampler-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.297590 equation-sampler-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.297590 equation-sampler-0.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.297590 equation-sampler-0.0.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.293590 equation-sampler-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/src/equation_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/src/equation_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19615 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/src/equation_sampler/equation_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/src/equation_sampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-03 22:03:19.000000 equation-sampler-0.0.3/src/equation_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 22:03:19.000000 equation-sampler-0.0.3/src/equation_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:03:19.000000 equation-sampler-0.0.3/src/equation_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 22:03:19.000000 equation-sampler-0.0.3/src/equation_sampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 22:03:19.000000 equation-sampler-0.0.3/src/equation_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:19.301591 equation-sampler-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/tests/test_equation_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-03 22:03:06.000000 equation-sampler-0.0.3/tests/test_equation_tree.py
```

### Comparing `equation-sampler-0.0.2/.github/pull_request_template.md` & `equation-sampler-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/.github/workflows/python-publish.yml` & `equation-sampler-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/.gitignore` & `equation-sampler-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/.pre-commit-config.yaml` & `equation-sampler-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/PKG-INFO` & `equation-sampler-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-sampler
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to sample equations
 Author-email: Ioana Marinescu <ioanam@princeton.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic-generator-equation-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `equation-sampler-0.0.2/README.md` & `equation-sampler-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/docs/Additional Example.ipynb` & `equation-sampler-0.0.3/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/docs/Basic Usage.ipynb` & `equation-sampler-0.0.3/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/docs/index.md` & `equation-sampler-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/mkdocs/base.yml` & `equation-sampler-0.0.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/pyproject.toml` & `equation-sampler-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/src/equation_sampler/__init__.py` & `equation-sampler-0.0.3/src/equation_sampler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 
 import numpy as np
 from sympy import simplify
 
-from .equation_tree import EquationTree, is_binary_tree, rooted_tree_iterator
+from src.equation_sampler.equation_tree import EquationTree, is_binary_tree, rooted_tree_iterator
 
 padding = "<PAD>"
 
 
 def prefix_to_infix(prefix, function_space, operation_space):
     stack = []
     for i in range(len(prefix) - 1, -1, -1):
@@ -373,13 +373,35 @@
 
     if transpose:
         evaluation = evaluation.T
 
     return evaluation
 
 
+def to_sympy(equations: list, function_space: list, operator_space: list):
+    """
+    Helper function to transform the output from an equation sampler into sympy readable format
+
+    Args:
+        equations: output of sample_equations
+        function_space: function space used in sample_equations
+        operator_space: operator space used in sample_equations
+
+    Returns:
+
+    """
+    res = equations
+    for i in range(len(res[0])):
+        res[0][i] = simplify(prefix_to_infix(res[0][i], function_space, operator_space))
+    return res
+
+
 def is_numeric(s):
     try:
         float(s)
         return True
     except ValueError:
         return False
+
+
+
+
```

### Comparing `equation-sampler-0.0.2/src/equation_sampler/equation_tree.py` & `equation-sampler-0.0.3/src/equation_sampler/equation_tree.py`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/src/equation_sampler.egg-info/PKG-INFO` & `equation-sampler-0.0.3/src/equation_sampler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-sampler
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to sample equations
 Author-email: Ioana Marinescu <ioanam@princeton.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic-generator-equation-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `equation-sampler-0.0.2/src/equation_sampler.egg-info/SOURCES.txt` & `equation-sampler-0.0.3/src/equation_sampler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/tests/README.md` & `equation-sampler-0.0.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/tests/test_equation_sampler.py` & `equation-sampler-0.0.3/tests/test_equation_sampler.py`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.2/tests/test_equation_tree.py` & `equation-sampler-0.0.3/tests/test_equation_tree.py`

 * *Files identical despite different names*

