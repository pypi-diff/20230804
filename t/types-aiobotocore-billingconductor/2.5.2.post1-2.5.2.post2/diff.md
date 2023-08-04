# Comparing `tmp/types-aiobotocore-billingconductor-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-billingconductor-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-billingconductor-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-billingconductor-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:30 2023, max compression
```

## Comparing `types-aiobotocore-billingconductor-2.5.2.post1.tar` & `types-aiobotocore-billingconductor-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.485643 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-08-02 14:33:51.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42685 2023-08-02 14:33:51.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.491308 types-aiobotocore-billingconductor-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-04 12:00:30.491308 types-aiobotocore-billingconductor-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:30.491308 types-aiobotocore-billingconductor-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.491308 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-04 11:41:03.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-08-04 11:41:03.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42685 2023-08-04 11:41:03.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:02.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.491308 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:30.000000 types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/LICENSE` & `types-aiobotocore-billingconductor-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/setup.py` & `types-aiobotocore-billingconductor-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-billingconductor",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.pyi` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__main__.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.BillingConductor 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
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

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.pyi` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.pyi` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.pyi` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.py` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.pyi` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt` & `types-aiobotocore-billingconductor-2.5.2.post2/types_aiobotocore_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

