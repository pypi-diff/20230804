# Comparing `tmp/conda-forge-metadata-0.5.0.tar.gz` & `tmp/conda-forge-metadata-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-forge-metadata-0.5.0.tar", last modified: Wed May 17 18:41:28 2023, max compression
+gzip compressed data, was "conda-forge-metadata-0.5.1.tar", last modified: Fri Aug  4 16:05:58 2023, max compression
```

## Comparing `conda-forge-metadata-0.5.0.tar` & `conda-forge-metadata-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.760373 conda-forge-metadata-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/conda_forge_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/info_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/import_to_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/conda_forge_metadata/oci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.768374 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 18:41:28.000000 conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:28.772374 conda-forge-metadata-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_info_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_map_import_to_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-17 18:41:05.000000 conda-forge-metadata-0.5.0/tests/test_map_pypi_to_conda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.480323 conda-forge-metadata-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/info_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/import_to_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_info_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_map_import_to_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_map_pypi_to_conda.py
```

### Comparing `conda-forge-metadata-0.5.0/.github/workflows/pypi.yml` & `conda-forge-metadata-0.5.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/.github/workflows/tests.yml` & `conda-forge-metadata-0.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/.gitignore` & `conda-forge-metadata-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/.pre-commit-config.yaml` & `conda-forge-metadata-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/LICENSE` & `conda-forge-metadata-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/PKG-INFO` & `conda-forge-metadata-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.5.0
+Version: 0.5.1
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/artifact_info/info_json.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/info_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+from __future__ import annotations
+
 from conda_forge_metadata.libcfgraph import get_libcfgraph_artifact_data
+from conda_forge_metadata.types import ArtifactData
 
 
-def get_artifact_info_as_json(channel, subdir, artifact, backend="libcfgraph"):
+def get_artifact_info_as_json(
+    channel: str, subdir: str, artifact: str, backend: str = "libcfgraph"
+) -> ArtifactData | None:
     """Get a blob of artifact data from the conda info directory.
 
     Parameters
     ----------
     channel : str
         The channel (e.g., "conda-forge").
     subdir : str
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/import_to_pkg.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/import_to_pkg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from __future__ import annotations
+
 from functools import lru_cache
 
 import requests
 
 from conda_forge_metadata.libcfgraph import get_libcfgraph_pkgs_for_import
 
 
 @lru_cache(maxsize=1)
-def _ranked_hubs_authorities():
+def _ranked_hubs_authorities() -> list[str]:
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/ranked_hubs_authorities.json"
     )
     req.raise_for_status()
     return req.json()
 
 
-def map_import_to_package(import_name):
+def map_import_to_package(import_name: str) -> str:
     """Map an import name to the most likely package that has it.
 
     Parameters
     ----------
     import_name : str
         The name of the import.
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+from __future__ import annotations
+
+import typing
 from functools import lru_cache
 
 import requests
 from ruamel import yaml
 
+if typing.TYPE_CHECKING:
+    from ..types import CondaPackageName, NameMappingEntry, PypiPackageName
+
 
 @lru_cache(maxsize=1)
-def get_pypi_name_mapping():
+def get_pypi_name_mapping() -> list[NameMappingEntry]:
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/mappings/pypi/name_mapping.yaml"
     )
     req.raise_for_status()
     return yaml.YAML(typ="safe").load(req.text)
 
 
 @lru_cache(maxsize=1)
-def get_grayskull_pypi_mapping():
+def get_grayskull_pypi_mapping() -> dict[PypiPackageName, NameMappingEntry]:
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/mappings/pypi/grayskull_pypi_mapping.json"
     )
     req.raise_for_status()
     return req.json()
 
 
-def map_pypi_to_conda(pypi_name):
+def map_pypi_to_conda(pypi_name: PypiPackageName) -> CondaPackageName:
     """Map a package's PyPi name to the most likely Conda name.
 
     Parameters
     ----------
     pypi_name : str
         The name on PyPi. This is case-sensitive.
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/feedstock_outputs.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/feedstock_outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from functools import lru_cache
+from typing import Any, TypedDict
 
 import requests
 
+from conda_forge_metadata.types import CondaPackageName
+
+
+class FeedstockOutputsConfig(TypedDict):
+    outputs_path: str
+    shard_level: int
+    shard_fill: str
+
 
 @lru_cache(maxsize=1)
-def feedstock_outputs_config():
+def feedstock_outputs_config() -> FeedstockOutputsConfig:
     ref = "main"
     req = requests.get(
         "https://raw.githubusercontent.com/conda-forge/feedstock-outputs/"
         f"{ref}/config.json"
     )
     req.raise_for_status()
     return req.json()
 
 
-def sharded_path(name) -> str:
+def sharded_path(name: CondaPackageName) -> str:
     """
     Get the path to the sharded JSON path in the feedstock_outputs repository.
 
     Parameters
     ----------
     name : str
         The name of the package.
@@ -41,28 +50,28 @@
     while len(chars) < shard_level:
         chars.append(shard_fill)
 
     return f"{outputs_path}/{'/'.join(chars)}/{name}.json"
 
 
 @lru_cache(maxsize=1024)
