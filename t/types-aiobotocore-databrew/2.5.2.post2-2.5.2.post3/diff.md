# Comparing `tmp/types-aiobotocore-databrew-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-databrew-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-databrew-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-databrew-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
```

## Comparing `types-aiobotocore-databrew-2.5.2.post2.tar` & `types-aiobotocore-databrew-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-04 11:43:21.000000 types-aiobotocore-databrew-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36017 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54090 2023-08-04 11:43:23.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53992 2023-08-04 11:43:23.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.155587 types-aiobotocore-databrew-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:37:34.147586 types-aiobotocore-databrew-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.155587 types-aiobotocore-databrew-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.143586 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36017 2023-08-04 12:21:08.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-08-04 12:21:08.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-08-04 12:21:08.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-04 12:21:08.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-04 12:21:08.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54090 2023-08-04 12:21:09.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53992 2023-08-04 12:21:09.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:07.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.147586 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:37:33.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:37:34.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:33.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:33.000000 types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-databrew-2.5.2.post2/LICENSE` & `types-aiobotocore-databrew-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/PKG-INFO` & `types-aiobotocore-databrew-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-databrew
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.GlueDataBrew 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-databrew-2.5.2.post2/README.md` & `types-aiobotocore-databrew-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/setup.py` & `types-aiobotocore-databrew-2.5.2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-databrew",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GlueDataBrew 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.pyi` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__main__.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GlueDataBrew 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.GlueDataBrew 2.5.2\nVersion:         2.5.2.post3\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.pyi` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.pyi` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.pyi` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.py` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.pyi` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/PKG-INFO` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-databrew
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.GlueDataBrew 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/SOURCES.txt` & `types-aiobotocore-databrew-2.5.2.post3/types_aiobotocore_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

