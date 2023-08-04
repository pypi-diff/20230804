# Comparing `tmp/types-aiobotocore-config-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-config-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-config-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-config-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-config-2.5.2.post2.tar` & `types-aiobotocore-config-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.655732 types-aiobotocore-config-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18131 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.655732 types-aiobotocore-config-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:42:53.000000 types-aiobotocore-config-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92692 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92560 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44399 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   128018 2023-08-04 11:42:58.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   127867 2023-08-04 11:42:57.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.623524 types-aiobotocore-config-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:37:31.619524 types-aiobotocore-config-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18131 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.623524 types-aiobotocore-config-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.611524 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92692 2023-08-04 12:20:43.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92560 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-08-04 12:20:43.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-08-04 12:20:43.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44399 2023-08-04 12:20:43.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-08-04 12:20:43.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   128018 2023-08-04 12:20:46.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127867 2023-08-04 12:20:45.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:42.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.619524 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:31.000000 types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-config-2.5.2.post2/LICENSE` & `types-aiobotocore-config-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/PKG-INFO` & `types-aiobotocore-config-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-config-2.5.2.post2/README.md` & `types-aiobotocore-config-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/setup.py` & `types-aiobotocore-config-2.5.2.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-config",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConfigService 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.pyi` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__main__.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConfigService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.pyi` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.pyi` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.pyi` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.py` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.pyi` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/PKG-INFO` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/SOURCES.txt` & `types-aiobotocore-config-2.5.2.post3/types_aiobotocore_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

