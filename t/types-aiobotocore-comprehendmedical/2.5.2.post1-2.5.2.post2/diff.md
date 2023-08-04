# Comparing `tmp/types-aiobotocore-comprehendmedical-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-comprehendmedical-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1.tar` & `types-aiobotocore-comprehendmedical-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-02 14:35:32.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.009618 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:04.000000 types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.447647 types-aiobotocore-comprehendmedical-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-08-04 12:00:39.439647 types-aiobotocore-comprehendmedical-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.447647 types-aiobotocore-comprehendmedical-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.435647 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-08-04 11:42:49.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-08-04 11:42:49.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-04 11:42:49.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-04 11:42:49.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-08-04 11:42:49.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:48.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.439647 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:39.000000 types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/LICENSE` & `types-aiobotocore-comprehendmedical-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/setup.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehendmedical",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__init__.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/__main__.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ComprehendMedical 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/client.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/literals.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.py` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical/type_defs.pyi` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt` & `types-aiobotocore-comprehendmedical-2.5.2.post2/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

