# Comparing `tmp/types-aiobotocore-comprehend-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-comprehend-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-comprehend-2.5.2.post2.tar` & `types-aiobotocore-comprehend-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.447647 types-aiobotocore-comprehend-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:00:39.439647 types-aiobotocore-comprehend-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.447647 types-aiobotocore-comprehend-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.435647 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70286 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70183 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-04 11:42:45.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-04 11:42:45.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98449 2023-08-04 11:42:48.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98372 2023-08-04 11:42:46.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.439647 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.335517 types-aiobotocore-comprehend-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:37:31.331517 types-aiobotocore-comprehend-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.335517 types-aiobotocore-comprehend-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.319517 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70286 2023-08-04 12:20:34.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70183 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-04 12:20:34.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-04 12:20:34.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-04 12:20:34.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-04 12:20:34.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98449 2023-08-04 12:20:37.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98372 2023-08-04 12:20:35.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:33.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.331517 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:31.000000 types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/LICENSE` & `types-aiobotocore-comprehend-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/PKG-INFO` & `types-aiobotocore-comprehend-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehend
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/README.md` & `types-aiobotocore-comprehend-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/setup.py` & `types-aiobotocore-comprehend-2.5.2.post3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehend",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Comprehend 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.pyi` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__main__.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2.post3\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.pyi` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.pyi` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.pyi` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.py` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.pyi` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/PKG-INFO` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehend
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.Comprehend 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/SOURCES.txt` & `types-aiobotocore-comprehend-2.5.2.post3/types_aiobotocore_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

