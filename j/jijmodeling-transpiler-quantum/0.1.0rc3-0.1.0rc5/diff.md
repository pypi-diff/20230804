# Comparing `tmp/jijmodeling_transpiler_quantum-0.1.0rc3.tar.gz` & `tmp/jijmodeling_transpiler_quantum-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jijmodeling_transpiler_quantum-0.1.0rc3.tar", max compression
+gzip compressed data, was "jijmodeling_transpiler_quantum-0.1.0rc5.tar", max compression
```

## Comparing `jijmodeling_transpiler_quantum-0.1.0rc3.tar` & `jijmodeling_transpiler_quantum-0.1.0rc5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1756 2023-08-02 14:30:10.299222 jijmodeling_transpiler_quantum-0.1.0rc3/README.md
--rw-r--r--   0        0        0      337 2023-08-02 14:30:10.299435 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/__init__.py
--rw-r--r--   0        0        0      147 2023-08-02 14:30:10.299605 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/__init__.py
--rw-r--r--   0        0        0     2474 2023-08-02 14:30:10.299919 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py
--rw-r--r--   0        0        0      248 2023-08-02 14:30:10.300095 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/__init__.py
--rw-r--r--   0        0        0     2309 2023-08-02 14:30:10.300218 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py
--rw-r--r--   0        0        0      610 2023-08-02 14:30:10.302724 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/__init__.py
--rw-r--r--   0        0        0      185 2023-08-02 14:30:10.302882 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/__init__.py
--rw-r--r--   0        0        0     1536 2023-08-02 14:30:10.303002 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/ising_hamiltonian.py
--rw-r--r--   0        0        0     3572 2023-08-02 14:30:10.303138 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/to_qaoa.py
--rw-r--r--   0        0        0      501 2023-08-02 14:30:10.303305 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/__init__.py
--rw-r--r--   0        0        0     1808 2023-08-02 14:30:10.303450 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao21.py
--rw-r--r--   0        0        0     3180 2023-08-02 14:30:10.303580 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao31.py
--rw-r--r--   0        0        0     4448 2023-08-02 14:30:10.303724 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao32.py
--rw-r--r--   0        0        0     2523 2023-08-02 14:30:10.303948 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao_space_efficient.py
--rw-r--r--   0        0        0    10633 2023-08-02 14:30:10.304219 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/to_qrac.py
--rw-r--r--   0        0        0      360 2023-08-02 14:30:10.307220 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/__init__.py
--rw-r--r--   0        0        0      175 2023-08-02 14:30:10.307501 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/__init__.py
--rw-r--r--   0        0        0     1625 2023-08-02 14:30:10.307729 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/ising_hamiltonian.py
--rw-r--r--   0        0        0     6490 2023-08-02 14:30:10.307927 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/to_qaoa.py
--rw-r--r--   0        0        0      427 2023-08-02 14:30:10.308212 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/__init__.py
--rw-r--r--   0        0        0     2169 2023-08-02 14:30:10.308446 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao21.py
--rw-r--r--   0        0        0     3615 2023-08-02 14:30:10.308622 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao31.py
--rw-r--r--   0        0        0     5720 2023-08-02 14:30:10.308810 jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/to_qrac.py
--rw-r--r--   0        0        0      795 2023-08-02 14:44:41.233557 jijmodeling_transpiler_quantum-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 jijmodeling_transpiler_quantum-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1718 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/README.md
+-rw-r--r--   0        0        0      337 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/__init__.py
+-rw-r--r--   0        0        0      147 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/ising_qubo/__init__.py
+-rw-r--r--   0        0        0     2474 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py
+-rw-r--r--   0        0        0      248 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/qrac/__init__.py
+-rw-r--r--   0        0        0     2309 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py
+-rw-r--r--   0        0        0      610 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/__init__.py
+-rw-r--r--   0        0        0      185 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qaoa/__init__.py
+-rw-r--r--   0        0        0     1536 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qaoa/ising_hamiltonian.py
+-rw-r--r--   0        0        0     3572 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      501 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/__init__.py
+-rw-r--r--   0        0        0     1808 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao21.py
+-rw-r--r--   0        0        0     3180 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao31.py
+-rw-r--r--   0        0        0     4448 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao32.py
+-rw-r--r--   0        0        0     2523 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao_space_efficient.py
+-rw-r--r--   0        0        0    10633 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/to_qrac.py
+-rw-r--r--   0        0        0      360 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/__init__.py
+-rw-r--r--   0        0        0      175 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qaoa/__init__.py
+-rw-r--r--   0        0        0     1625 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qaoa/ising_hamiltonian.py
+-rw-r--r--   0        0        0     6490 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      427 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/__init__.py
+-rw-r--r--   0        0        0     2169 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao21.py
+-rw-r--r--   0        0        0     3615 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao31.py
+-rw-r--r--   0        0        0     5720 2023-08-04 05:13:08.560042 jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/to_qrac.py
+-rw-r--r--   0        0        0      908 2023-08-04 05:13:32.624393 jijmodeling_transpiler_quantum-0.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 jijmodeling_transpiler_quantum-0.1.0rc5/PKG-INFO
```

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/README.md` & `jijmodeling_transpiler_quantum-0.1.0rc5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # JijModeling-Transpiler-Quantum
 
 `JijModeling-Transpiler-Quantum` is a transpiler from model written in [JijModeling]() to quantum optimization algorithms on variaous quantum platform.
 
-## Installation
-
-```bash
-pip install jijmodeling-transpiler-quantum
-```
+- [Qiskit](#qiskit)
+- [QURI-Parts](#quri-parts)
 
 ## Qiskit
 
 [Qiskit](https://qiskit.org/) is an open-source SDK for working with quantum computers at the level of circuits, algorithms, and application modules.
 
+### Installation
+
+```bash
+pip install "jijmodeling-transpiler-quantum[qiskit]"
+```
+
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
 ```python
 import jijmodeling as jm
 import jijmodeling_transpiler as jmt
 import jijmodeling_transpiler_quantum as jtq
 
