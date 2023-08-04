# Comparing `tmp/types-aiobotocore-drs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-drs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-drs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-drs-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-drs-2.5.2.post1.tar` & `types-aiobotocore-drs-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.025601 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56844 2023-08-02 14:36:42.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-08-02 14:36:42.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.025601 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.423953 types-aiobotocore-drs-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-04 12:00:47.423953 types-aiobotocore-drs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.423953 types-aiobotocore-drs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.411952 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-08-04 11:44:04.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56844 2023-08-04 11:44:05.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-08-04 11:44:04.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:03.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.423953 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:47.000000 types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-drs-2.5.2.post1/LICENSE` & `types-aiobotocore-drs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/setup.py` & `types-aiobotocore-drs-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-drs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.pyi` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__main__.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.pyi` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.pyi` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.pyi` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.py` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.pyi` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/SOURCES.txt` & `types-aiobotocore-drs-2.5.2.post2/types_aiobotocore_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

