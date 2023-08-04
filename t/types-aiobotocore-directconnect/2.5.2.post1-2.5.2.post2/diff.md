# Comparing `tmp/types-aiobotocore-directconnect-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-directconnect-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-directconnect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-directconnect-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-directconnect-2.5.2.post1.tar` & `types-aiobotocore-directconnect-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49705 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49630 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54831 2023-08-02 14:36:25.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-08-02 14:36:25.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.939859 types-aiobotocore-directconnect-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-08-04 12:00:44.939859 types-aiobotocore-directconnect-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.939859 types-aiobotocore-directconnect-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.939859 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49705 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49630 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54831 2023-08-04 11:43:46.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-08-04 11:43:46.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:45.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.939859 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:44.000000 types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/LICENSE` & `types-aiobotocore-directconnect-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/setup.py` & `types-aiobotocore-directconnect-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-directconnect",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.pyi` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__main__.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.DirectConnect 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
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

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.pyi` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.pyi` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.pyi` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.py` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.pyi` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/SOURCES.txt` & `types-aiobotocore-directconnect-2.5.2.post2/types_aiobotocore_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