@@ -29,23 +32,20 @@
 # Transpile to QAOA of qikit
 qaoa_builder = jtq.qiskit.transpile_to_qaoa(compiled_instance)
 ```
 
 
 ## QURI-Parts
 
-
-
-| ❌ Not supported yet.                         | 
-|------------------------------------------|
-| Currently, `quri-parts` is not supported. Please wait for the next release. |
-
-
 [QURI Parts](https://quri-parts.qunasys.com/) is an open source library suite for creating and executing quantum algorithms on various quantum computers and simulators.
 
+```bash
+pip install "jijmodeling-transpiler-quantum[quri-parts]"
+```
+
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
 ```python
 import jijmodeling as jm
 import jijmodeling_transpiler as jmt
 import jijmodeling_transpiler_quantum as jtq
 
@@ -63,15 +63,15 @@
 
 ## Contributing
 
 ### Setup
 
 ```bash
 pip install poetry
-poetry install
+poetry install --all-extras
 poetry shell
 ```
 
 ### Test
 
 ```bash
 pytest tests
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/ising_qubo/ising_qubo.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/core/qrac/graph_coloring.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/__init__.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/ising_hamiltonian.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qaoa/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qaoa/to_qaoa.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qaoa/to_qaoa.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao21.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao21.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao31.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao31.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao32.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao32.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/qrao_space_efficient.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/qrao_space_efficient.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/qiskit/qrao/to_qrac.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/qiskit/qrao/to_qrac.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/ising_hamiltonian.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qaoa/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qaoa/to_qaoa.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qaoa/to_qaoa.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao21.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao21.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao31.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/qrao31.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/jijmodeling_transpiler_quantum/quri_parts/qrao/to_qrac.py` & `jijmodeling_transpiler_quantum-0.1.0rc5/jijmodeling_transpiler_quantum/quri_parts/qrao/to_qrac.py`

 * *Files identical despite different names*

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/pyproject.toml` & `jijmodeling_transpiler_quantum-0.1.0rc5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
+requires = ["poetry-core>=1.5.2", "poetry-dynamic-versioning>=0.21.4"]
 build-backend = "poetry_dynamic_versioning.backend"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+style = "pep440"
