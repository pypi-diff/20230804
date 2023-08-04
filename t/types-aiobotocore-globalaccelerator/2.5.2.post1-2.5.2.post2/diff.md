# Comparing `tmp/types-aiobotocore-globalaccelerator-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-globalaccelerator-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-globalaccelerator-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-globalaccelerator-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1.tar` & `types-aiobotocore-globalaccelerator-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.317577 types-aiobotocore-globalaccelerator-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-08-02 14:52:21.317577 types-aiobotocore-globalaccelerator-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.317577 types-aiobotocore-globalaccelerator-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.313577 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43795 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43729 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44656 2023-08-02 14:39:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44607 2023-08-02 14:39:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:18.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.317577 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.076350 types-aiobotocore-globalaccelerator-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-04 12:00:58.076350 types-aiobotocore-globalaccelerator-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.076350 types-aiobotocore-globalaccelerator-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.076350 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43795 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43729 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-04 11:46:51.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44656 2023-08-04 11:46:51.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44607 2023-08-04 11:46:51.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:50.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.076350 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:57.000000 types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/LICENSE` & `types-aiobotocore-globalaccelerator-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/setup.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-globalaccelerator",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GlobalAccelerator 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__init__.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__init__.pyi` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/__main__.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.GlobalAccelerator 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/client.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/client.pyi` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/literals.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/literals.pyi` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/paginator.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/paginator.pyi` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/type_defs.py` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator/type_defs.pyi` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post1/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt` & `types-aiobotocore-globalaccelerator-2.5.2.post2/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

