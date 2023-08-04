# Comparing `tmp/types-aiobotocore-alexaforbusiness-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-alexaforbusiness-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1.tar` & `types-aiobotocore-alexaforbusiness-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.829667 types-aiobotocore-alexaforbusiness-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24605 2023-08-02 14:51:47.829667 types-aiobotocore-alexaforbusiness-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23051 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.829667 types-aiobotocore-alexaforbusiness-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.829667 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-08-02 14:32:46.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71421 2023-08-02 14:32:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71346 2023-08-02 14:32:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:45.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.829667 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24605 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:51:47.000000 types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.734887 types-aiobotocore-alexaforbusiness-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-08-04 12:00:19.730886 types-aiobotocore-alexaforbusiness-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.734887 types-aiobotocore-alexaforbusiness-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:39:49.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.726886 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-08-04 11:39:51.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71421 2023-08-04 11:39:53.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71346 2023-08-04 11:39:51.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:50.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.730886 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:19.000000 types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/LICENSE` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/setup.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-alexaforbusiness",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AlexaForBusiness 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__init__.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__init__.pyi` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/__main__.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AlexaForBusiness 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
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

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/client.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/client.pyi` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/literals.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/literals.pyi` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/paginator.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/paginator.pyi` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/type_defs.py` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness/type_defs.pyi` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post1/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt` & `types-aiobotocore-alexaforbusiness-2.5.2.post2/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

