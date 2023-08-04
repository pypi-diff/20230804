# Comparing `tmp/types-aiobotocore-docdb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-docdb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-docdb-2.5.2.post1.tar` & `types-aiobotocore-docdb-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.029601 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53689 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53612 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.395952 types-aiobotocore-docdb-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-08-04 12:00:47.395952 types-aiobotocore-docdb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.395952 types-aiobotocore-docdb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.395952 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53689 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53612 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:58.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-04 11:43:59.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.395952 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-2.5.2.post1/LICENSE` & `types-aiobotocore-docdb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/setup.py` & `types-aiobotocore-docdb-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__main__.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DocDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
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

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.py` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.pyi` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-2.5.2.post2/types_aiobotocore_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

