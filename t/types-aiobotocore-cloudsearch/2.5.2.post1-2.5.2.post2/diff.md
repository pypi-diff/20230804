# Comparing `tmp/types-aiobotocore-cloudsearch-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudsearch-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearch-2.5.2.post1.tar` & `types-aiobotocore-cloudsearch-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.189636 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-02 14:34:43.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-08-02 14:34:42.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:41.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.209636 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:00.000000 types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.955438 types-aiobotocore-cloudsearch-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-04 12:00:33.955438 types-aiobotocore-cloudsearch-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.955438 types-aiobotocore-cloudsearch-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.951438 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-04 11:41:57.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-04 11:41:57.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-04 11:41:57.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-08-04 11:41:57.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:56.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.955438 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:00:33.000000 types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudsearch-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/setup.py` & `types-aiobotocore-cloudsearch-2.5.2.post2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearch",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/__main__.py` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.py` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/client.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.py` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/literals.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.py` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch/type_defs.pyi` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post1/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearch-2.5.2.post2/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

