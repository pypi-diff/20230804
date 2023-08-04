# Comparing `tmp/cosimtlk-0.1.0.tar.gz` & `tmp/cosimtlk-0.1.1.tar.gz`

## Comparing `cosimtlk-0.1.0.tar` & `cosimtlk-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/Makefile
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/README.md
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/__version__.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/models.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/py.typed
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/simulator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/__init__.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/config.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/dependencies.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/main.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/routers/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/routers/simulation.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/src/cosimtlk/app/routers/simulators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/tests/test_simulator.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/.gitignore
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/LICENCE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/README.md
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 cosimtlk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/Makefile
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/README.md
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/__version__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/models.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/py.typed
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/simulator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/__init__.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/client.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/config.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/dependencies.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/main.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/routers/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/routers/simulation.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/src/cosimtlk/app/routers/simulators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/tests/test_simulator.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/LICENCE
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/README.md
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 cosimtlk-0.1.1/PKG-INFO
```

### Comparing `cosimtlk-0.1.0/Makefile` & `cosimtlk-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/README.md` & `cosimtlk-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Cosimulation toolkit
 ====================
 
-[![PyPI version](https://badge.fury.io/py/enfobench.svg)](https://badge.fury.io/py/enfobench)
+[![PyPI version](https://badge.fury.io/py/cosimtlk.svg)](https://badge.fury.io/py/cosimtlk)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
```

### Comparing `cosimtlk-0.1.0/pyproject.toml` & `cosimtlk-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "attrs>=23.0.0",
     "fmpy",
     "fastapi>=0.68.0,<1.0.0",
     "requests>=2.26.0,<3.0.0",
+    "pydantic-settings>=2.0.0",
     "uvicorn>=0.20.0,<1.0.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/attila-balint-kul/cosimulation-toolkit"
```

### Comparing `cosimtlk-0.1.0/src/cosimtlk/models.py` & `cosimtlk-0.1.1/src/cosimtlk/models.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/simulator.py` & `cosimtlk-0.1.1/src/cosimtlk/simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/client.py` & `cosimtlk-0.1.1/src/cosimtlk/app/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/dependencies.py` & `cosimtlk-0.1.1/src/cosimtlk/app/dependencies.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/main.py` & `cosimtlk-0.1.1/src/cosimtlk/app/main.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/schemas.py` & `cosimtlk-0.1.1/src/cosimtlk/app/schemas.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/routers/simulation.py` & `cosimtlk-0.1.1/src/cosimtlk/app/routers/simulation.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/src/cosimtlk/app/routers/simulators.py` & `cosimtlk-0.1.1/src/cosimtlk/app/routers/simulators.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/tests/test_simulator.py` & `cosimtlk-0.1.1/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/.gitignore` & `cosimtlk-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/LICENCE` & `cosimtlk-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.1.0/PKG-INFO` & `cosimtlk-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosimtlk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cosimulation toolkit.
 Project-URL: Homepage, https://github.com/attila-balint-kul/cosimulation-toolkit
 Author-email: attila.balint@kuleuven.be
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: attrs>=23.0.0
 Requires-Dist: fastapi<1.0.0,>=0.68.0
 Requires-Dist: fmpy
+Requires-Dist: pydantic-settings>=2.0.0
 Requires-Dist: requests<3.0.0,>=2.26.0
 Requires-Dist: uvicorn<1.0.0,>=0.20.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<4.0.0,>=3.0.0; extra == 'dev'
 Requires-Dist: twine<5.0.0,>=4.0.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black==23.3.0; extra == 'test'
@@ -34,15 +35,15 @@
 Requires-Dist: pytest==7.3.2; extra == 'test'
 Requires-Dist: ruff==0.0.274; extra == 'test'
 Description-Content-Type: text/markdown
 
 Cosimulation toolkit
 ====================
 
-[![PyPI version](https://badge.fury.io/py/enfobench.svg)](https://badge.fury.io/py/enfobench)
+[![PyPI version](https://badge.fury.io/py/cosimtlk.svg)](https://badge.fury.io/py/cosimtlk)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
```

