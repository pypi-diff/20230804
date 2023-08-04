# Comparing `tmp/types-aiobotocore-fis-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-fis-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fis-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-fis-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-fis-2.5.2.post1.tar` & `types-aiobotocore-fis-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.021583 types-aiobotocore-fis-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-08-02 14:52:19.017583 types-aiobotocore-fis-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.021583 types-aiobotocore-fis-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.017583 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-08-02 14:38:49.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:48.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.017583 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:18.000000 types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.444254 types-aiobotocore-fis-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:00:55.444254 types-aiobotocore-fis-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.444254 types-aiobotocore-fis-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.444254 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-08-04 11:46:19.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:18.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.444254 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:55.000000 types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fis-2.5.2.post1/LICENSE` & `types-aiobotocore-fis-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/setup.py` & `types-aiobotocore-fis-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fis",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/__main__.py` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FIS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.FIS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS\nOther"
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

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/client.py` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/client.pyi` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/literals.py` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/literals.pyi` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/type_defs.py` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis/type_defs.pyi` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post1/types_aiobotocore_fis.egg-info/SOURCES.txt` & `types-aiobotocore-fis-2.5.2.post2/types_aiobotocore_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

