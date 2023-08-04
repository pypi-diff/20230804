# Comparing `tmp/types-aiobotocore-connectcampaigns-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-connectcampaigns-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
```

## Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2.tar` & `types-aiobotocore-connectcampaigns-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:43:11.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/LICENSE` & `types-aiobotocore-connectcampaigns-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/README.md` & `types-aiobotocore-connectcampaigns-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/setup.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcampaigns",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__main__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.py` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt` & `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

