# Comparing `tmp/types-aiobotocore-codeartifact-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codeartifact-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeartifact-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeartifact-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codeartifact-2.5.2.post1.tar` & `types-aiobotocore-codeartifact-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.409626 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-08-02 14:34:51.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-02 14:34:51.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46914 2023-08-02 14:34:53.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-02 14:34:52.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:50.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.417626 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:02.000000 types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.519535 types-aiobotocore-codeartifact-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-08-04 12:00:36.519535 types-aiobotocore-codeartifact-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.519535 types-aiobotocore-codeartifact-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.519535 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-04 11:42:07.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-04 11:42:07.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46914 2023-08-04 11:42:08.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-04 11:42:07.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:06.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.519535 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:36.000000 types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/LICENSE` & `types-aiobotocore-codeartifact-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/setup.py` & `types-aiobotocore-codeartifact-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeartifact",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__init__.pyi` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/__main__.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeArtifact 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeArtifact 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
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

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/client.pyi` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/literals.pyi` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/paginator.pyi` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.py` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact/type_defs.pyi` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post1/types_aiobotocore_codeartifact.egg-info/SOURCES.txt` & `types-aiobotocore-codeartifact-2.5.2.post2/types_aiobotocore_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

