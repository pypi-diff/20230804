# Comparing `tmp/squirrel_core-0.19.2.dev863.tar.gz` & `tmp/squirrel_core-0.19.3.dev1207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.19.2.dev863.tar", max compression
+gzip compressed data, was "squirrel_core-0.19.3.dev1207.tar", max compression
```

## Comparing `squirrel_core-0.19.2.dev863.tar` & `squirrel_core-0.19.3.dev1207.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0    11348 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/LICENSE
--rw-r--r--   0        0        0     5424 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/README.md
--rw-r--r--   0        0        0     3006 2023-07-21 14:06:11.503828 squirrel_core-0.19.2.dev863/pyproject.toml
--rw-r--r--   0        0        0       80 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/__init__.py
--rw-r--r--   0        0        0     3253 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    14080 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/constants.py
--rw-r--r--   0        0        0      887 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4511 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2127 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/file.py
--rw-r--r--   0        0        0     2192 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1099 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4586 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2211 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3837 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    23773 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0     5999 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5202 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/py.typed
--rw-r--r--   0        0        0      263 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     4864 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 squirrel_core-0.19.2.dev863/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-08-04 12:51:28.035509 squirrel_core-0.19.3.dev1207/LICENSE
+-rw-r--r--   0        0        0     5424 2023-08-04 12:51:28.035509 squirrel_core-0.19.3.dev1207/README.md
+-rw-r--r--   0        0        0     3007 2023-08-04 12:55:42.941558 squirrel_core-0.19.3.dev1207/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/__init__.py
+-rw-r--r--   0        0        0     1526 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/benchmark/msgpack_caching.py
+-rw-r--r--   0        0        0     3253 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    15250 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4716 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2330 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2396 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1303 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4030 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2510 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3837 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      471 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    23773 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0     5999 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5202 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2023-08-04 12:51:28.047510 squirrel_core-0.19.3.dev1207/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     3117 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2023-08-04 12:51:28.051510 squirrel_core-0.19.3.dev1207/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8040 1970-01-01 00:00:00.000000 squirrel_core-0.19.3.dev1207/PKG-INFO
```

### Comparing `squirrel_core-0.19.2.dev863/LICENSE` & `squirrel_core-0.19.3.dev1207/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/README.md` & `squirrel_core-0.19.3.dev1207/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/pyproject.toml` & `squirrel_core-0.19.3.dev1207/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.19.2-dev863"
+version = "0.19.3-dev1207"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.19.3.dev1207/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py` & `squirrel_core-0.19.3.dev1207/squirrel/catalog/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from __future__ import annotations
 
 import io
 import json
-from typing import Any, Callable, Iterable, Iterator, KeysView, MutableMapping, NamedTuple, TYPE_CHECKING
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Iterator,
+    KeysView,
+    MutableMapping,
+    NamedTuple,
+)
 
 import fsspec
-
 from squirrel.catalog.source import Source
 from squirrel.fsspec.fs import get_fs_from_url
 
 if TYPE_CHECKING:
     from ruamel.yaml import Constructor, Representer, SequenceNode