+
 [tool.poetry]
 name = "jijmodeling-transpiler-quantum"
-version = "0.1.0rc3"
+version = "0.1.0rc5" # using poetry-dynamic-versioning
 description = ""
-authors = ["Jij Inc."]
+authors = ["Jij Inc. <info@j-ij.com>"]
 readme = "README.md"
 packages = [
     {include = "jijmodeling_transpiler_quantum"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.8,<3.11"
-jijmodeling-transpiler = "^0.6.0rc2"
-qiskit = {version = "^0.44.0", extras = ["qiskit"]}
-quri-parts = {version = "^0.13.0", extras = ["quri-parts"]}
+jijmodeling-transpiler = ">=0.6.0rc3"
+qiskit = {version = ">=0.44.0", extras = ["qiskit"]}
+quri-parts = {version = ">=0.13.0", extras = ["quri-parts"]}
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 matplotlib = "^3.7.1"
 pylatexenc = "^2.10"
 pytest = "^7.3.2"
```

### Comparing `jijmodeling_transpiler_quantum-0.1.0rc3/PKG-INFO` & `jijmodeling_transpiler_quantum-0.1.0rc5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: jijmodeling-transpiler-quantum
-Version: 0.1.0rc3
+Version: 0.1.0rc5
 Summary: 
 Author: Jij Inc.
+Author-email: info@j-ij.com
 Requires-Python: >=3.9.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: qiskit
 Provides-Extra: quri-parts
-Requires-Dist: jijmodeling-transpiler (>=0.6.0rc2,<0.7.0)
-Requires-Dist: qiskit[qiskit] (>=0.44.0,<0.45.0) ; extra == "qiskit"
-Requires-Dist: quri-parts[quri-parts] (>=0.13.0,<0.14.0) ; extra == "quri-parts"
+Requires-Dist: jijmodeling-transpiler (>=0.6.0rc3)
+Requires-Dist: qiskit[qiskit] (>=0.44.0) ; extra == "qiskit"
+Requires-Dist: quri-parts[quri-parts] (>=0.13.0) ; extra == "quri-parts"
 Description-Content-Type: text/markdown
 
 # JijModeling-Transpiler-Quantum
 
 `JijModeling-Transpiler-Quantum` is a transpiler from model written in [JijModeling]() to quantum optimization algorithms on variaous quantum platform.
 
-## Installation
-
-```bash
-pip install jijmodeling-transpiler-quantum
-```
+- [Qiskit](#qiskit)
+- [QURI-Parts](#quri-parts)
 
 ## Qiskit
 
 [Qiskit](https://qiskit.org/) is an open-source SDK for working with quantum computers at the level of circuits, algorithms, and application modules.
 
+### Installation
+
+```bash
+pip install "jijmodeling-transpiler-quantum[qiskit]"
+```
+
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
 ```python
 import jijmodeling as jm
 import jijmodeling_transpiler as jmt
 import jijmodeling_transpiler_quantum as jtq
 
@@ -44,23 +48,20 @@
 # Transpile to QAOA of qikit
 qaoa_builder = jtq.qiskit.transpile_to_qaoa(compiled_instance)
 ```
 
 
 ## QURI-Parts
 
-
-
-| ❌ Not supported yet.                         | 
-|------------------------------------------|
-| Currently, `quri-parts` is not supported. Please wait for the next release. |
-
-
 [QURI Parts](https://quri-parts.qunasys.com/) is an open source library suite for creating and executing quantum algorithms on various quantum computers and simulators.
 
+```bash
+pip install "jijmodeling-transpiler-quantum[quri-parts]"
+```
+
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
 ```python
 import jijmodeling as jm
 import jijmodeling_transpiler as jmt
 import jijmodeling_transpiler_quantum as jtq
 
@@ -78,15 +79,15 @@
 
 ## Contributing
 
 ### Setup
 
 ```bash
 pip install poetry
-poetry install
+poetry install --all-extras
 poetry shell
 ```
 
 ### Test
 
 ```bash
 pytest tests
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

