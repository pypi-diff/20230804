# Comparing `tmp/types-aiobotocore-cur-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-cur-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cur-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-cur-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:33 2023, max compression
```

## Comparing `types-aiobotocore-cur-2.5.2.post2.tar` & `types-aiobotocore-cur-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 11:43:16.000000 types-aiobotocore-cur-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.195753 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.939581 types-aiobotocore-cur-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:33.939581 types-aiobotocore-cur-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cur-2.5.2.post2/LICENSE` & `types-aiobotocore-cur-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/PKG-INFO` & `types-aiobotocore-cur-2.5.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-cur-2.5.2.post2/README.md` & `types-aiobotocore-cur-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/setup.py` & `types-aiobotocore-cur-2.5.2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cur",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.pyi` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__main__.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CostandUsageReportService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.pyi` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.pyi` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.pyi` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.py` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.pyi` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/PKG-INFO` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/SOURCES.txt` & `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