-
     from squirrel.driver import Driver
 
 __all__ = ["Catalog", "CatalogKey", "CatalogSource"]
 
 
 class CatalogKey(NamedTuple):
     """Defines a key in a catalog consisting of the identifier and the version of a source.
@@ -128,15 +135,19 @@
 
     def __len__(self) -> int:  # noqa D105
         return len(self.keys())
 
     def copy(self) -> Catalog:
         """Return a deep copy of catalog"""
         # To be 100% save, serialize to string and back
-        from squirrel.catalog.yaml import catalog2yamlcatalog, prep_yaml, yamlcatalog2catalog
+        from squirrel.catalog.yaml import (
+            catalog2yamlcatalog,
+            prep_yaml,
+            yamlcatalog2catalog,
+        )
 
         yaml = prep_yaml()
         ret = None
 
         with io.StringIO() as fh:
             yaml.dump(catalog2yamlcatalog(self), fh)
             fh.seek(0)
@@ -353,14 +364,27 @@
         """Returns an instance of the driver specified by the source."""
         from squirrel.framework.plugins.plugin_manager import squirrel_plugin_manager
 
         plugins: list[list[type[Driver]]] = squirrel_plugin_manager.hook.squirrel_drivers()
         for plugin in plugins:
             for driver_cls in plugin:
                 if driver_cls.name == self.driver_name:
+                    # Problem: If users provide "storage_options" in the `kwargs` and the `self.driver_kwargs`
+                    # already defines "storage_options", then vanilla dict merging
+                    # (i.e., {**self.driver_kwargs, **kwargs}) will overwrite the "storage_options" in
+                    # `self.driver_kwargs` entirely. This is undesired, since important information like
+                    # bucket configurations (e.g., "requester_pays") may be stored in the `self.driver_kwargs`
+                    # "storage_options", which users don't want to provide again using `kwargs`.
+                    # Solution: The below mechanism merges the "storage_options" in `kwargs` with the existing
+                    # "storage_options" in `self.driver_kwargs` (while the newly passed "storage_options"
+                    # in `kwargs` take precendence).
+                    kwargs["storage_options"] = {
+                        **self.driver_kwargs.get("storage_options", {}),
+                        **kwargs.get("storage_options", {}),
+                    }
                     return driver_cls(catalog=self._catalog, **{**self.driver_kwargs, **kwargs})
 
         raise ValueError(f"driver {self.driver_name} not found")
 
 
 class DummyCatalogSource:
     def __init__(
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/catalog/source.py` & `squirrel_core-0.19.3.dev1207/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py` & `squirrel_core-0.19.3.dev1207/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/constants.py` & `squirrel_core-0.19.3.dev1207/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/csv.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/data_frame.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 
         This defines a common interface for all driver using different read methods to read a dataframe such as
         from .csv, .xls, .parqet etc. These derived drivers have to only specify the read() method.
 
         Args:
             url (URL): URL to file. Prefix with a protocol like ``s3://`` or ``gs://`` to read from other filesystems.
                        Data type may depend on the derived class.
-            storage_options (Optional[Dict[str, Any]]): a dict with keyword arguments passed to file system initializer
+            storage_options (Optional[Dict[str, Any]]): a dict with keyword arguments passed to file system initializer.
+                Example of storage_options if you want to enable `fsspec` caching:
+                `storage_options={"protocol": "simplecache", "target_protocol": "gs", "cache_storage": "path/to/cache"}`
             engine (ENGINE): Which engine to use for DataFrame loading. Currently, all drivers support "pandas" to use
                              Pandas and some support "dask" to asynchronously load DataFrames using Dask.
             df_hooks (Iterable[Callable], optional): Preprocessing hooks to execute on the dataframe.
                                                      The first hook must accept a dask.dataframe.DataFrame or
                                                      pandas.Dataframe depending on the used engine.
             read_kwargs: Arguments passed to all read methods of the derived driver.
             **kwargs: Keyword arguments passed to the Driver class initializer.
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/driver.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/excel.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/feather.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/file.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 from typing import IO, Any
 
 import fsspec
-
 from squirrel.constants import URL
 from squirrel.driver.driver import Driver
 
 
 class FileDriver(Driver):
     name = "file"
 
     def __init__(self, url: URL, storage_options: dict[str, Any] | None = None, **kwargs) -> None:
         """Initializes FileDriver.
 
         Args:
             url (URL): URL to file. Prefix with a protocol like ``s3://`` or ``gs://`` to read from other filesystems.
                        For a full list of supported types, refer to :func:`fsspec.open()`.
             storage_options (dict[str, Any] | None): A dict with keyword arguments passed to file system initializer.
+                Example of storage_options if you want to enable `fsspec` caching:
+                `storage_options={"protocol": "simplecache", "target_protocol": "gs", "cache_storage": "path/to/cache"}`
             **kwargs: Keyword arguments passed to the super class initializer.
         """
         super().__init__(**kwargs)
         self.url = url
         self.storage_options = storage_options or {}
 
     def open(self, mode: str = "r", create_if_not_exists: bool = False, **kwargs) -> IO:
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/jsonl.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         """Initializes JsonlDriver with default serializer.
 
         Args:
             url (str): Path to the root directory. If this path does not exist, it will be created.
             deser_hook (Callable): Callable that is passed as `object_hook` to :py:class:`JsonDecoder` during json
                 deserialization. Defaults to None.
             storage_options (Dict): a dictionary containing storage_options to be passed to fsspec.
+                Example of storage_options if you want to enable `fsspec` caching:
+                `storage_options={"protocol": "simplecache", "target_protocol": "gs", "cache_storage": "path/to/cache"}`
             **kwargs: Keyword arguments passed to the super class initializer.
         """
         if "store" in kwargs:
             raise ValueError("Store of JsonlDriver is fixed, `store` cannot be provided.")
         super().__init__(
             url=url, serializer=JsonSerializer(deser_hook=deser_hook), storage_options=storage_options, **kwargs
         )
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/msgpack.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,12 +17,14 @@
 
     def __init__(self, url: str, storage_options: dict[str, Any] | None = None, **kwargs):
         """Initializes MessagepackDriver with default serializer. See parent class for more options.
 
         Args:
             url (str): Path to the root directory. If this path does not exist, it will be created.
             storage_options (Dict): a dictionary containing storage_options to be passed to fsspec.
