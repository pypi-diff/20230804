# Comparing `tmp/jijmodeling_transpiler_quantum-0.1.0rc2.tar.gz` & `tmp/jijmodeling_transpiler_quantum-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jijmodeling_transpiler_quantum-0.1.0rc2.tar", max compression
+gzip compressed data, was "jijmodeling_transpiler_quantum-0.1.0rc3.tar", max compression
```

## Comparing `jijmodeling_transpiler_quantum-0.1.0rc2.tar` & `jijmodeling_transpiler_quantum-0.1.0rc3.tar`

### file list

```diff
@@ -1,9 +1,26 @@
--rw-r--r--   0        0        0     1756 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/README.md
--rw-r--r--   0        0        0        0 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/__init__.py
--rw-r--r--   0        0        0      337 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/__init__.py
--rw-r--r--   0        0        0      147 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/ising_qubo/__init__.py
--rw-r--r--   0        0        0     2474 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py
--rw-r--r--   0        0        0      248 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/qrac/__init__.py
--rw-r--r--   0        0        0     2309 2023-07-18 10:43:51.839950 jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py
--rw-r--r--   0        0        0      684 2023-07-18 13:43:51.419322 jijmodeling_transpiler_quantum-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 jijmodeling_transpiler_quantum-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1756 2023-08-02 14:30:10.299222 jijmodeling_transpiler_quantum-0.1.0rc3/README.md
+-rw-r--r--   0        0        0      337 2023-08-02 14:30:10.299435 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-02 14:30:10.299605 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/__init__.py
+-rw-r--r--   0        0        0     2474 2023-08-02 14:30:10.299919 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py
+-rw-r--r--   0        0        0      248 2023-08-02 14:30:10.300095 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/__init__.py
+-rw-r--r--   0        0        0     2309 2023-08-02 14:30:10.300218 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py
+-rw-r--r--   0        0        0      610 2023-08-02 14:30:10.302724 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/__init__.py
+-rw-r--r--   0        0        0      185 2023-08-02 14:30:10.302882 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/__init__.py
+-rw-r--r--   0        0        0     1536 2023-08-02 14:30:10.303002 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/ising_hamiltonian.py
+-rw-r--r--   0        0        0     3572 2023-08-02 14:30:10.303138 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      501 2023-08-02 14:30:10.303305 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/__init__.py
+-rw-r--r--   0        0        0     1808 2023-08-02 14:30:10.303450 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao21.py
+-rw-r--r--   0        0        0     3180 2023-08-02 14:30:10.303580 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao31.py
+-rw-r--r--   0        0        0     4448 2023-08-02 14:30:10.303724 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao32.py
+-rw-r--r--   0        0        0     2523 2023-08-02 14:30:10.303948 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao_space_efficient.py
+-rw-r--r--   0        0        0    10633 2023-08-02 14:30:10.304219 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/to_qrac.py
+-rw-r--r--   0        0        0      360 2023-08-02 14:30:10.307220 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/__init__.py
+-rw-r--r--   0        0        0      175 2023-08-02 14:30:10.307501 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/__init__.py
+-rw-r--r--   0        0        0     1625 2023-08-02 14:30:10.307729 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/ising_hamiltonian.py
+-rw-r--r--   0        0        0     6490 2023-08-02 14:30:10.307927 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      427 2023-08-02 14:30:10.308212 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/__init__.py
+-rw-r--r--   0        0        0     2169 2023-08-02 14:30:10.308446 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao21.py
+-rw-r--r--   0        0        0     3615 2023-08-02 14:30:10.308622 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao31.py
+-rw-r--r--   0        0        0     5720 2023-08-02 14:30:10.308810 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/to_qrac.py
+-rw-r--r--   0        0        0      795 2023-08-02 14:44:41.233557 jijmodeling_transpiler_quantum-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 jijmodeling_transpiler_quantum-0.1.0rc3/PKG-INFO
```

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc2/README.md` & `jijmodeling_transpiler_quantum-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py` & `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc2/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py` & `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc2/pyproject.toml` & `jijmodeling_transpiler_quantum-0.1.0rc3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "jijmodeling-transpiler-quantum"
-version = "0.1.0rc2"
+version = "0.1.0rc3"
 description = ""
 authors = ["Jij Inc."]
 readme = "README.md"
 packages = [
     {include = "jijmodeling_transpiler_quantum"},
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9.8,<3.11"
 jijmodeling-transpiler = "^0.6.0rc2"
+qiskit = {version = "^0.44.0", extras = ["qiskit"]}
+quri-parts = {version = "^0.13.0", extras = ["quri-parts"]}
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 matplotlib = "^3.7.1"
 pylatexenc = "^2.10"
 pytest = "^7.3.2"
 
 [tool.poetry.extras]
-qiskit = ["jijmodeling-transpiler-quantum-qiskit"]
+qiskit = ["qiskit"]
+quri-parts = ["quri-parts"]
 
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
```

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc2/PKG-INFO` & `jijmodeling_transpiler_quantum-0.1.0rc3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: jijmodeling-transpiler-quantum
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: 
 Author: Jij Inc.
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9.8,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: qiskit
+Provides-Extra: quri-parts
 Requires-Dist: jijmodeling-transpiler (>=0.6.0rc2,<0.7.0)
+Requires-Dist: qiskit[qiskit] (>=0.44.0,<0.45.0) ; extra == "qiskit"
+Requires-Dist: quri-parts[quri-parts] (>=0.13.0,<0.14.0) ; extra == "quri-parts"
 Description-Content-Type: text/markdown
 
 # JijModeling-Transpiler-Quantum
 
 `JijModeling-Transpiler-Quantum` is a transpiler from model written in [JijModeling]() to quantum optimization algorithms on variaous quantum platform.
 
 ## Installation
```

