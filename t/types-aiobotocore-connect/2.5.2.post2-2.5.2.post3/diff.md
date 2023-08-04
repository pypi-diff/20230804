# Comparing `tmp/types-aiobotocore-connect-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-connect-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-connect-2.5.2.post2.tar` & `types-aiobotocore-connect-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.963744 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   156901 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   156653 2023-08-04 11:43:02.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-08-04 11:43:04.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-08-04 11:43:04.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   217314 2023-08-04 11:43:11.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   216983 2023-08-04 11:43:07.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.735527 types-aiobotocore-connect-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:37:31.731527 types-aiobotocore-connect-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.735527 types-aiobotocore-connect-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.727527 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156901 2023-08-04 12:20:50.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156653 2023-08-04 12:20:50.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   217314 2023-08-04 12:20:58.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216983 2023-08-04 12:20:54.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.731527 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-2.5.2.post2/LICENSE` & `types-aiobotocore-connect-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/PKG-INFO` & `types-aiobotocore-connect-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connect-2.5.2.post2/README.md` & `types-aiobotocore-connect-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/setup.py` & `types-aiobotocore-connect-2.5.2.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder"
```

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.pyi` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__main__.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2.post3\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.2.post3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.pyi` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.pyi` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.pyi` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.py` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.pyi` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/PKG-INFO` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/SOURCES.txt` & `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