+                Example of storage_options if you want to enable `fsspec` caching:
+                `storage_options={"protocol": "simplecache", "target_protocol": "gs", "cache_storage": "path/to/cache"}`
             **kwargs: Keyword arguments passed to the super class initializer.
         """
         if "store" in kwargs:
             raise ValueError("Store of MessagepackDriver is fixed, `store` cannot be provided.")
         super().__init__(url=url, serializer=MessagepackSerializer(), storage_options=storage_options, **kwargs)
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/store.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/store.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
-from typing import Any, Iterable, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Iterable
 
 from squirrel.driver.driver import MapDriver
 from squirrel.serialization import SquirrelSerializer
 from squirrel.store import SquirrelStore
-from squirrel.store.squirrel_store import CacheStore
 
 if TYPE_CHECKING:
     from squirrel.iterstream import Composable
     from squirrel.store.store import AbstractStore
 
 
 class StoreDriver(MapDriver):
@@ -20,36 +19,31 @@
 
     name = "store_driver"
 
     def __init__(
         self,
         url: str,
         serializer: SquirrelSerializer,
-        cache_url: str | None = None,
         storage_options: dict[str, Any] | None = None,
-        cash_storage_options: dict[str, Any] | None = None,
         **kwargs,
     ) -> None:
         """Initializes StoreDriver.
 
         Args:
             url (str): the url of the store
             serializer (SquirrelSerializer): serializer to be passed to SquirrelStore
-            cache_url (str): if provided, the data will be cached in a store at this url
             storage_options (Optional[Dict[str, Any]]): a dict with keyword arguments to be passed to store initializer
-            cash_storage_options (Optional[Dict[str, Any]]): a dict with keyword arguments to be passed to
-                cache store initializer
+                Example of storage_options if you want to enable `fsspec` caching:
+                `storage_options={"protocol": "simplecache", "target_protocol": "gs", "cache_storage": "path/to/cache"}`
             **kwargs: Keyword arguments to pass to the super class initializer.
         """
         super().__init__(**kwargs)
         self.url = url
         self.serializer = serializer
         self.storage_options = storage_options if storage_options is not None else {}
-        self.cash_storage_options = cash_storage_options if cash_storage_options is not None else {}
-        self.cache_url = cache_url
         self._store = None
 
     def get_iter(self, flatten: bool = True, **kwargs) -> Composable:
         """Returns an iterable of items in the form of a :py:class:`squirrel.iterstream.Composable`, which allows
         various stream manipulation functionalities.
 
         Items are fetched using the :py:meth:`get` method. The returned :py:class:`Composable` iterates over the items
@@ -95,14 +89,9 @@
         """
         return self.store.keys(**kwargs)
 
     @property
     def store(self) -> AbstractStore:
         """Store that is used by the driver."""
         if self._store is None:
-            if self.cache_url is None:
-                self._store = SquirrelStore(url=self.url, serializer=self.serializer, **self.storage_options)
-            else:
-                self._store = CacheStore(
-                    url=self.url, serializer=self.serializer, cache_url=self.cache_url, **self.cash_storage_options
-                )
+            self._store = SquirrelStore(url=self.url, serializer=self.serializer, **self.storage_options)
         return self._store
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py` & `squirrel_core-0.19.3.dev1207/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/framework/io.py` & `squirrel_core-0.19.3.dev1207/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.19.3.dev1207/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.19.3.dev1207/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py` & `squirrel_core-0.19.3.dev1207/squirrel/fsspec/fs.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,22 @@
     for the project that contains the bucket. The Billing Project Manager role contains the required permission.
     Access charges associated with these requests are billed to the project that contains the bucket.
 
     If you have encountered `ValueError: Bucket is requester pays. Set `requester_pays=True` when creating the
     GCSFileSystem.` I suggest you instead of passing `requester_pays=True` to `storage_options` in fsspec, simply
     switch to the right project by `gcloud config set project PROJECT_ID` where you have the right role(s). The problem
     should be resolved by itself.
+
+    The protocol can be overriden via the `storage_options`. This is important if people want to use the fsspec caching
+    functionality, which requires the protocol to be, e.g., `simplecache`.
     """
+
     protocol, _ = split_protocol(url)
-    return fsspec.filesystem(protocol, **storage_options)
+
+    # Provided storage_options take precedence
+    storage_options = {"protocol": protocol, **storage_options}
+    return fsspec.filesystem(**storage_options)
 
 
 def get_protocol(url: str) -> str:
     """Get the protocol from a url, return empty string if local"""
     return f"{url.split('://')[0]}://" if "://" in url else ""
```

### Comparing `squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py` & `squirrel_core-0.19.3.dev1207/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.19.3.dev1207/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.19.3.dev1207/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py` & `squirrel_core-0.19.3.dev1207/squirrel/iterstream/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py` & `squirrel_core-0.19.3.dev1207/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py` & `squirrel_core-0.19.3.dev1207/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py` & `squirrel_core-0.19.3.dev1207/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.19.3.dev1207/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py` & `squirrel_core-0.19.3.dev1207/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py` & `squirrel_core-0.19.3.dev1207/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py` & `squirrel_core-0.19.3.dev1207/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py` & `squirrel_core-0.19.3.dev1207/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/store/store.py` & `squirrel_core-0.19.3.dev1207/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/zarr/group.py` & `squirrel_core-0.19.3.dev1207/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/zarr/key.py` & `squirrel_core-0.19.3.dev1207/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/zarr/store.py` & `squirrel_core-0.19.3.dev1207/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py` & `squirrel_core-0.19.3.dev1207/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2.dev863/PKG-INFO` & `squirrel_core-0.19.3.dev1207/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.19.2.dev863
+Version: 0.19.3.dev1207
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

