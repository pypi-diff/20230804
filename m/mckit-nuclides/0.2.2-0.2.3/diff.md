# Comparing `tmp/mckit_nuclides-0.2.2.tar.gz` & `tmp/mckit_nuclides-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckit_nuclides-0.2.2.tar", max compression
+gzip compressed data, was "mckit_nuclides-0.2.3.tar", max compression
```

## Comparing `mckit_nuclides-0.2.2.tar` & `mckit_nuclides-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-06-19 11:26:09.801151 mckit_nuclides-0.2.2/LICENSE
--rw-r--r--   0        0        0     3281 2023-06-19 11:26:09.801151 mckit_nuclides-0.2.2/README.rst
--rw-r--r--   0        0        0    16503 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      752 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/__init__.py
--rw-r--r--   0        0        0     1647 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/abundance.py
--rw-r--r--   0        0        0    13595 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/data/elements.csv
--rw-r--r--   0        0        0   717942 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt
--rw-r--r--   0        0        0     3255 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/elements.py
--rw-r--r--   0        0        0     3113 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/nuclides.py
--rw-r--r--   0        0        0        0 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/py.typed
--rw-r--r--   0        0        0       20 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/utils/__init__.py
--rw-r--r--   0        0        0      768 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/utils/resource.py
--rw-r--r--   0        0        0     4504 1970-01-01 00:00:00.000000 mckit_nuclides-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-04 12:36:47.856833 mckit_nuclides-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3281 2023-08-04 12:36:47.856833 mckit_nuclides-0.2.3/README.rst
+-rw-r--r--   0        0        0    16397 2023-08-04 12:37:06.953092 mckit_nuclides-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/__init__.py
+-rw-r--r--   0        0        0     1647 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/abundance.py
+-rw-r--r--   0        0        0    13595 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/data/elements.csv
+-rw-r--r--   0        0        0    70652 2023-08-04 12:37:06.953092 mckit_nuclides-0.2.3/src/mckit_nuclides/data/half-lifes.csv
+-rw-r--r--   0        0        0   717942 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt
+-rw-r--r--   0        0        0     3255 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/elements.py
+-rw-r--r--   0        0        0     3076 2023-08-04 12:37:06.953092 mckit_nuclides-0.2.3/src/mckit_nuclides/nuclides.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/py.typed
+-rw-r--r--   0        0        0       20 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/utils/__init__.py
+-rw-r--r--   0        0        0      768 2023-08-04 12:36:47.868833 mckit_nuclides-0.2.3/src/mckit_nuclides/utils/resource.py
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 mckit_nuclides-0.2.3/PKG-INFO
```

### Comparing `mckit_nuclides-0.2.2/LICENSE` & `mckit_nuclides-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/README.rst` & `mckit_nuclides-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/pyproject.toml` & `mckit_nuclides-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mckit-nuclides"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python tools to work with elements and isotopes"
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/mckit-nuclides"
 repository = "https://github.com/MC-kit/mckit-nuclides"
 # documentation = "https://mckit-nuclides.readthedocs.io
 keywords = [
@@ -37,15 +37,15 @@
 
 [tool.poetry.urls]
 # documentation = "https://mckit_nuclides.readthedocs.io"
 Changelog = "https://github.com/MC-kit/mckit-nuclides/releases"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 importlib-resources = {version = ">=5.12.0", python = "3.8"}
 numpy = ">=1.24.2"
 openpyxl = ">=3.0.9"
 pandas = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
@@ -61,25 +61,25 @@
 
 [tool.poetry.group.pre_commit.dependencies]
 pre-commit = ">=2.15.0"
 rstcheck = ">=3.3.1"
 pydocstringformatter = ">=0.7.3"
 
 [tool.poetry.group.black.dependencies]
-black = ">=22.8.0"  #TODO dvp: update with safety and packaging
+black = ">=22.8.0"
 
 [tool.poetry.group.isort.dependencies]
 isort = ">=5.9.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.1"
-pytest-cache = ">=1.0"
+# pytest-cache = ">=1.0"
 pytest-cov = ">=4.0"
-pytest-mock = ">=3.9"
-pytest-randomly = ">=3.12"
+# pytest-mock = ">=3.9"
+# pytest-randomly = ">=3.12"
 coverage = { version = ">=6.1.2", extras = ["toml"] }
 
 [tool.poetry.group.coverage.dependencies]
 coverage = { version = ">=6.1.2", extras = ["toml"] }
 
 [tool.poetry.group.xdoctest.dependencies]
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
@@ -117,16 +117,14 @@
 flake8-pie = ">=0.16.0"
 flake8-print = ">=5.0.0"
 flake8-rst-docstrings = ">=0.2.7"
 flake8-scream = ">=0.1.0"
 flake8-simplify = ">=0.19.3"
 flake8-use-fstring = ">=1.4"
 flake8-use-pathlib = ">=0.3.0"
-pandas-vet = ">=0.2.3"
-tryceratops = ">=1.0.1"
 pylint = ">=2.15.10"
 flake8-pylint = ">=0.1.3"
 # TODO dvp: check/use flake8-pyprojecttoml plugin
 # https://gitlab.com/durko/flake8-pyprojecttoml/-/blob/master/pyproject.toml
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=6.1.3"
@@ -222,15 +220,14 @@
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.xdoctest]
 quiet = true
 options = ""
 
-# [tool.coverage]
 [tool.coverage.paths]
 source = ["src", ".nox/*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["src"]
 omit = ["*_tab.py", "**/__init__.py"]
```

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/__init__.py` & `mckit_nuclides-0.2.3/src/mckit_nuclides/__init__.py`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/abundance.py` & `mckit_nuclides-0.2.3/src/mckit_nuclides/abundance.py`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/data/elements.csv` & `mckit_nuclides-0.2.3/src/mckit_nuclides/data/elements.csv`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt` & `mckit_nuclides-0.2.3/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/elements.py` & `mckit_nuclides-0.2.3/src/mckit_nuclides/elements.py`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/nuclides.py` & `mckit_nuclides-0.2.3/src/mckit_nuclides/nuclides.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,18 @@
     collector["atomic_symbol"] = symbols
     nuclides_table = pd.DataFrame.from_dict(collector)
     nuclides_table = nuclides_table.set_index(
         ["atomic_number", "mass_number"],
         verify_integrity=True,
     )
     nuclides_table.index.name = "atom_and_mass_numbers"
-    nuclides_table = nuclides_table.rename(
+    return nuclides_table.rename(
         columns={"atomic_symbol": "symbol", "relative_atomic_mass": "nuclide_mass"},
     )
 
-    return nuclides_table
-
 
 def _load_nist_file() -> dict[str, list[Any]]:
     collector: dict[str, list[Any]] = {
         "atomic_number": [],
         "atomic_symbol": [],
         "mass_number": [],
         "relative_atomic_mass": [],
```

### Comparing `mckit_nuclides-0.2.2/src/mckit_nuclides/utils/resource.py` & `mckit_nuclides-0.2.3/src/mckit_nuclides/utils/resource.py`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.2/PKG-INFO` & `mckit_nuclides-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mckit-nuclides
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python tools to work with elements and isotopes
 Home-page: https://github.com/MC-kit/mckit-nuclides
 License: MIT
 Keywords: element,nuclide,isotope,abundance
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

