# Comparing `tmp/types-aiobotocore-compute-optimizer-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-compute-optimizer-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2.tar` & `types-aiobotocore-compute-optimizer-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.039709 types-aiobotocore-compute-optimizer-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.039709 types-aiobotocore-compute-optimizer-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-08-04 11:42:51.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42051 2023-08-04 11:42:53.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-08-04 11:42:52.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.523522 types-aiobotocore-compute-optimizer-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:37:31.519521 types-aiobotocore-compute-optimizer-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.523522 types-aiobotocore-compute-optimizer-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.515521 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42051 2023-08-04 12:20:41.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-08-04 12:20:41.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:39.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.519521 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:31.000000 types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/LICENSE` & `types-aiobotocore-compute-optimizer-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/README.md` & `types-aiobotocore-compute-optimizer-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/setup.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-compute-optimizer",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__main__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ComputeOptimizer 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.2.post3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.py` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt` & `types-aiobotocore-compute-optimizer-2.5.2.post3/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

