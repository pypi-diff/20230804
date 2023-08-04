# Comparing `tmp/types-aiobotocore-gamesparks-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-gamesparks-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamesparks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamesparks-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:56 2023, max compression
```

## Comparing `types-aiobotocore-gamesparks-2.5.2.post1.tar` & `types-aiobotocore-gamesparks-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.565581 types-aiobotocore-gamesparks-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.565581 types-aiobotocore-gamesparks-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29801 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.068277 types-aiobotocore-gamesparks-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-08-04 12:00:56.068277 types-aiobotocore-gamesparks-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:56.068277 types-aiobotocore-gamesparks-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.068277 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-08-04 11:46:46.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29801 2023-08-04 11:46:45.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:44.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.068277 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:55.000000 types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/LICENSE` & `types-aiobotocore-gamesparks-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/setup.py` & `types-aiobotocore-gamesparks-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamesparks",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GameSparks 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.pyi` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__main__.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameSparks 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.GameSparks 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.pyi` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.pyi` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.pyi` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.py` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.pyi` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/SOURCES.txt` & `types-aiobotocore-gamesparks-2.5.2.post2/types_aiobotocore_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

