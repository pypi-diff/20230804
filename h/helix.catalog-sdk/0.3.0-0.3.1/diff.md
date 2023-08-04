# Comparing `tmp/helix.catalog-sdk-0.3.0.tar.gz` & `tmp/helix.catalog-sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helix.catalog-sdk-0.3.0.tar", last modified: Mon May 15 23:59:27 2023, max compression
+gzip compressed data, was "dist/helix.catalog-sdk-0.3.1.tar", last modified: Fri Aug  4 15:38:23 2023, max compression
```

## Comparing `helix.catalog-sdk-0.3.0.tar` & `helix.catalog-sdk-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 23:59:26.000000 helix.catalog-sdk-0.3.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-15 23:59:26.000000 helix.catalog-sdk-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 15:38:21.000000 helix.catalog-sdk-0.3.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-04 15:38:22.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:38:22.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:38:22.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/helix_catalog_sdk/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-04 15:38:21.000000 helix.catalog-sdk-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:23.000000 helix.catalog-sdk-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-08-04 15:37:10.000000 helix.catalog-sdk-0.3.1/tests/test_catalog.py
```

### Comparing `helix.catalog-sdk-0.3.0/LICENSE` & `helix.catalog-sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/Makefile` & `helix.catalog-sdk-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/PKG-INFO` & `helix.catalog-sdk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/PKG-INFO` & `helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/SOURCES.txt` & `helix.catalog-sdk-0.3.1/helix.catalog_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/helix_catalog_sdk/catalog.py` & `helix.catalog-sdk-0.3.1/helix_catalog_sdk/catalog.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/helix_catalog_sdk/data_source.py` & `helix.catalog-sdk-0.3.1/helix_catalog_sdk/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             if resource.matches_path(path):
                 return resource
         return None
 
     def update_path_with_latest_file(self, file_path: str) -> None:
         resource = self.get_matching_resource(file_path)
         if resource is not None and resource.path_slug is not None:
-            index: int = file_path.find(resource.path_slug)
+            index: int = file_path.rfind(resource.path_slug)
             resource.path = file_path[index:]
 
 
 class PipelineSubscription:
     def __init__(self, content: SimpleNamespace):
         if isinstance(content, str):
             self.flow_name: str = content
```

### Comparing `helix.catalog-sdk-0.3.0/helix_catalog_sdk/repo.py` & `helix.catalog-sdk-0.3.1/helix_catalog_sdk/repo.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/setup.py` & `helix.catalog-sdk-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.3.0/tests/test_catalog.py` & `helix.catalog-sdk-0.3.1/tests/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,33 @@
     claims_resource = data_source.resources[0]
     assert (
         claims_resource.full_path
         == "s3://bwell-ingestion/preprocessed/burris_highmark_claims_medical/20210915_2645841001FLX.txt"
     )
 
 
+def test_catalog_update_data_source_resource_with_same_directory_name() -> None:
+    clean_test_folder()
+    repo = DirectoryRepo(location="")
+    catalog = Catalog(repo=repo)
+    catalog.get_all_data_sources()
+
+    updated_data_source = catalog.update_data_source_resource(
+        "s3://bwell-ingestion/preprocessed/altrua_manifestrx_claims_rx/manifestrx_654321.csv"
+    )
+
+    assert updated_data_source is not None
+    claims_resource = updated_data_source.resources[0]
+    assert (
+        claims_resource.full_path
+        == "s3://bwell-ingestion/preprocessed/altrua_manifestrx_claims_rx/manifestrx_654321.csv"
+    )
+    assert claims_resource.path == "manifestrx_654321.csv"
+
+
 def test_catalog_update_data_source_resource_returns_none() -> None:
     clean_test_folder()
     repo = DirectoryRepo(location="")
     catalog = Catalog(repo=repo)
     catalog.get_all_data_sources()
 
     updated_data_source = catalog.update_data_source_resource(
```

