# Comparing `tmp/types-aiobotocore-connectparticipant-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-connectparticipant-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectparticipant-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectparticipant-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:32 2023, max compression
```

## Comparing `types-aiobotocore-connectparticipant-2.5.2.post2.tar` & `types-aiobotocore-connectparticipant-2.5.2.post3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.011746 types-aiobotocore-connectparticipant-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:00:42.011746 types-aiobotocore-connectparticipant-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.011746 types-aiobotocore-connectparticipant-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.011746 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:14.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.011746 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 12:00:41.000000 types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:32.235539 types-aiobotocore-connectparticipant-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:37:32.227539 types-aiobotocore-connectparticipant-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:32.235539 types-aiobotocore-connectparticipant-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 12:21:00.000000 types-aiobotocore-connectparticipant-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:32.227539 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:01.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:32.227539 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 12:37:32.000000 types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/LICENSE` & `types-aiobotocore-connectparticipant-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/PKG-INFO` & `types-aiobotocore-connectparticipant-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectparticipant
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/README.md` & `types-aiobotocore-connectparticipant-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/setup.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectparticipant",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_connectparticipant"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__init__.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__init__.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/__main__.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectParticipant 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant\nOther"
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

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/client.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/client.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/literals.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/literals.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/type_defs.py` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant/type_defs.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/PKG-INFO` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectparticipant
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2.post2/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt` & `types-aiobotocore-connectparticipant-2.5.2.post3/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

