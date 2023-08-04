# Comparing `tmp/types-aiobotocore-connectcases-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-connectcases-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-connectcases-2.5.2.post2.tar` & `types-aiobotocore-connectcases-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-08-04 11:43:14.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcases-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:37:31.695526 types-aiobotocore-connectcases-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.699526 types-aiobotocore-connectcases-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.691526 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.695526 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/LICENSE` & `types-aiobotocore-connectcases-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/README.md` & `types-aiobotocore-connectcases-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/setup.py` & `types-aiobotocore-connectcases-2.5.2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcases",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.pyi` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__main__.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post3\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.pyi` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.pyi` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.pyi` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.py` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.pyi` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/SOURCES.txt` & `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

