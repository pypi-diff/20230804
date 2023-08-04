# Comparing `tmp/types-aiobotocore-customer-profiles-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-customer-profiles-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
```

## Comparing `types-aiobotocore-customer-profiles-2.5.2.post2.tar` & `types-aiobotocore-customer-profiles-2.5.2.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.207754 types-aiobotocore-customer-profiles-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:00:42.203754 types-aiobotocore-customer-profiles-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.207754 types-aiobotocore-customer-profiles-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.195753 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41017 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40958 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62983 2023-08-04 11:43:21.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62895 2023-08-04 11:43:19.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.099585 types-aiobotocore-customer-profiles-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:37:34.091585 types-aiobotocore-customer-profiles-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.099585 types-aiobotocore-customer-profiles-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.087585 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41017 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40958 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62983 2023-08-04 12:21:07.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62895 2023-08-04 12:21:05.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.091585 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/LICENSE` & `types-aiobotocore-customer-profiles-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.2.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/README.md` & `types-aiobotocore-customer-profiles-2.5.2.post3/README.md`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/setup.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-customer-profiles",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with"
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__main__.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CustomerProfiles 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.py` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.2.post2
+Version: 2.5.2.post3
 Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt` & `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

