# Comparing `tmp/types-aiobotocore-healthlake-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-healthlake-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-healthlake-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-healthlake-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:48 2023, max compression
```

## Comparing `types-aiobotocore-healthlake-2.5.2.post1.tar` & `types-aiobotocore-healthlake-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.117575 types-aiobotocore-healthlake-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:22.117575 types-aiobotocore-healthlake-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.587925 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/LICENSE` & `types-aiobotocore-healthlake-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/setup.py` & `types-aiobotocore-healthlake-2.5.2.post2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-healthlake",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.HealthLake 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__main__.py` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthLake 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.HealthLake 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.py` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.pyi` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.py` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.pyi` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.py` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.pyi` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/SOURCES.txt` & `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

