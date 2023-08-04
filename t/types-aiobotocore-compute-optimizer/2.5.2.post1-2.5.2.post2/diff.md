# Comparing `tmp/types-aiobotocore-compute-optimizer-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-compute-optimizer-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
```

## Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1.tar` & `types-aiobotocore-compute-optimizer-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.853614 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42051 2023-08-02 14:35:34.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.039709 types-aiobotocore-compute-optimizer-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.039709 types-aiobotocore-compute-optimizer-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-08-04 11:42:51.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42051 2023-08-04 11:42:53.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-08-04 11:42:52.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:50.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.031708 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:40.000000 types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/LICENSE` & `types-aiobotocore-compute-optimizer-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/setup.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-compute-optimizer",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__main__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ComputeOptimizer 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
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
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.py` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt` & `types-aiobotocore-compute-optimizer-2.5.2.post2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