-def package_to_feedstock(name, **request_kwargs):
+def package_to_feedstock(name: CondaPackageName, **request_kwargs: Any) -> str:
     """Map a package name to the feedstock name(s).
 
     Parameters
     ----------
     package : str
         The name of the package.
+    request_kwargs : dict
+        Keyword arguments to pass to ``requests.get``.
 
     Returns
     -------
     feedstock : str
         The name of the feedstock, without the ``-feedstock`` suffix.
-    request_kwargs : dict
-        Keyword arguments to pass to ``requests.get``.
     """
     assert name, "name must not be empty"
 
     ref = "main"
     path = sharded_path(name)
     req = requests.get(
         f"https://raw.githubusercontent.com/conda-forge/feedstock-outputs/{ref}/{path}",
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/libcfgraph.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/libcfgraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from __future__ import annotations
+
 from functools import lru_cache
 
 import requests
 
+from conda_forge_metadata.types import ArtifactData
+
 _LIBCFGRAPH_INDEX = None
 
 
 def _download_libcfgraph_index():
     global _LIBCFGRAPH_INDEX
     r = requests.get(
         "https://raw.githubusercontent.com/regro/libcfgraph"
@@ -19,32 +23,35 @@
             "https://raw.githubusercontent.com/regro/libcfgraph"
             "/master/.file_listing_%d.json" % i,
         )
         r.raise_for_status()
         _LIBCFGRAPH_INDEX += r.json()
 
 
-def get_libcfgraph_index():
+def get_libcfgraph_index() -> list[str]:
     """Get a list of all artifacts indexed by libcfgraph.
 
     Each element of the list looks like
 
         "artifacts/21cmfast/conda-forge/linux-64/21cmfast-3.0.2-py36h2e3f83d_0.json"
 
     for the conda-forge artifact
 
         linux-64/21cmfast-3.0.2-py36h2e3f83d_0.{tar.bz2,conda}
     """
     if _LIBCFGRAPH_INDEX is None:
         _download_libcfgraph_index()
+    assert _LIBCFGRAPH_INDEX is not None
     return _LIBCFGRAPH_INDEX
 
 
 @lru_cache(maxsize=1024)
-def get_libcfgraph_artifact_data(channel, subdir, artifact):
+def get_libcfgraph_artifact_data(
+    channel: str, subdir: str, artifact: str
+) -> ArtifactData | None:
     """Get a blob of artifact data from the conda info directory.
 
     Parameters
     ----------
     channel : str
         The channel (e.g., "conda-forge").
     subdir : str
@@ -95,41 +102,41 @@
         r.raise_for_status()
         return r.json()
     else:
         return None
 
 
 @lru_cache(maxsize=1)
-def _import_to_pkg_maps_num_letters():
+def _import_to_pkg_maps_num_letters() -> int:
     req = requests.get(
         "https://raw.githubusercontent.com/regro/libcfgraph/master"
         "/import_to_pkg_maps_meta.json"
     )
     req.raise_for_status()
     return int(req.json()["num_letters"])
 
 
 @lru_cache(maxsize=128)
-def _import_to_pkg_maps_cache(import_first_letters):
+def _import_to_pkg_maps_cache(import_first_letters: str) -> dict[str, set[str]]:
     req = requests.get(
         f"https://raw.githubusercontent.com/regro/libcfgraph"
         f"/master/import_to_pkg_maps/{import_first_letters.lower()}.json"
     )
     req.raise_for_status()
     return {k: set(v["elements"]) for k, v in req.json().items()}
 
 
-def _get_libcfgraph_pkgs_for_import(import_name):
+def _get_libcfgraph_pkgs_for_import(import_name: str) -> set[str] | None:
     num_letters = _import_to_pkg_maps_num_letters()
     fllt = import_name[: min(len(import_name), num_letters)]
     import_to_pkg_map = _import_to_pkg_maps_cache(fllt)
     return import_to_pkg_map.get(import_name, None)
 
 
-def get_libcfgraph_pkgs_for_import(import_name):
+def get_libcfgraph_pkgs_for_import(import_name: str) -> tuple[set[str] | None, str]:
     """Get a list of possible packages that supply a given import.
 
     **This data is approximate and may be wrong.**
 
     For a better guess, use the function
 
         `conda_forge_metadata.autotick_bot.map_import_to_package`
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata/oci.py` & `conda-forge-metadata-0.5.1/conda_forge_metadata/oci.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 import json
+import tarfile
 from functools import lru_cache
 from logging import getLogger
-from typing import Union
+from typing import Any
 
 from conda_oci_mirror.repo import PackageRepo
 from ruamel import yaml
 
+from conda_forge_metadata.types import ArtifactData
+
 logger = getLogger(__name__)
 
 
-def _extract_read(infotar, *names) -> Union[str, None]:
+def _extract_read(infotar: tarfile.TarFile, *names: str) -> str:
+    """
+    Extract a file from a tarfile and return its contents as a string.
+
+    Parameters
+    ----------
+    infotar : tarfile.TarFile
+        The tarfile to extract from.
+    names : str
+        The different names to try to extract. Only the first one found is
+        returned.
+    """
     names_in_tar = infotar.getnames()
     for name in names:
         if name in names_in_tar:
-            return infotar.extractfile(name).read().decode()
+            file = infotar.extractfile(name)
+            if file is not None:
+                return file.read().decode()
+    else:
+        raise ValueError(f"{names} not in {names_in_tar}")
 
 
 @lru_cache(maxsize=1024)
 def get_oci_artifact_data(
     channel: str,
     subdir: str,
     artifact: str,
     registry: str = "ghcr.io/channel-mirrors",
-) -> Union[dict, None]:
+) -> "ArtifactData | None":
     """Get a blob of artifact data from the conda info directory.
 
     Note this function might need token authentication to access the registry.
     Export the following environment variables:
     - ORAS_USER: the username to use for authentication
     - ORAS_PASS: the password/token to use for authentication
 
@@ -79,16 +97,15 @@
     try:
         infotar = repo.get_info(oci_name)
     except ValueError as exc:
         logger.debug("Failed to get info for %s", oci_name, exc_info=exc)
         return None
 
     YAML = yaml.YAML(typ="safe")
-
-    index = json.loads(_extract_read(infotar, "index.json"))
+    index: dict[str, Any] = json.loads(_extract_read(infotar, "index.json"))
     return {
         # https://github.com/regro/libcflib/blob/062858e90af2795d2eb098034728cace574a51b8/libcflib/harvester.py#L14
         "metadata_version": 1,
         "name": index.get("name", ""),
         "version": index.get("version", ""),
         "index": index,
         "about": json.loads(_extract_read(infotar, "about.json")),
@@ -97,16 +114,18 @@
         ),
         "raw_recipe": _extract_read(
             infotar,
             "recipe/meta.yaml.template",
             "recipe/meta.yaml",
             "meta.yaml",
         ),
-        "conda_build_config": YAML.load(
-            _extract_read(infotar, "recipe/conda_build_config.yaml")
+        "conda_build_config": (
+            YAML.load(_extract_read(infotar, "recipe/conda_build_config.yaml"))
+            if "recipe/conda_build_config.yaml" in infotar.getnames()
+            else {}
         ),
         "files": [
             f
             for f in _extract_read(infotar, "files").splitlines()
             if not f.lower().endswith((".pyc", ".txt"))
         ],
     }
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/PKG-INFO` & `conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.5.0
+Version: 0.5.1
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `conda-forge-metadata-0.5.0/conda_forge_metadata.egg-info/SOURCES.txt` & `conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+pyrightconfig.json
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/pre-commit.yml
 .github/workflows/pypi.yml
 .github/workflows/tests.yml
 conda_forge_metadata/__init__.py
 conda_forge_metadata/_version.py
 conda_forge_metadata/feedstock_outputs.py
 conda_forge_metadata/libcfgraph.py
 conda_forge_metadata/oci.py
+conda_forge_metadata/py.typed
+conda_forge_metadata/types.py
 conda_forge_metadata.egg-info/PKG-INFO
 conda_forge_metadata.egg-info/SOURCES.txt
 conda_forge_metadata.egg-info/dependency_links.txt
 conda_forge_metadata.egg-info/requires.txt
 conda_forge_metadata.egg-info/top_level.txt
 conda_forge_metadata/artifact_info/__init__.py
 conda_forge_metadata/artifact_info/info_json.py
```

### Comparing `conda-forge-metadata-0.5.0/pyproject.toml` & `conda-forge-metadata-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.0/tests/test_libcfgraph.py` & `conda-forge-metadata-0.5.1/tests/test_libcfgraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 def test_get_libcfgraph_artifact_data():
     data = get_libcfgraph_artifact_data(
         "conda-forge",
         "noarch",
         "flake8-6.0.0-pyhd8ed1ab_0.conda",
     )
+    assert data is not None
     assert data["name"] == "flake8"
     assert data["version"] == "6.0.0"
 
 
 def test_get_libcfgraph_artifact_data_none():
     data = get_libcfgraph_artifact_data(
         "conda-forge",
@@ -30,23 +31,27 @@
         "flake8-6.0.0-pyhd8ed1ab_0.conda",
     )
     assert data is None
 
 
 def test_get_libcfgraph_pkgs_for_import():
     pkgs, nm = get_libcfgraph_pkgs_for_import("numpy")
+    assert pkgs is not None
     assert nm == "numpy"
     assert "numpy" in pkgs
 
     pkgs, nm = get_libcfgraph_pkgs_for_import("numpy.linalg")
+    assert pkgs is not None
     assert nm == "numpy"
     assert "numpy" in pkgs
 
     # something bespoke
     pkgs, nm = get_libcfgraph_pkgs_for_import("eastlake")
+    assert pkgs is not None
     assert nm == "eastlake"
     assert "des-eastlake" in pkgs
     assert len(pkgs) == 1
 
     pkgs, nm = get_libcfgraph_pkgs_for_import("scipy")
+    assert pkgs is not None
     assert nm == "scipy"
     assert "scipy" in pkgs
```

